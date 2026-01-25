## ADDED Requirements
### Requirement: Document Style Layout
The Rules section SHALL be styled as a clean, white content box resembling a document or terms sheet.

#### Scenario: Visual Structure
- **WHEN** the user views the Rules section
- **THEN** it should have a white background with a subtle gray border (approx 1px solid #E5E7EB).
- **AND** the title "活動辦法" should be centered at the top, colored Gray (#9CA3AF), and font-weight bold.
- **AND** there must be a full-width horizontal divider line immediately below the title.

### Requirement: List Formatting
The content within the rules box SHALL be formatted with specific bullet points and indentation.

#### Scenario: List Hierarchy
- **WHEN** displaying main sections (Time, Description, Awards, Notices)
- **THEN** they should be prefixed with a solid black circle bullet (`●`).
- **AND** the section titles should be bold.
- **AND** detail text should be indented to align with the start of the title text (hanging indent).

## MODIFIED Requirements
### Requirement: Collapse Functionality
The collapse/expand functionality SHALL remain, but the "Expand" button visual should be unobtrusive to match the clean document style (or kept as the yellow button if it sits *outside* the document box).

#### Scenario: Expand Button
- **WHEN** viewing the collapsed rules
- **THEN** the gradient fade effect should still be present.
