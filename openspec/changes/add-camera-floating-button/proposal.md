# Change: Add Camera Floating Button

## Why
To encourage users to take photos for the campaign, a floating camera button is needed on the mobile version. It allows easy access to the camera function while browsing the steps and incentive section.

## What Changes
- Add a floating button with `open-camera.svg` icon to the mobile view.
- Position the button on the right side of the incentive banner and step buttons.
- Implement sticky/floating behavior so it moves with the scroll but stops at its original top position.
- Configure the button to open the mobile camera when clicked.

## Impact
- Affected specs: `campaign-page`
- Affected code: `new-campaign-2026/index.html`, `new-campaign-2026/css/campaign-2026.css`
