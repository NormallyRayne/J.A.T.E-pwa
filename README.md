# Text Editor Web Application

Welcome to the Text Editor Web Application! This web application provides a robust text editing experience with advanced features such as IndexedDB for content persistence, Webpack for bundling JavaScript files, and service worker integration for offline capabilities. Follow the instructions below to set up and run the application seamlessly.

## Table of Contents

- [Folder Structure](#folder-structure)
- [Getting Started](#getting-started)
- [Webpack Build](#webpack-build)
- [IndexedDB Integration](#indexeddb-integration)
- [Offline Functionality](#offline-functionality)
- [Deployment on Render](#deployment-on-render)

## Folder Structure

Upon opening the application in your text editor, you'll find the following folder structure:

```
/
|-- client
|   |-- // Client-side files and components
|
|-- server
|   |-- // Server-side files and configurations
|
|-- webpack.config.js
|-- package.json
|-- // Other project files
```

## Getting Started

1. Open your terminal and navigate to the root directory of the application.

2. Run the following command to start the application:

```bash
npm run start
```

This command initiates the backend and serves the client, making your application accessible.

## Webpack Build

When running the text editor application, Webpack will bundle your JavaScript files. Ensure you have the necessary dependencies installed and run the webpack plugins:

```bash
npm install
npm run build
```

This generates an HTML file, service worker, and a manifest file for your application.

## IndexedDB Integration

The text editor seamlessly integrates with IndexedDB for content storage. When you open the editor, IndexedDB immediately creates a database storage. Enter content, click off the DOM window, and witness the content being saved in IndexedDB. Closing and reopening the text editor retrieves the content from IndexedDB.

## Offline Functionality

1. Click on the "Install" button to download the web application icon on your desktop.

2. Upon loading, your web application registers a service worker using Workbox.

3. Static assets are pre-cached upon loading, ensuring offline functionality for subsequent pages and static assets.

