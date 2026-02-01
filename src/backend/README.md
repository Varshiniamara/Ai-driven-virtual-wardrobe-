# Backend API

Since this project uses Next.js 15, the "backend" is integrated as Serverless API Routes.

## Structure
The API endpoints are located in `src/frontend/app/api`.

## Endpoints
- `/api/outfits`: Handles outfit generation logic.
- `/api/suggestions`: Returns AI-based clothing suggestions.
- `/api/reminders`: Manages laundry and usage reminders.

## Future Scalability
For a dedicated microservices backend, we would use:
- **Node.js/Express** or **Python/FastAPI** (for AI heavy lifting).
- **PostgreSQL** for persistence.
