Pest Control Training - Ready-to-deploy package
Generated on: 2025-08-15T02:27:55.030782Z

Contents:
- frontend/: Vite React frontend. Replace src/App.jsx with the canvas version if you want the full UI customization.
- backend/: Node/Express backend that serves /api/content and allows POST to save training-content.json
- Dockerfile (backend), Procfile, render.yaml for easy deployment to Render/Railway
- backend/training-content.json is preloaded with:
  - 50 Core exam questions (mixed beginner/advanced)
  - PA category banks (household_health, wood_destroying, fumigation, turf_ornamental, structural)
  - Flashcards with image URLs + attribution

Quick start (local):
1) Install Node 18+
2) Frontend: cd frontend && npm install && npm run dev (port 5173)
3) Backend: cd backend && npm install && npm start (port 4000)
4) Configure frontend to proxy /api to backend in Vite config or set VITE_API_URL to your backend URL

Deployment notes:
- Deploy backend to Render/Railway/Heroku using the render.yaml/Procfile or Dockerfile
- Build frontend and host on static host (Netlify/Vercel) and point API to the backend URL

If you want, I can replace frontend/src/App.jsx with the full canvas App.jsx (more complex UI), or deploy this for you to a demo URL. 
"# Training" 
