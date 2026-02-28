# ai-quiz
Name: Amogh Bhat
Tools used: ChatGPT

Q1:

Key finding (2-4 sentences): The hero section and grid layout can be fully responsive using CSS flexbox and grid with appropriate breakpoints. The container should use max-width and padding to prevent content from touching screen edges. Hover effects enhance interactivity and provide visual cues for buttons and cards.

Outlier: The initial plan suggested using fixed pixel widths for all elements, which would break mobile responsiveness.

Q2:

What was broken: On mobile screens, the hero section did not stack vertically; the hero card remained on the right.

What I changed: Added a media query for max-width 600px and changed .hero to flex-direction: column, aligning the card below the text and making it full width.

Q3:
Prompt 1 :
I want to create a responsive portfolio page with a hero section and a grid. Can you give me a plan for implementing breakpoints for desktop, tablet, and mobile, and explain how the hero section should behave on different screen sizes?

Response snippet:

Use flexbox for the hero section to have two columns on desktop and stack vertically on mobile.

Use CSS grid for the cards section with different column counts at desktop, tablet, and mobile breakpoints.

Suggested fixed pixel widths for all elements.

Accepted:

Use flexbox for hero section columns.

Use CSS grid for card layout with breakpoints.

Rejected:

Fixed pixel widths (would break responsiveness; replaced with max-width and percentages).

Prompt 2 (debug):
Problem: My hero section is not stacking correctly on mobile screens; the hero card stays on the right instead of below the text.

CSS snippet asked about:
.hero {
display: flex;
justify-content: space-between;
}

Response snippet:
You need to add a media query for max-width 600px and change .hero to flex-direction: column so that the items stack vertically.

What I verified:

viewport sizes tested: 375px, 768px, 1200px

what I checked visually:

Header logo left, nav right on desktop; stacked and centered on mobile

Hero section two columns on desktop, stacked on mobile

Hero card aligned right on desktop and full width below text on mobile

Grid layout: 4 columns desktop, 2 tablet, 1 mobile

Hover effects for .btn and .card applied correctly

No horizontal scroll or overflow at any breakpoint

Q4:

Chart caption (Gallery images):

Plot 1: This chart shows the monthly sales trends over the past year.

Plot 2: This chart shows quarterly customer satisfaction ratings.

Decision based on chart:

Focus marketing efforts in months where revenue is lower.

Improve customer support in the quarter with the lowest satisfaction scores.
