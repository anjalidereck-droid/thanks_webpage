# Docking Console

A creative, fully self-contained thank-you gift for my MSc supervisor, presented as an interactive molecular docking dashboard. Rather than a traditional thank-you card, this is an engaging single-file webpage that merges scientific accuracy, interaction design, and web engineering.

## Project Intent

This project reimagines a simple gesture of gratitude as an interactive experience. By styling it as a computational chemistry interface featuring real PDB protein structure 4A7T and co-crystallized ligand 5FW, it combines:

- Genuine scientific data with interactive storytelling
- Technical craftsmanship to create a memorable experience
- Zero external dependencies—pure frontend implementation

The project is intentionally designed to be forked and adapted. Users can modify the message, color scheme, and molecular target to create personalized versions for any occasion.

## How It Works

The application uses a two-page interface model to deliver its narrative:

**Page 1: The Laboratory Console**

Presents an illustrated laboratory scene featuring the real target protein (4A7T) and its bound ligand (5FW). The interactive "RUN DOCKING" button triggers a sequence of animations and audio playback. An original synth composition accompanies the docking simulation, with a progress bar providing visual feedback throughout the interaction.

**Page 2: The Results Dashboard**

Following successful docking simulation, the interface transitions to a styled laboratory report. This page reveals the actual thank-you message with accompanying confetti animation and celebratory effects.

## Technical Implementation

### Frontend Development

Implementation utilizes vanilla HTML, CSS, and JavaScript without external frameworks or build tools. The codebase consists of approximately 800 lines organized within a single file, maintaining clean separation of concerns through structured commenting and logical organization.

### Cascading Style Sheets (CSS)

Advanced CSS techniques are employed throughout the project:

- Responsive Typography: Fluid scaling using CSS clamp() function for adaptation across device sizes
- Visual Effects: Implementation of neon glow text shadows, procedural gradient hazard stripes, and smooth page transitions
- Design System: Centralized color palette using CSS custom properties for maintainable theming
- Accessibility Considerations: Inclusion of prefers-reduced-motion media query to respect user motion preferences
- Pseudo-elements: Strategic use of ::before and ::after for decorative elements without DOM inflation

### JavaScript Interactivity

Core JavaScript capabilities include:

- Event handling and application state management
- Dynamic DOM manipulation through class-based element toggling
- Audio playback synchronization and lifecycle management
- Animation frame requests for smooth motion rendering
- Template element cloning for efficient UI component reuse

### User Interface and User Experience Design

The interface employs a cohesive dark theme reflecting scientific instrument aesthetics. Design decisions include:

- Neon-inspired color palette with purpose-driven accent colors
- Temporal animations and transitions for visual polish
- Structured typography hierarchy using Google Fonts integration
- Responsive layout architecture scaling from mobile to desktop viewports

### Audio Production and Web Audio Integration

An original synth composition was created specifically for this project and integrated using the Web Audio API. The implementation includes looping audio with proper resource cleanup.

### Scientific Data Integration

Real molecular data from the Protein Data Bank (4A7T structure, 5FW ligand) is incorporated into the interface design, demonstrating the ability to blend domain-specific scientific knowledge with frontend development.

### Software Engineering Best Practices

Code architecture demonstrates professional standards:

- Semantic HTML structure following accessibility guidelines
- Organized CSS with clear sectioning and inline documentation
- Minimal technical debt with straightforward code organization
- Git-friendly single-file format eliminating build artifacts and external dependencies

## File Structure

The project comprises the following components:

```
thank-you-professor-berry-commented.html    Single-file implementation (~800 lines)
README.md                                   Project documentation
```

## Usage Instructions

### Direct Browser Access

Double-click the thank-you-professor-berry-commented.html file or right-click and select "Open with Default Browser."

### VS Code Live Server Extension

Right-click the HTML file within the explorer panel and select "Open with Live Server" for hot-reload development.

### Local Python Server

```powershell
cd /path/to/repository
python -m http.server 8000
```

Access the application at `http://localhost:8000/thank-you-professor-berry-commented.html`.

## Customization and Extension

The codebase is structured for straightforward modification and personalization:

1. Message Customization: Locate the heading and paragraph elements in the Page 2 markup section
2. Color Scheme Modification: Edit CSS custom properties defined within the :root selector
3. Molecular Target Substitution: Replace PDB codes (4A7T) and ligand identifiers (5FW) as needed
4. Audio Integration: Encode custom audio files and update the Web Audio API implementation section

## Audio Attribution

The background theme is an original composition created specifically for this project and is not derived from the copyrighted Dexter's Laboratory theme.

## Context

This project was developed as a thank-you acknowledgment to my MSc supervisor and represents a demonstration of frontend development methodology emphasizing clean code principles, thoughtful design, and user-centered interactivity.
