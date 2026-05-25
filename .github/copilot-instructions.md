<!-- Use this file to provide workspace-specific custom instructions to Copilot. -->

# S3 Bucket File Upload - Node Express App

## Project Setup Complete

This is a Node.js Express application with Multer configured for file upload handling.

## Dependencies

- **express**: Web framework
- **multer**: File upload middleware
- **dotenv**: Environment variable management
- **nodemon**: Development auto-reload (dev only)

## Key Files

- `server.js`: Main Express server with Multer setup
- `package.json`: Project dependencies and scripts
- `.env`: Environment configuration
- `README.md`: Project documentation

## Available Commands

- `npm start`: Start production server
- `npm run dev`: Start development server with auto-reload
- `npm install`: Install dependencies

## Quick Start

1. Install dependencies: `npm install`
2. Run development server: `npm run dev`
3. Open http://localhost:3000 in your browser
4. Use the form to upload files

## Endpoints

- `GET /`: HTML form interface
- `POST /upload`: Single file upload
- `POST /upload-multiple`: Multiple files upload (max 5)
