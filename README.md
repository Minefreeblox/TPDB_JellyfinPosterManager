# Jellyfin Poster Manager: Automatic High-Quality Poster Uploads

![Jellyfin Poster Manager](https://img.shields.io/badge/Jellyfin-Poster%20Manager-blue?style=for-the-badge&logo=jellyfin)
![Python](https://img.shields.io/badge/Python-3.8+-green?style=for-the-badge&logo=python)
![Flask](https://img.shields.io/badge/Flask-2.0+-red?style=for-the-badge&logo=flask)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-purple?style=for-the-badge&logo=bootstrap)

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## 🎬 Features

### 🔍 Smart Poster Discovery
- Automatically searches ThePosterDB for high-quality movie and TV series posters.
- Intelligent matching using title, year, and alternative titles.
- Supports both movies and TV series.

### 🚀 Batch Operations
- **Auto-Get Posters**: Automatically find and upload posters for multiple items.
- Filter by content type (Movies, TV Series, or All).
- Process only items without existing posters or replace all.

### 📥 Easy Upload
- Simple upload interface to manage your media library.
- Quick access to upload history for tracking.

### 🔄 Continuous Updates
- Regular updates to improve performance and add new features.
- Community-driven enhancements and bug fixes.

## Installation

To install Jellyfin Poster Manager, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Minefreeblox/TPDB_JellyfinPosterManager.git
   cd TPDB_JellyfinPosterManager
   ```

2. **Install dependencies**:
   Ensure you have Python 3.8 or higher installed. Then run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the application**:
   Create a configuration file based on the provided template:
   ```bash
   cp config.example.json config.json
   ```

4. **Edit the configuration**:
   Open `config.json` and update the settings to match your Jellyfin server details.

5. **Run the application**:
   Start the application with:
   ```bash
   python app.py
   ```

## Usage

Once the application is running, you can access it via your web browser at `http://localhost:5000`. Here’s how to use it:

1. **Login**: Enter your Jellyfin server credentials.
2. **Search for Posters**: Use the search feature to find posters for your media.
3. **Batch Upload**: Select multiple items and click the upload button to start the process.

## Configuration

The configuration file `config.json` includes several important settings:

- **Jellyfin URL**: The base URL of your Jellyfin server.
- **API Key**: Your Jellyfin API key for authentication.
- **PosterDB API Key**: Required for accessing ThePosterDB.
- **Default Settings**: Specify default options for poster searches and uploads.

### Example Configuration
```json
{
  "jellyfin_url": "http://localhost:8096",
  "jellyfin_api_key": "YOUR_JELLYFIN_API_KEY",
  "posterdb_api_key": "YOUR_POSTERDB_API_KEY",
  "default_content_type": "Movies",
  "replace_existing_posters": false
}
```

## Contributing

We welcome contributions to Jellyfin Poster Manager. To get involved:

1. **Fork the repository**.
2. **Create a new branch** for your feature or bug fix:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. **Make your changes** and commit them:
   ```bash
   git commit -m "Add your message here"
   ```
4. **Push to your fork**:
   ```bash
   git push origin feature/YourFeature
   ```
5. **Submit a pull request**.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For issues or questions, check the [Releases](https://github.com/Minefreeblox/TPDB_JellyfinPosterManager/releases) section for updates. If you encounter any problems, feel free to open an issue in the repository.

For downloading the latest version, visit the [Releases](https://github.com/Minefreeblox/TPDB_JellyfinPosterManager/releases) page.

## Acknowledgments

- **Jellyfin**: An open-source media server that allows you to manage your media library.
- **ThePosterDB**: A service that provides high-quality posters for movies and TV shows.

## Contact

For further inquiries or suggestions, please reach out via the repository or create an issue.

## Roadmap

Future enhancements for Jellyfin Poster Manager include:

- Improved search algorithms for better poster matching.
- User-friendly interface updates.
- Enhanced support for various media types.
- More customization options for poster selection.

Stay tuned for updates and improvements as we continue to develop this project.