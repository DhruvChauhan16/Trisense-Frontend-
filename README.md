 # TriSense — Frontend

TriSense is a multimodal emotion detection and music recommendation app. This repository contains the **frontend only** — the user interface that captures input, displays detected emotions, and presents music recommendations in real time.

> Note: The emotion-detection model, training pipeline, and backend integration were built by teammates. This repo covers the React/Vite frontend that I designed and developed.

---

## What this frontend does

- Provides a responsive, user-friendly interface for the TriSense experience
- Sends user input data to the backend via REST API calls (fetch/axios) for emotion detection
- Displays the detected emotion and corresponding music recommendations in real time
- Handles UI state for loading, success, and error responses from the API
- Built with a mobile-first, animation-driven design for smooth, engaging interactions

---

## Tech Stack

- **React** — component-based UI
- **Vite** — build tool and dev server
- **Tailwind CSS** — styling and responsive layout

---

## Project Structure

```
├── public/          # Static assets
├── src/             # React components, pages, styles, API calls
├── index.html        # App entry point
├── vite.config.js    # Vite configuration
├── package.json      # Dependencies and scripts
```

---

## Getting Started

### Prerequisites
- Node.js (v16 or higher recommended)
- npm

### Installation

```bash
git clone https://github.com/DhruvChauhan16/Trisense-Frontend-.git
cd Trisense-Frontend-
npm install
```

### Running locally

```bash
npm run dev
```

The app will be available at `http://localhost:5173` (default Vite port).

### Build for production

```bash
npm run build
```

---

## API Integration

This frontend expects a backend API endpoint that accepts user input (e.g., image/audio/text depending on the modality) and returns the detected emotion along with recommended tracks. API base URL and endpoint configuration can be set in the relevant config/`.env` file used in `src/`.

> If you're reviewing this project: the model training, multimodal data processing, and backend logic live in a separate repository maintained by my teammates. This repo is scoped to the frontend implementation.

---

## My Contribution

- Designed and built the complete UI/UX for the TriSense application
- Implemented responsive layouts using Tailwind CSS
- Built reusable React components for input capture, emotion display, and music recommendation results
- Integrated frontend with backend REST APIs for real-time data exchange
- Handled UI states (loading, error, success) for a smooth user experience during API calls
