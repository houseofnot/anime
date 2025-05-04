Anime Streaming Website

This is an open-source PHP-based anime streaming website that integrates with MyAnimeList (MAL), AniList, and Jikan API. The website allows users to stream anime, read manga, and track their progress across different platforms (MAL and AniList). This project is designed for personal use and is not intended for commercial purposes.

Table of Contents
- Installation
- Usage
- Configuration
- Documentation
- Contributing
- Disclaimer

Installation

Requirements:
- PHP 8.4+ (Compatible with modern PHP features)
- MySQL or MariaDB database server
- A web server (Apache or Nginx)
- Composer (for dependency management)
- Access to MyAnimeList and AniList APIs

Steps to Install:
1. Clone the repository:
   git clone https://github.com/your-username/anime-streaming-website.git
   cd anime-streaming-website

2. Install dependencies using Composer:
   composer install

3. Set up the database:
   - Create a MySQL or MariaDB database for your project.
   - Import the provided SQL schema to set up the necessary tables (e.g., users, anime, manga).

4. Configure the config.php:
   - Open config/config.php and add your MAL, AniList, and Jikan API keys.
   - Set the booleans $myanimelist and $anilist to true to enable integration with those platforms. If you don’t want to use them, set them to false.

5. Set up a web server (Apache or Nginx):
   - For Apache: Ensure mod_rewrite is enabled and configure .htaccess for clean URLs.
   - For Nginx: Configure your server block to point to the public directory.

6. Run the application:
   - Navigate to your server's URL (e.g., http://localhost/), and the website should be up and running.

Usage

- Login: Users can log in with their MyAnimeList or AniList accounts to sync their anime and manga progress.
- Streaming: Once logged in, users can stream anime or read manga, while their progress is tracked automatically.
- Progress Sync: When a user finishes an episode or chapter, the website will update their progress on MAL or AniList, depending on the configuration.
- Dashboard: Users can view their current anime/manga list and progress through a personal dashboard.

Configuration

1. API Integration:
   - You must configure your MAL and AniList API credentials in config/config.php. You can obtain these from their respective developer platforms.

2. Enable/Disable API Features:
   - Set $myanimelist = true; to enable MAL integration, or false to disable.
   - Set $anilist = true; to enable AniList integration, or false to disable.

3. Database Configuration:
   - In the config.php file, update the $database array to match your database connection details (host, username, password, etc.).

4. Web Server Configuration:
   - The site is built to run on a typical PHP web server. Make sure you configure your server (Apache/Nginx) to serve the files correctly.

Documentation

- MAL API: https://myanimelist.net/apiconfig
- AniList API: https://anilist.gitbook.io/anilist-apiv2-docs/
- Jikan API: https://jikan.docs.apiary.io/

This documentation contains all the necessary information about how to interact with the APIs and how the system is designed.

Contributing

We welcome contributions from the community! If you would like to contribute to this project, please follow these steps:

1. Fork the repository:
   - Click on the "Fork" button at the top right of this page to create your own copy of the repository.

2. Clone your fork:
   git clone https://github.com/your-username/anime-streaming-website.git
   cd anime-streaming-website

3. Create a new branch:
   git checkout -b feature/your-feature-name

4. Make changes:
   - Make sure to write clear, concise commit messages.
   - Follow the existing coding style of the project.

5. Push your changes:
   git push origin feature/your-feature-name

6. Create a pull request:
   - Navigate to the GitHub repository and open a pull request with a description of the changes you made.

---

Disclaimer

This project is for personal use only. It is not intended to be used commercially or for profit. Please do not use it for commercial streaming or any monetization purposes.

By using this software, you agree that the creators are not responsible for any misuse, errors, or legal issues arising from the use of this software.

Thank you for using and contributing to this open-source project! 😊 



