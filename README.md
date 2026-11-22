# 🍽️ Recipe Finder (Vite + React)

Search recipes from the free [TheMealDB API](https://www.themealdb.com/api.php), filter by category, and save favorites with `localStorage`.

## Setup (how this project was created)
```bash
npm create vite@latest recipe-finder -- --template react
cd recipe-finder
npm install
npm run dev
```

## Features
- Data fetching with `fetch` + `useEffect` (500ms debounce on search)
- Loading spinner and error message with a retry button
- Search by name + category filter
- Favorites saved in `localStorage` (custom `useLocalStorage` hook)
- Recipe details modal (ingredients + instructions)

## Structure
- `src/api.js` – API call
- `src/hooks/useLocalStorage.js` – saves state to localStorage
- `src/components/` – SearchBar, MealList, MealCard, MealModal, Loading, ErrorMessage
- `src/App.jsx` – state, fetching, filtering
