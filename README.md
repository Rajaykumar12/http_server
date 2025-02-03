# Simple HTTP Server in Python

This repository contains a basic implementation of an HTTP server in Python using sockets.

## Features
- Handles basic HTTP requests.
- Supports GET requests to serve static files.
- Returns appropriate HTTP response codes (200, 404, 501).
- Implements a simple TCP server as the foundation for the HTTP server.

## Installation
No external dependencies are required. This script runs with the built-in Python standard library.

## Usage
1. Clone this repository:
   ```sh
   git clone <repository-url>
   cd <repository-name>
   ```
2. Run the server:
   ```sh
   python server.py
   ```
3. Open a web browser and go to:
   ```
   http://127.0.0.1:8888/<your-file>
   ```
   Replace `<your-file>` with the name of a file you want to serve.

## Code Structure
- **TCPServer**: A basic TCP server that listens for connections.
- **HTTPServer**: Inherits from `TCPServer` and implements basic HTTP request handling.
- **HTTPRequest**: Parses HTTP request data.
- **handle_GET**: Serves static files based on the request URI.

## Example
Place an `index.html` file in the same directory and access it via:
```
http://127.0.0.1:8888/index.html
```
