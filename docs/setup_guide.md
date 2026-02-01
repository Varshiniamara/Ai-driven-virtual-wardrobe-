# Setup Guide

## Prerequisites
- Node.js v18+
- npm or pnpm
- Git

## Installation Steps

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/Varshiniamara/Ai-driven-virtual-wardrobe-.git
    cd Virtual-Wardrobe-main
    ```

2.  **Navigate to Frontend**
    ```bash
    cd src/frontend
    ```

3.  **Install Dependencies**
    ```bash
    npm install
    # or
    pnpm install
    ```

4.  **Environment Setup**
    Create a `.env.local` file in `src/frontend`:
    ```bash
    NEXT_PUBLIC_API_URL=http://localhost:3000
    ```

5.  **Run Development Server**
    ```bash
    npm run dev
    ```

6.  **Build for Production**
    ```bash
    npm run build
    npm start
    ```
