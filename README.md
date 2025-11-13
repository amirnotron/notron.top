# 🌐 notron.top - Dynamic Discord & Spotify Status Page

## 📝 Description

This repository hosts the source code for my dynamic public personal website, **notron.top**.

It's a single-page application designed to display my live **Discord status** (Online, Idle, DND, Offline) and current **Spotify listening activity** using the **Lanyard API**. The design is inspired by the modern Discord UI, featuring custom avatar decoration, background effects, and media controls.

## ✨ Key Features

* **Live Discord Status:** Integrates with the Lanyard API to show real-time user status, avatar, and username.
* **Spotify Activity:** Displays the album art, song title, and artist of the music I'm currently listening to on Spotify via Discord Rich Presence.
* **Aesthetic Design:** Discord-themed UI with a blurred, dynamic background, custom avatar decoration, and `Roboto` font.
* **Background Effects:** Includes a **Snowfall** animation (`#snow-container`) and a smooth background image transition.
* **Interactive Entry Screen:** A full-screen "Click to Enter" prompt that initiates background music playback (prevents browser autoplay restrictions) and displays a pulsing glow effect.
* **Media Control:** A fixed button (`#music-control`) allows users to pause or play the embedded background music (`background-music.mp3`).
* **Responsive Layout:** Fully optimized for mobile screens using CSS `@media` queries.

## 🛠️ Technology Stack

| Component | Usage | Details |
| :--- | :--- | :--- |
| **HTML5** | Structure | Semantic structure for the status page. |
| **CSS3** | Styling/Design | Heavily customized styling, using `@import` for Google Fonts (`Roboto`), custom variables, and complex box-shadows/gradients for the avatar decoration. |
| **JavaScript** | Functionality | Handles API fetching, DOM manipulation, status updates, music control, entry screen, and snowfall animation. |
| **Lanyard API** | Data Fetching | Used to retrieve real-time Discord and Spotify user data. |
| **GitHub** | Hosting | The project is configured for deployment as a static site. |

## 🔗 Setup & Configuration

This page relies on a single **User ID** and a **Background Image URL** for setup.

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/amirnotron/notron.top.git](https://github.com/amirnotron/notron.top.git)
    cd notron.top
    ```

2.  **Required Assets:**
    * Ensure the background music file named **`background-music.mp3`** is in the root directory.

3.  **Update JavaScript Variables:**
    In the `<script>` tag at the bottom of `index.html`, update the following variables with your own data:

    ```javascript
    const manualBannerUrl = 'YOUR_BACKGROUND_IMAGE_URL'; // e.g., '[https://i.pinimg.com/736x/bb/ee/76/bbee7696b6888d205c4de0ec8eb8d991.jpg](https://i.pinimg.com/736x/bb/ee/76/bbee7696b6888d205c4de0ec8eb8d991.jpg)'
    const userId = 'YOUR_DISCORD_USER_ID';              // The Discord ID used for Lanyard API fetching.
    ```

4.  **Deployment:**
    The site can be deployed instantly using GitHub Pages or any static hosting service (Vercel, Netlify).

## 🗂️ File Structure

| File Name | Description |
| :--- | :--- |
| **`index.html`** | Contains all HTML markup, internal CSS, and JavaScript logic. |
| **`background-music.mp3`** | The audio track played when the user clicks the "Enter" screen. |
| **`README.md`** | This documentation file. |

## 🤝 Contact

* **Discord ID (Lanyard Source):** `634488416771244076`
* **GitHub:** [@amirnotron](https://github.com/amirnotron)
* *Add your preferred contact method here (e.g., Email, LinkedIn, etc.)*
