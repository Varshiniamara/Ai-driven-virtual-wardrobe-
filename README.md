# Virtual Wardrobe - Vibecraft Hackathon Submission

> **Theme**: AI-Driven Utility & Design

---

## 1. Project Title & Short Overview

**Virtual Wardrobe** is an AI-powered digital closet that helps users organize their clothes, plan outfits, and solve the "I have nothing to wear" dilemma. It combines a premium glassmorphism UI with smart categorization.

### 🚀 **Live Demo**: [v0-virtual-wardrobe-website.vercel.app](https://v0-virtual-wardrobe-website.vercel.app/)

## 2. Problem Statement

In today’s fast-paced lifestyle, selecting an outfit that matches one’s skin tone, personal style, and occasion is a common challenge. Most individuals rely on trial and error, generic fashion advice, or limited inspiration, which often results in mismatched outfits and wasted time. Existing fashion platforms lack personalized analysis and fail to adapt recommendations to individual user characteristics. This creates a gap between user expectations and actual fashion outcomes. There is a strong need for a smart, user-centric system that can analyze visual inputs and preferences to deliver accurate, personalized outfit recommendations in real time.

## 3. System Architecture

```mermaid
graph TD
    User[User (Web / Mobile Browser)] -->|Uploads image, Selects preferences| Frontend[Frontend Application (Next.js / React)]
    Frontend -->|API Request| Backend[Backend Server (Next.js API Routes)]
    Backend -->|Routes requests| AI[AI Processing Engine (Gemini 2.0)]
    Backend -->|Store/Retrieve| DB[(Database / LocalStorage)]
    AI -->|Analysis & Recommendations| Backend
    Backend -->|JSON Response| Frontend
    Frontend -->|Displays| Output[Personalized Fashion Output]

    subgraph "AI Capabilities"
    AI --o SkinTone[Skin Tone Analysis]
    AI --o OutfitClass[Outfit Classification]
    AI --o StyleRec[Style Recommendation]
    end
```

### 💻 Core Framework
-   **Next.js 15.2.4**: Leveraging the latest App Router and Server Components for optimal performance.
-   **React 19**: Utilizing the newest concurrent features and server actions.
-   **TypeScript 5**: Strict type safety ensures code reliability and maintainability.

### 🎨 UI & Styling
-   **Tailwind CSS 3.4**: Utility-first styling for a completely custom, responsive design.
-   **Shadcn UI (Radix Primitives)**: Accessible, headless UI components (Dialog, Tabs, Slider, etc.).
-   **Lucide React**: Modern, scalable SVG icons.
-   **Tailwindcss-Animate**: For smooth micro-interactions and transitions.
-   **Next-Themes**: Robust light/dark mode implementation.

### 📊 Data & Functionality
-   **Recharts**: For visualizing wardrobe statistics (cost, usage, color distribution).
-   **Zod + React Hook Form**: Type-safe schema validation for all user inputs.
-   **Date-fns**: Lightweight date manipulation library.
-   **Vaul**: Drawer component for mobile-first interactions.
-   **Sonner**: Toast notifications for user feedback.

### 🧠 AI & Integration
-   **Gemini 2.0 (via Agent)**: Powering the intelligence behind outfit recommendations.
-   **Serverless API Routes**: Handling backend logic within the Next.js infrastructure.

## 5. Setup Instructions

To run this project locally:

1.  Clone the repo:
    ```bash
    git clone https://github.com/Varshiniamara/Ai-driven-virtual-wardrobe-.git
    ```
2.  Navigate to the source code:
    ```bash
    cd src/frontend
    ```
3.  Install Dependencies:
    ```bash
    npm install
    ```
4.  Run Dev Server:
    ```bash
    npm run dev
    ```
5.  Open `http://localhost:3000`.

*See `docs/setup_guide.md` for more details.*

## 6. AI Tools Used

-   **Google DeepMind Antigravity**: For end-to-end code generation and debugging.
-   **LLM Prompting**: For generating component logic and accessibility features.

## 7. Prompt Strategy Summary

We utilized a **Component-Driven AI Strategy**:
-   **Role-Based Prompting**: Assigned the AI roles like "Senior Designer" for UI work.
-   **Iterative Refinement**: Loop of Generate -> Critique -> Polish.
-   **Chain of Thought**: Used for complex logic like the Outfit Recommender algorithm.

*See `prompts/prompts_used.md` and `prompts/prompt_template.md` for full logs.*

## 8. Source Code Overview / Folder Structure

```
Virtual-Wardrobe-main/
├── README.md                # Scorecard & Documentation
├── demo_video.mp4           # 3-Minute Demo
├── src/
│   ├── frontend/            # Next.js Application (Main Logic)
│   ├── backend/             # API Logic
│   └── ai/                  # AI Simulation Scripts
├── prompts/                 # Prompt Engineering Evidence
│   ├── prompt_template.md
│   └── prompts_used.md
├── docs/                    # Reproducibility Docs
│   └── setup_guide.md
└── outputs/                 # Screenshots & Final Output
```

## 9. Final Outputs / Screenshots

(Please refer to the `outputs/` folder for high-res images)

-   **Home Page**: Clean, dark-mode landing.
-   **Wardrobe Grid**: Drag-and-drop interface.
-   **Outfit Builder**: Canvas for mixing items.

## 10. Build Reproducibility Instructions

This project is fully reproducible.
1.  Follow the **Setup Instructions** above.
2.  No external database is required (uses LocalStorage/Mock Data for demo).
3.  Works on Node.js v18+.

## 11. Demo Video Link

[INSERT YOUTUBE/DRIVE LINK HERE]

*(See `demo_video.mp4` in root if uploaded directly)*
