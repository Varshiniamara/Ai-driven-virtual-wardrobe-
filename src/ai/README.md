# AI Engine

This folder represents the AI Logic simulation. In the production app, this logic is handled by the `Antigravity` agent and Next.js API routes calling LLMs.

## AI logic Files (Simulated)
- `recommendation_engine.py`: Logic for outfit matching.
- `image_analysis.py`: Computer vision for auto-tagging uploaded clothes.
- `trend_forecaster.py`: Scrapes web for fashion trends.

## Integration
The frontend communicates with these services via the Next.js API layer.
