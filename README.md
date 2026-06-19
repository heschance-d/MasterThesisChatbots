# MasterThesisChatbots

This repository contains a minimal chatbot interface developed for a user study on conversational AI. The interface is designed to support controlled chatbot interactions in a clean and neutral layout, with minimal branding to reduce bias during participant testing.

The application is built with React, Vite, Tailwind CSS, and the Google Gemini API. It includes a simple chat interface, message history display, loading state, and an option to export the conversation log locally at the end of each session.

## Features

* Minimal chatbot interface for user-study interaction
* React + Vite frontend setup
* Tailwind-based styling
* Gemini API integration
* Local conversation log export as JSON
* Neutral visual design suitable for comparative chatbot studies

## Project Structure

```bash
.
├── src/
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
├── index.html
├── package.json
├── tsconfig.json
├── vite.config.ts
└── README.md
```

## Getting Started

### Prerequisites

Make sure you have Node.js installed.

### Installation

Install the project dependencies:

```bash
npm install
```

### Environment Variables

Create a `.env.local` file in the project root and add your Gemini API key:

```bash
GEMINI_API_KEY=your_api_key_here
```

Do not commit `.env.local` to GitHub.

### Run Locally

Start the development server:

```bash
npm run dev
```

The app will usually be available at:

```bash
http://localhost:3000
```

### Build

To create a production build:

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Data and Privacy Notes

Conversation logs may contain participant responses or other sensitive research data. These exported chatlog files should not be committed to this repository.

## Security Notes

API keys should never be hardcoded in the frontend source code. For public deployment, it is recommended to move API calls to a backend endpoint so that the Gemini API key is not exposed in the browser bundle.

## Research Context

This interface was developed as part of an academic user study exploring how different chatbot conversational styles are perceived by users. The system prompt and interaction design can be adjusted depending on the study condition.

## License

This project is intended for academic and research use. Please check and update the license before public release.
