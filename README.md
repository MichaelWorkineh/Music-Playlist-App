# 🎵 Music Playlist App

A responsive web application built with React that allows users to search for songs, view song details (including lyrics), and create personalized playlists. This project integrates a free public music API (e.g., [Deezer API](https://developers.deezer.com/api)) to fetch real-time music data, making it a perfect showcase for API integration, state management, and UI/UX design skills.

---

## 🚀 Features

### 🔍 **Search for Songs or Artists**
- Search for songs by title or artists by name.
- Display search results with song/album details:
  - Song title
  - Artist name
  - Album cover
  - Play preview (if supported by the API)

### 🎶 **View Song Details**
- Click on a song to view detailed information:
  - Song title and artist
  - Album name and cover
  - Song duration
  - Release date
  - Lyrics (if available via an additional lyrics API)

### 📂 **Create and Manage Playlists**
- Create custom playlists by adding songs from search results.
- Save playlists with unique names.
- View, edit, and delete playlists.
- Store playlists persistently in **local storage**.

### 🕹️ **Interactive Features**
- Play song previews directly from the app.
- Drag-and-drop functionality to reorder songs in playlists (optional feature).
- User-friendly error handling for API rate limits or network issues.

### 📱 **Responsive Design**
- Fully responsive layout that works seamlessly on mobile, tablet, and desktop devices.
- Music-themed UI with support for **dark mode** (optional).

---

## 🛠️ Tech Stack

### **Frontend**
- **React**: For building the user interface and managing state.
- **React Router**: For navigation between pages (e.g., Home, Search, Playlists).
- **Axios**: For making API calls.
- **CSS Framework**: Styled with **TailwindCSS** or **Material-UI** for a sleek, responsive design.

### **APIs**
- **[Deezer API](https://developers.deezer.com/api)**: For fetching music data such as songs, albums, and artists.
- **[Lyrics.ovh](https://lyricsovh.docs.apiary.io/)** (optional): For fetching song lyrics.
- **[Musixmatch API](https://developer.musixmatch.com/)** (alternative): For more advanced lyrics integration.

### **State Management**
- **React Context API**: For managing global state (e.g., playlists).
- **LocalStorage**: For persisting playlists across sessions.

---

## 📂 Project Structure

```plaintext
Music-Playlist-App/
├── public/
│   └── index.html       # Main HTML file
├── src/
│   ├── components/      # Reusable UI components (e.g., SongCard, PlaylistCard)
│   ├── pages/           # Page components (e.g., Home, Search, Playlist Details)
│   ├── hooks/           # Custom React hooks (e.g., useDebouncedValue, useCachedApi)
│   ├── context/         # Context API setup for global state management
│   ├── styles/          # Global and component-specific styles
│   ├── App.js           # Main App component
│   ├── index.js         # React entry point
│   └── utils/           # Utility functions for API calls, caching, etc.
├── package.json         # NPM dependencies and scripts
└── README.md            # Project documentation
```

---

## 🔧 Installation and Setup

Follow these steps to run the project locally:

### 1. Clone the repository:
```bash
git clone https://github.com/your-username/music-playlist-app.git
cd music-playlist-app
```

### 2. Install dependencies:
```bash
npm install
```

### 3. Create and configure an `.env` file:
- Add your API keys or endpoints for the music API and lyrics API (if applicable).
- Example:
  ```plaintext
  REACT_APP_DEEZER_API_BASE_URL=https://api.deezer.com
  REACT_APP_LYRICS_API_BASE_URL=https://api.lyrics.ovh/v1
  ```
- Make sure to replace these with the actual API URLs or keys as needed.

### 4. Start the development server:
```bash
npm start
```

### 5. Open your browser:
Visit [http://localhost:3000](http://localhost:3000) to view the app.

---

## 🖥️ Demo

Check out a live demo of the project: [Music Playlist App Live Demo](#)  
---

## 🚨 Key Challenges and Solutions

### 1. **Handling API Rate Limits**
- Implemented **caching** to store previously fetched results and reduce API calls.
- Used **debouncing** for search input to limit requests during typing.
- Added **retry logic** to handle `429 Too Many Requests` errors gracefully.

### 2. **Data Persistence**
- Used **LocalStorage** to save playlists, ensuring they persist across browser sessions.
- Future improvement: Add a backend to store playlists in a database.

### 3. **Responsive Design**
- Used **CSS Flexbox** and **Grid** for a responsive layout.
- Tested the app on multiple screen sizes to ensure a seamless experience.

---

## 🛣️ Roadmap

### Future Enhancements:
- **User Authentication**: Allow users to log in and save playlists to the cloud.
- **Drag-and-Drop Reordering**: Add functionality to reorder songs within playlists.
- **Music Recommendations**: Suggest similar songs or artists based on user preferences.
- **Dark Mode**: Add a toggle for dark/light theme.

---

## 🤝 Contributing

Contributions are welcome! Please follow the steps below to contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes and push to the branch:
   ```bash
   git commit -m "Add your feature description"
   git push origin feature/your-feature-name
   ```
4. Open a pull request describing your changes.

---

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## 📧 Contact

Have any questions or feedback? Feel free to reach out!

- **Your Name**: [Email](mailto:micwor96@gmail.com)

---

**Enjoy creating your playlists! 🎶**
```

