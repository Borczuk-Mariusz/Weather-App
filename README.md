# Weather App - Vite + React + TypeScript

A simple weather dashboard built with Vite, React, and TypeScript. This app allows users to **view current weather** for cities worldwide using the [WeatherAPI.com](https://www.weatherapi.com/) service.

---

## 🚀 Features

- **Search for any city** and instantly see the current weather.
- **Save favorite locations** for quick access—cities remain saved between sessions.
- **Drag & drop** saved cities to rearrange their order; the city at the top is highlighted as the main card.
- **Remove saved locations** easily.
- **API key managed securely** using a `.env` file.

---

## 🛠️ Getting Started

### 1. Clone and install

git clone [repository-url]
cd WHEATHER-APP
npm install

### 2. Set up Environment Variables

You need an API key from [WeatherAPI.com](https://www.weatherapi.com/).

- Do **NOT** commit your `.env` file!
- Create a `.env` file in the root directory based on the example below and add your API key.

#### .env.example
VITE_WEATHER_API_KEY=your_weatherapi_key_here

- Replace `your_weatherapi_key_here` with your actual key from WeatherAPI.com.
- Restart the dev server after editing `.env` (required by Vite).

### 3. Run the app

npm run dev

App runs at [http://localhost:5173](http://localhost:5173) by default.

---

## 🖥️ How it works

- **Search:** Enter a city name to see the current weather (temperature, description, wind, humidity, etc.).
- **Save:** Click "Save" to store the city in your saved locations.
- **Drag & Drop:** Rearrange cities by dragging—top city shows as the featured card.
- **Delete:** Use the trash/delete button to remove a city from your saved list.
- **Persistence:** Saved cities and their order are kept in browser `localStorage` and survive page reloads/sessions.

---

## 📚 Development Details

- **Frameworks:** Vite, React, TypeScript
- **API:** [WeatherAPI.com](https://www.weatherapi.com/)
- **State Management:** React hooks + localStorage
- **Drag & Drop:** Recommended: [React DnD](https://react-dnd.github.io/react-dnd/about) or similar.
- **API Key:** Managed via Vite env variable `VITE_WEATHER_API_KEY`.

---

## ⚠️ Best Practices

- Never expose your API key publicly.
- `.env` is excluded in `.gitignore`; only use `.env.example` for reference.
- All environment variables accessed from client-side via Vite must use the `VITE_` prefix.

---

## 📂 Project Structure


src/
.env.example 
.gitignore 
README.md 
---

## 🙌 Contributions

Contributions welcome! Feel free to open issues or PRs for new features or bugfixes.

---

## 📝 License

[MIT](LICENSE.txt)

---

## 🧑‍💻 Demo Instructions

1. Type a city name and search.
2. Save city with the "Save" button.
3. Drag cities to set main card or reorder.
4. Delete unwanted saved cities with the trash button.

---

**Happy coding!**


