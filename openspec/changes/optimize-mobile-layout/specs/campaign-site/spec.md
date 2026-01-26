## MODIFIED Requirements
### Requirement: Responsive Layout
The campaign page MUST adapt to different screen sizes.

#### Scenario: Mobile View Optimization
- **WHEN** viewed on a mobile device (width < 768px)
- **THEN** the layout adjusts to stack elements vertically
- **BUT** the hero buttons remain horizontal (side-by-side)
- **AND** hero title font sizes are increased
- **AND** hero subtitle is moved up to clear character area
- **AND** character images are positioned at bottom corners (Scheme A)
- **AND** the desktop layout remains unchanged

#### Scenario: Desktop Button Scaling
- **WHEN** viewed on desktop screens (width >= 768px)
- **THEN** hero buttons scale proportionally using clamp(500px, 40vw, 800px)
- **AND** buttons remain readable on small laptops (min 500px)
- **AND** buttons don't become too large on wide screens (max 800px)
- **AND** on 1920px screens, buttons display at approximately 40% viewport width
