# S3 Bucket File Upload - Node Express App

A simple Node.js Express application with Multer for handling file uploads.

## Features

- Express.js server setup
- Single file upload endpoint
- Multiple files upload endpoint
- File storage with multer disk storage
- Error handling for file upload errors
- 10MB file size limit
- Simple HTML form for testing uploads

## Project Structure

```
s3-bucket-file-upload/
├── server.js           # Main Express server
├── package.json        # Project dependencies
├── .env               # Environment variables
├── .gitignore         # Git ignore file
└── uploads/           # Directory for uploaded files (created automatically)
```

## Installation

Install dependencies:

```bash
npm install
```

## Usage

### Development (with auto-reload)

```bash
npm run dev
```

### Production

```bash
npm start
```

The server will run on `http://localhost:3000`

## API Endpoints

### GET /
Returns an HTML form for testing file uploads.

### POST /upload
Single file upload endpoint.
- **Field name**: `file`
- **Returns**: File metadata (filename, size, path)

### POST /upload-multiple
Multiple files upload endpoint.
- **Field name**: `files`
- **Max files**: 5
- **Returns**: Array of file metadata

## Configuration

Edit `.env` to customize:
- `PORT`: Server port (default: 3000)
- `NODE_ENV`: Environment mode (development/production)

## Limits

- Maximum file size: 10MB
- Maximum files per upload: 5 (for /upload-multiple endpoint)

## Next Steps

To integrate with AWS S3:
1. Install AWS SDK: `npm install aws-sdk`
2. Configure AWS credentials
3. Modify the storage configuration to upload to S3 instead of local disk
