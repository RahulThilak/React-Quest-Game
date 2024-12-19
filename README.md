# ReactQuest Game

A simple React quiz game that allows users to take a quiz and track their score. The app fetches questions from a static JSON file (`questions.json`) stored in the `public` folder.

## Features

- Start, answer, and navigate through questions with a timer for each.
- Display of score and high score after completing the quiz.
- User-friendly UI with screens for start, question, and finish.

## Technologies Used

- **React**: For building the user interface
- **CSS**: For styling
- **React Hooks**: `useReducer` for state management, `useEffect` for data fetching
- **Static JSON**: Stores quiz questions

## How It Works

The app retrieves quiz questions from `questions.json` in the `public` folder, displaying them one at a time to the user. Each question object in the JSON file includes:

- **question**: The quiz question
- **options**: Multiple choice answers
- **correctOption**: The index of the correct answer
- **points**: Points for a correct answer

### Sample JSON Structure

```json
{
  "questions": [
    {
      "question": "Which is the most popular JavaScript framework?",
      "options": ["Angular", "React", "Svelte", "Vue"],
      "correctOption": 1,
      "points": 10
    }
  ]
}
```

## Key Components

- **Header**: Displays the app's header
- **Loader**: Spinner shown while fetching questions
- **Error**: Displayed if there's an error fetching data
- **StartScreen**: Initial screen before the quiz starts
- **Question**: Displays current question and options
- **NextButton**: Navigates to the next question
- **Progress**: Tracks quiz progress
- **FinishScreen**: Shows quiz results and high score
- **Timer**: Displays remaining time for the question

## Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/react-quest-game.git
   ```

2. **Install Dependencies**:

   ```bash
   cd react-quiz-app
   npm install
   ```

3. **Run the Application**:

   ```bash
   npm start
   ```

   Opens the app at http://localhost:3000.

4. **Build for Production**:
   ```bash
   npm run build
   ```

## React Concepts Used

- **Functional Components**: Modular components for each part of the UI
- **JSX**: Syntax for rendering UI
- **Hooks**: `useState`, `useReducer`, and `useEffect` for managing state and side effects
- **Conditional Rendering**: Dynamically rendered UI based on app states (loading, active, finished)
- **Data Fetching**: Using `fetch()` to retrieve quiz data from JSON
- **Timer**: Countdown functionality for each question
- **Responsive Design**: Styled for various screen sizes
