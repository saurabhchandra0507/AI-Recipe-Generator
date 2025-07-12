# AI-Recipe-Generator


<img width="1467" alt="Screenshot 2025-07-10 at 12 28 08 AM" src="https://github.com/user-attachments/assets/42de2317-cfb4-40be-8177-9016cbdbdf03" />

## Prototype
<img width="1370" height="677" alt="Screenshot 2025-07-11 at 9 25 41 PM" src="https://github.com/user-attachments/assets/1c33fa83-d650-472e-aead-f5a8c18bcbfc" />



AI Recipe Generator is a web application that uses OpenAI's GPT models to generate creative and detailed recipes based on user-provided ingredients and preferences. The app streams the recipe in real-time as it's generated, providing an interactive and engaging experience.

## Features

- **Custom Recipe Generation:** Enter your available ingredients, meal type, cuisine, cooking time, and complexity to get a unique recipe.
- **Real-Time Streaming:** Recipes are streamed live from the AI, so you see the recipe as it's being created.
- **Modern Tech Stack:** Built with a React frontend and a Node.js/Express backend.
- **OpenAI Integration:** Uses OpenAI's GPT models for high-quality, context-aware recipe generation.

## How It Works

1. **Frontend (React):**
   - Users input their ingredients and preferences.
   - Sends a request to the backend to generate a recipe.
   - Displays the recipe as it streams in from the server.

2. **Backend (Express):**
   - Receives user input via an API endpoint.
   - Formats a prompt for the OpenAI API.
   - Streams the AI-generated recipe back to the frontend using Server-Sent Events (SSE).

3. **OpenAI API:**
   - Processes the prompt and generates a recipe in real-time.

## Project Structure

```
client/recipe-generator/   # React frontend (UI, user input, recipe display)
server/                   # Express backend (API, OpenAI integration)
```

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm or yarn
- OpenAI API key

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ai-recipe-generator.git
   cd ai-recipe-generator
   ```

2. **Install backend dependencies:**
   ```bash
   cd server
   npm install
   ```

3. **Install frontend dependencies:**
   ```bash
   cd ../client/recipe-generator
   npm install
   ```

4. **Set your OpenAI API key:**
   - In `server/server.js`, replace the placeholder with your actual OpenAI API key.

5. **Run the backend server:**
   ```bash
   cd ../../server
   node server.js
   ```

6. **Run the frontend app:**
   ```bash
   cd ../client/recipe-generator
   npm start
   ```

7. **Open your browser and go to:**  
   `http://localhost:3000`

## Usage

- Enter your ingredients and preferences in the UI.
- Click "Generate Recipe".
- Watch as your custom recipe streams in live!



**Note:** This project uses the OpenAI API, which may incur costs. Please review OpenAI's pricing and usage policies.
