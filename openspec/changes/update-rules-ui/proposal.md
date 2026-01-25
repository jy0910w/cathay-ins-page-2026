# Change: Update Rules Section UI

## Why
The current "Rules" (活動辦法) section implementation needs to match the specific visual design provided in `活動辦法.jpg`. The previous assumption of a "Yellow Card" style was incorrect. The actual design reflects a clean, document-style layout with a minimalistic aesthetic, emphasizing readability for long text content.

## What Changes
- **Visual Style**: Implement a clean, white "Paper/Document" style container.
- **Typography & Layout**: 
    - Title "活動辦法" centered at the top with specific gray styling.
    - A distinct horizontal separator line between the title and the content.
    - Content formatted as a structured list with black bullet points (`●`) for main section headers.
    - Indented content for details.
- **Structure**: Ensure the container has a subtle border/shadow to resemble a sheet of paper or a clean content box, rather than a vibrant marketing card.

## Impact
- **Affected Specs**: `rules`
- **Affected Code**: `index.html`, `css/campaign-2026.css`
