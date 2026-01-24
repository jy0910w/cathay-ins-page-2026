# Design: Camera Floating Button Implementation

## Context
The campaign requires users to record a dance video. To facilitate this on mobile, a floating button will be added that directly triggers the video camera.

## Decisions
- **Implementation Method**: Use hidden HTML `<input type="file">` element.
- **Attributes**:
    - `accept="video/*"`: To restrict selection to video files.
    - `capture="environment"`: To prefer the rear camera for recording the dance (higher quality than front camera).
- **Interaction**: The floating button will trigger the hidden input's click event.
- **Positioning**: Use CSS `position: sticky` or JavaScript-based scroll monitoring if sticky is not viable within the specific container layout (Step 1-3 area).

## Technical Constraints
- **iOS/Android Webview**: Some in-app browsers (Line, FB) might behave differently, but `accept="video/*"` is the standard fallback.
