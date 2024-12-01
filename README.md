# YouTube Export Meta Data

![YouTube Export Meta Data Banner](https://via.placeholder.com/1200x300?text=YouTube+Export+Meta+Data)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Getting a YouTube Data API Key](#getting-a-youtube-data-api-key)
- [Technologies Used](#technologies-used)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Overview

**YouTube Export Meta Data** is a web application that allows users to fetch, view, and analyze metadata from any public YouTube channel. By providing a YouTube Data API key and the Channel ID, users can retrieve comprehensive information about the channel's videos, including view counts, likes, comments, and more. The application offers an interactive data table with export functionalities and dynamic charts for visual analysis.

## Features

- **API Integration:** Connects to the YouTube Data API to fetch channel and video metadata.
- **Interactive Data Table:** Displays video data with sorting, searching, and pagination.
- **Export Options:** Export data in CSV, Excel, PDF, and Print formats.
- **Column Visibility Control:** Easily show or hide table columns using DataTables' built-in `colvis` button.
- **Thumbnail Download:** Download video thumbnails directly from the data table.
- **Dynamic Charts:** Visualize data with ApexCharts, including top videos by views, likes vs. views, and top comments.
- **Dark Mode:** Toggle between light and dark themes for optimal viewing.
- **Persistent Settings:** API key and theme preferences are saved in local storage for convenience.
- **Ko-fi Support:** Includes a Ko-fi widget for donations and support.

## Demo

![Demo Screenshot](https://via.placeholder.com/800x600?text=Demo+Screenshot)

_Note: Replace the above placeholder image with actual screenshots of your application._

## Prerequisites

- **Web Browser:** Latest versions of Chrome, Firefox, Edge, or Safari.
- **YouTube Data API Key:** Required to fetch data from YouTube. [Learn how to obtain one](#getting-a-youtube-data-api-key).
- **Internet Connection:** Required to load external libraries and fetch data from YouTube.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/youtube-export-meta-data.git
   ```

2. **Navigate to the Project Directory:**

   ```bash
   cd youtube-export-meta-data
   ```

3. **Open the Application:**

   - Simply open the `index.html` file in your preferred web browser.

   - **OR**

   - Serve the directory using a local server for better performance and to avoid CORS issues.

     ```bash
     # Using Python 3.x
     python -m http.server 8000
     ```

     Then, navigate to `http://localhost:8000` in your browser.

## Usage

1. **Obtain a YouTube Data API Key:** [Follow the instructions here](#getting-a-youtube-data-api-key).

2. **Retrieve the YouTube Channel ID:**

   - Navigate to the YouTube channel's page.
   - The Channel ID can be found in the URL. It typically looks like `UCxxxxxxxxxxxxxxxxxxxxxx`.

   - **Example:** In `https://www.youtube.com/channel/UCabcd1234efgh5678ijkl`, the Channel ID is `UCabcd1234efgh5678ijkl`.

3. **Enter Credentials:**

   - Open the application in your browser.
   - Enter your **YouTube API Key** and **Channel ID** in the respective fields.
   - Click on the **"Fetch Meta Data"** button.

4. **Interact with the Data Table:**

   - **Sorting & Searching:** Click on column headers to sort. Use the search box to filter results.
   - **Export Data:** Use the export buttons (`CSV`, `Excel`, `PDF`, `Print`) to export the data.
   - **Column Visibility:** Click on the **"Columns"** button to show or hide specific columns.
   - **Download Thumbnails:** Use the **"Download"** dropdown under the **"Thumbnail"** column to download different sizes of thumbnails.

5. **View Charts:**

   - Navigate to the **"Charts"** tab to view dynamic visualizations of your channel's data.

6. **Toggle Dark Mode:**

   - Use the **Dark Mode** switch at the top-right to toggle between light and dark themes.

7. **Support the Developer:**

   - Use the **Ko-fi** widget at the bottom-left to make a donation or show support.

## Getting a YouTube Data API Key

To fetch data from YouTube, you need a YouTube Data API key. Follow these steps to obtain one:

1. **Create a Google Cloud Project:**

   - Go to the [Google Cloud Console](https://console.cloud.google.com/).
   - Click on **"Select a project"** and then **"New Project"**.
   - Enter a project name and click **"Create"**.

2. **Enable YouTube Data API:**

   - In the Cloud Console, navigate to **"APIs & Services"** > **"Library"**.
   - Search for **"YouTube Data API v3"**.
   - Click on it and then click **"Enable"**.

3. **Create Credentials:**

   - Go to **"APIs & Services"** > **"Credentials"**.
   - Click on **"Create Credentials"** > **"API Key"**.
   - Your API key will be generated. Copy and store it securely.

4. **Restrict Your API Key (Recommended):**

   - In the **"Credentials"** section, click on your API key.
   - Under **"Application restrictions"**, choose the appropriate restriction (e.g., HTTP referrers).
   - Under **"API restrictions"**, select **"Restrict key"** and choose **"YouTube Data API v3"**.
   - Click **"Save"**.

_For detailed instructions, refer to Google's [official documentation](https://developers.google.com/youtube/v3/getting-started)._

## Technologies Used

- **HTML5 & CSS3:** Structure and styling of the application.
- **Bootstrap 5:** Responsive design and pre-built components.
- **jQuery:** Simplified JavaScript operations.
- **DataTables:** Advanced table features like sorting, searching, pagination, and exporting.
- **ApexCharts:** Interactive and responsive charts for data visualization.
- **FileSaver.js:** Enables file downloads directly from the browser.
- **Bootstrap Icons:** Iconography for better UI/UX.
- **Ko-fi Widget:** Integration for donations and support.
- **Local Storage:** Persists user preferences like API key and theme.

## Troubleshooting

- **CORS Issues When Downloading Thumbnails:**

  - Ensure that your browser allows cross-origin requests.
  - If you encounter CORS-related errors, consider serving the application via a local server.

- **API Quota Exhausted:**

  - The YouTube Data API has quota limits. If you exceed your quota, you'll need to wait until it resets or request higher quotas from Google.

- **Invalid API Key or Channel ID:**

  - Double-check that your API key is correct and active.
  - Ensure that the Channel ID is accurate and corresponds to a public YouTube channel.

- **Data Not Loading:**

  - Verify your internet connection.
  - Check the browser console for any error messages.

## Contributing

Contributions are welcome! If you have suggestions, bug reports, or enhancements, please open an issue or submit a pull request.

1. **Fork the Repository**
2. **Create a Feature Branch**

   ```bash
   git checkout -b feature/YourFeatureName
   ```

3. **Commit Your Changes**

   ```bash
   git commit -m "Add Your Feature"
   ```

4. **Push to the Branch**

   ```bash
   git push origin feature/YourFeatureName
   ```

5. **Open a Pull Request**

## License

This project is licensed under the [MIT License](LICENSE).

---

_Feel free to customize this README to better fit your project's specifics and to include any additional sections as needed._
