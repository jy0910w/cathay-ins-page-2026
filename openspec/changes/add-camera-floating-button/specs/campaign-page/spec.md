## ADDED Requirements
### Requirement: Floating Camera Button
The mobile interface SHALL display a floating camera button on the right side of the incentive banner and step buttons area.

#### Scenario: Display and Positioning
- **WHEN** the user views the page on a mobile device
- **THEN** a button with the `open-camera.svg` icon appears on the right side of the steps/incentive section
- **AND** the button moves down as the user scrolls (sticky behavior)
- **AND** the button stops at its original position when scrolled to the top.

#### Scenario: Open Video Camera
- **WHEN** the user clicks the floating camera button
- **THEN** the mobile device's video recording interface is opened directly (where supported)
- **AND** the input only accepts video files.
