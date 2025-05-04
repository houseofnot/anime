welcome to Myotakunest

NOTE MAL SUPPORT WONT BE ADDED DUE TO NEEDED TO GET APPLICATION APPROVED

YOU CAN VIEW A LIVE DEMO HERE

This is an open-source PHP-based anime streaming website that integrates with Animepahe api, mangadex api, AniList, and Jikan API. The website allows users to stream anime, read manga, and track their progress across AniList. This project is designed for personal use and is not intended for commercial purposes.

Table of Contents:
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
- Access **AniList** API
- FTP client (for file upload) (or alternate file transfer method of your preference)

Steps to Install:
1. **Download the files**: 
   Download the files from the GitHub repository or the provided link.

2. **Upload the files via FTP**:
   Use your FTP client (such as FileZilla) to upload the files to your web server. Upload all the contents of the repository (including subfolders) to the desired location on your server.
   If youre on Xampp windows drop the files into the "htdocs" directory

4. **Set up the database**:
   - Create a MySQL or MariaDB database on your web server.
   - Import the provided SQL schema to create the necessary tables (e.g., `users`, `anime`, `manga`).

5. **Configure the `config.php`**:
   - Open `config/config.php` and enter your **MAL**, **AniList**, and **Jikan API** keys.
   - Set the booleans `$myanimelist` and `$anilist` to `true` to enable integration with those platforms. If you don’t want to use them, set them to `false`.

6. **Set up a web server** (Apache or Nginx):
   - Ensure that your server has PHP 8.4+ installed.
   - For **Apache**: Ensure `mod_rewrite` is enabled and configure `.htaccess` for clean URLs.
   - For **Nginx**: Make sure your server block is configured to point to the root directory where you uploaded the files.

7. **Access the website**:
   - Once the files are uploaded and configured, open your web browser and navigate to your website's URL (e.g., `http://yourdomain.com`). The website should be live and ready for use.

Usage

- **Login**: Users can log in with their **MyAnimeList** or **AniList** accounts to sync their anime and manga progress.
- **Streaming**: Once logged in, users can stream anime or read manga while their progress is tracked automatically.
- **Progress Sync**: When a user finishes an episode or chapter, the website will update their progress on **MAL** or **AniList**, depending on the configuration.
- **Dashboard**: Users can view their current anime/manga list and progress through a personal dashboard.

Configuration

1. **API Integration**:
   - You must configure your l**AniList** API credentials in the `config.php`. You can obtain these from their respective developer platforms.

2. **Enable/Disable API Features**:
   - Set `$anilist = true;` to enable **AniList** integration, or `false` to disable.

3. **Database Configuration**:
   - In the `config.php` file, update the `$database` array to match your database connection details (host, username, password, etc.).

4. **Web Server Configuration**:
   - The site is built to run on a typical PHP web server. Make sure you configure your server (Apache/Nginx) to serve the files correctly.

Documentation

- **AniList API**: [AniList API Documentation](https://anilist.gitbook.io/anilist-apiv2-docs/)

This documentation contains all the necessary information about how to interact with the APIs and how the system is designed.

Contributing

We welcome contributions from the community! If you would like to contribute to this project, please follow these steps:

1. **Fork the repository**: 
   - Click on the "Fork" button at the top right of this page to create your own copy of the repository.

2. **Clone your fork**:
   - You can clone the forked repository to your local system if you plan on working on it locally.

3. **Make changes**:
   - Make sure to write clear, concise commit messages.
   - Follow the existing coding style of the project.

4. **Push your changes**:
   - After making your changes, push them to your fork.

5. **Create a pull request**:
   - Once you're ready, open a pull request from your fork to the original repository, explaining the changes you made.

Disclaimer

This project is **for personal use only**. It is not intended to be used commercially or for profit. Please do not use it for commercial streaming or any monetization purposes.

By using this software, you agree that the creators are not responsible for any misuse, errors, or legal issues arising from the use of this software.

Thank you for using and contributing to this open-source project! 
