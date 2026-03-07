# Todo

## Backend
- [ ] Set up FastAPI project structure with uv
- [ ] Implement SQLite database with lazy initialization and schema
- [ ] Implement market data simulator (GBM-based price generation)
- [ ] Implement Massive API client (optional, env-variable driven)
- [ ] SSE streaming endpoint (`/api/stream/prices`)
- [ ] Portfolio API endpoints (positions, trade execution, history)
- [ ] Watchlist API endpoints (get, add, remove)
- [ ] Chat API endpoint with LLM integration (LiteLLM → OpenRouter/Cerebras)
- [ ] Structured output parsing for LLM responses
- [ ] Auto-execution of trades and watchlist changes from LLM
- [ ] LLM mock mode (`LLM_MOCK=true`)
- [ ] Portfolio snapshot background task (every 30s)
- [ ] Health check endpoint

## Frontend
- [ ] Set up Next.js TypeScript project with static export
- [ ] Configure Tailwind CSS with dark theme
- [ ] SSE connection via `EventSource` to `/api/stream/prices`
- [ ] Watchlist panel with price flash animations and sparklines
- [ ] Main chart area (Lightweight Charts or Recharts)
- [ ] Portfolio heatmap (treemap)
- [ ] P&L chart (portfolio value over time)
- [ ] Positions table
- [ ] Trade bar (buy/sell market orders)
- [ ] AI chat panel with inline trade/watchlist confirmations
- [ ] Header with live portfolio value, cash balance, connection status

## Infrastructure
- [ ] Multi-stage Dockerfile (Node build → Python runtime)
- [ ] Docker volume for SQLite persistence
- [ ] `start_mac.sh` / `stop_mac.sh` scripts
- [ ] `start_windows.ps1` / `stop_windows.ps1` scripts
- [ ] `.env.example` file

## Testing
- [ ] Backend unit tests (pytest): market data, portfolio, LLM, API routes
- [ ] Frontend unit tests: components, price flash, watchlist, chat
- [ ] E2E Playwright tests in `test/` with `docker-compose.test.yml`
- [ ] LLM mock mode integration for E2E tests

## Completed
- [x] Market data component (simulator + Massive API client, shared price cache)
