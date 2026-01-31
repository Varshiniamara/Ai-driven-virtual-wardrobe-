# Prompt Engineering & Strategy

## Strategy Overview
Our approach to building the Virtual Wardrobe relied on **Iterative & Component-Driven Development**. We utilized advanced AI assistants to generate code, adhering to strict design guidelines.

### Phases
1.  **Foundation**: Defining the design system (Tailwind config, color palette, typography).
2.  **Component Generation**: creating atomic components (Buttons, Cards, Inputs) before complex UIs.
3.  **Page Assembly**: Composition of components into full pages.
4.  **Refinement**: Aesthetic polishing and animation integration.

## AI Tools Used
- **Google DeepMind Antigravity**: For end-to-end coding, project structure, and debugging.
- **LLM for Code Generation**: Used to generate boilerplate and logic for Next.js 13+ App Router.

## Prompt Templates Used

### Template 1: Initial Skeleton & Design System
> "Create a Next.js web application for a Virtual Wardrobe. Use TailwindCSS for styling. Implement a premium, dark-mode first design with glassmorphism effects. Start by defining the `index.css` and `tailwind.config.ts` with a vibrant color palette."

### Template 2: Component Creation
> "Create a reusable `ClothingCard` component. It should accept an image, title, and tags. Use the defined design tokens. Ensure it has a hover effect that scales the card slightly and shows a 'View Details' button."

### Template 3: Feature Implementation
> "Implement the logic for the 'Outfit Creator'. Allow users to drag and drop items from the sidebar onto a canvas. Use a grid layout. Ensure the state is managed efficiently."

## Log of Prompts Used
1.  *Initial Setup*: "Setup a Next.js project with TypeScript and Tailwind."
2.  *Design*: "Create a modern, sleek navbar with a blurred background."
3.  *Logic*: "Write a hook `useWardrobe` to manage add/remove/update operations for clothing items."
4.  *Hackathon Compliance*: "Add detailed README and documentation required for submission."
