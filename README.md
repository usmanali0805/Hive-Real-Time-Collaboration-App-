# NEXORA frontend

A React + Vite client-side prototype for NEXORA. It includes public marketing pages, mock authentication, protected application routes, workspace creation, messaging, AI assistant UI, notifications, profile/settings, and responsive layouts.

## Run locally
1. Install Node.js 18+.
2. Run `npm install`.
3. Run `npm run dev`.
4. Open the local URL printed by Vite.

## Demo access
Open `/login`. The form is prefilled with `alex@nexora.dev` and `nexora123`; any valid email and password of 6+ characters will work in this mock frontend.

## Important boundaries
- Authentication and persistence are mock-only and stored in localStorage.
- AI replies are deterministic demo responses, not connected to an AI API.
- Socket.IO is intentionally not connected. `src/services/socketService.js` is an integration boundary only.
- Google sign-in, invitations, file uploads, and password reset delivery require backend/provider integration.
- Workspace data and messages persist locally in the browser.
