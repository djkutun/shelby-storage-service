
# Shelby Storage Service

A production-style Node.js backend integrating Shelby Protocol SDK for decentralized file storage.

## Features

- Upload files to Shelby decentralized storage
- Retrieve file metadata
- Download stored files
- SHA256 hash verification
- REST API architecture

## Install

```bash
git clone https://github.com/YOUR_USERNAME/shelby-storage-service.git
cd shelby-storage-service
npm install
```

## Setup

Create `.env` file:

```
PORT=3000
SHELBY_API_KEY=your_api_key_here
```

## Run

Development

```
npm run dev
```

Production

```
npm run build
npm start
```

## API

Upload file

```
POST /upload
```
Form-data:
file: <binary>

Download file

```
GET /download/:cid
```

Get metadata

```
GET /file/:cid
```

## Tech

- Node.js
- TypeScript
- Express
- Shelby Protocol SDK
