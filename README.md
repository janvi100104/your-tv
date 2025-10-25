# Your TV

A modern movie search and discovery web application built with React and Vite. Instantly search for movies, view trending titles, and enjoy a smooth, responsive user experience.

## Features

- **Search Movies:** Find movies by title using the search bar with debounced input for performance.
- **Trending Movies:** See a list of trending movies fetched from a backend (Appwrite integration).
- **Popular Movies:** Browse popular movies by default.
- **Movie Details:** View movie posters and titles in a clean card layout.
- **Loading Spinner:** Visual feedback while fetching data.
- **Error Handling:** User-friendly error messages for failed searches or network issues.
- **Responsive Design:** Works well on desktop and mobile devices.

## Tech Stack

- **Frontend:** React, Vite
- **API:** [The Movie Database (TMDb) API](https://www.themoviedb.org/documentation/api)
- **Backend:** Appwrite (for trending movies and search count)
- **Styling:** CSS

## Getting Started

### Prerequisites
- Node.js (v16 or above recommended)
- npm or yarn
- TMDb API Key ([Get one here](https://www.themoviedb.org/settings/api))
- Appwrite instance (optional, for trending/search count)

### Installation

1. **Clone the repository:**
	```bash
	git clone <your-repo-url>
	cd movie-app
	```
2. **Install dependencies:**
	```bash
	npm install
	# or
	yarn install
	```
3. **Set up environment variables:**
	- Create a `.env` file in the root directory.
	- Add your TMDb API key:
	  ```env
	  VITE_TMDB_API_KEY=your_tmdb_api_key_here
	  ```
	- (Optional) Configure Appwrite credentials in `src/appwrite.js`.

4. **Run the development server:**
	```bash
	npm run dev
	# or
	yarn dev
	```
	The app will be available at `http://localhost:5173` (default Vite port).

## Project Structure

```
movie-app/
├── public/
├── src/
│   ├── assets/           # Images and icons
│   ├── components/       # React components (MovieCard, Search, Spinner)
│   ├── App.jsx           # Main app logic
│   ├── appwrite.js       # Appwrite integration
│   └── main.jsx          # Entry point
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

## Environment Variables
- `VITE_TMDB_API_KEY`: Your TMDb API key (required)
- Appwrite credentials: Set in `src/appwrite.js` (if using Appwrite)

## Credits
- Movie data provided by [TMDb](https://www.themoviedb.org/)
- Built with [React](https://react.dev/) and [Vite](https://vitejs.dev/)

## License

This project is licensed under the MIT License.
