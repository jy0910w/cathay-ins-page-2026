# Design: Camera Floating Button Implementation

## Context
The campaign requires users to record a dance video. To facilitate this on mobile, a floating button will be added that directly triggers the video camera.

## Decisions
- **Implementation Method**: Use hidden HTML `<input type="file">` element.
- **Attributes**:
    - `accept="video/*"`: To restrict selection to video files.
    - `capture="environment"`: To prefer the rear camera for recording the dance (higher quality than front camera).
- **Interaction**: The floating button will trigger the hidden input's click event.
- **Save Workaround**: Since web input capture does not consistently save to the device's gallery (especially on iOS), the application will automatically trigger a file download of the captured video blob immediately after recording.
    - **Android**: Most devices/browsers will download silently or with a non-intrusive notification.
    - **iOS**: Will always prompt "Do you want to download?".
    - **Decision**: Accept this native behavior difference. Force-download is the most reliable cross-platform method to ensure the user gets the file. Provide OS-specific alert messages to guide user expectations (iOS users need to know to look for the "Download" prompt).
- **Positioning**: Use CSS `position: sticky` or JavaScript-based scroll monitoring if sticky is not viable within the specific container layout (Step 1-3 area).

## Technical Constraints
- **iOS/Android Webview**: Some in-app browsers (Line, FB) might behave differently, but `accept="video/*"` is the standard fallback.
- **iOS Download Behavior**: On iOS (both Safari and Chrome), the browser enforces a security prompt ("Do you want to download...?") for programmatic blob downloads. It will not silently save to the device like Android often does. This is an OS-level restriction and cannot be bypassed.
