# KidZo API

An Express.js API server for AI picture books for kids to publish on Amazon KDP (Kindle Direct Publishing).

## What We Did

This project was initialized as a basic Express.js server application with the following setup:

### Project Setup

1. **Created a Node.js project** with the following configuration:
   - Project name: `kidzo-api`
   - Version: `1.0.0`
   - Description: AI picture books for Kids to publish in KDP
   - Author: Rajesh Paramanandam
   - License: ISC

2. **Installed Dependencies**:
   - **express** (v5.1.0): A fast, unopinionated, minimalist web framework for Node.js
   - **nodemon** (v3.1.10, dev dependency): A tool that automatically restarts the server when file changes are detected during development

3. **Configured ES Modules**: Set `"type": "module"` in `package.json` to enable ES6 module syntax (import/export)

4. **Created the Express Server** (`app.js`):
   - Initialized an Express application
   - Configured the server to run on port 3000 (or environment variable PORT)
   - Created a basic GET endpoint at the root path (`/`) that returns "Hello World"
   - Added server startup logging to confirm the server is running

5. **Set up Git Ignore** (`.gitignore`):
   - Excluded `node_modules/` directory
   - Excluded environment files (`.env`)
   - Excluded system files (`.DS_Store`)
   - Excluded log files (`*.log`)
   - Excluded build artifacts (`dist/`, `build/`)
   - Excluded IDE configuration folders (`.vscode/`, `.idea/`)
   - Excluded test coverage folders (`coverage/`, `.nyc_output/`)

### Project Structure

```
KidZo/
├── app.js              # Main Express server application
├── package.json        # Project configuration and dependencies
├── package-lock.json   # Locked versions of installed dependencies
├── .gitignore          # Git ignore rules
└── README.md           # Project documentation (this file)
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Rajeshcse/KidZo.git
cd KidZo
```

2. Install dependencies:
```bash
npm install
```

## Usage

### Start the server in production mode:
```bash
node app.js
```

### Start the server in development mode (with auto-restart):
```bash
npm run dev
```

The server will start on port 3000 by default. You can access it at:
```
http://localhost:3000/
```

### Environment Variables

- `PORT`: Specify a custom port number (default: 3000)

Example:
```bash
PORT=8080 node app.js
```

## API Endpoints

### GET /
Returns a simple "Hello World" message.

**Response:**
```
Hello World
```

## Technologies Used

- **Node.js**: JavaScript runtime environment
- **Express.js v5**: Web application framework
- **ES6 Modules**: Modern JavaScript module system

## Development

The project uses nodemon for development to automatically restart the server when changes are detected.

To run in development mode:
```bash
npm run dev
```

## Future Development

This is the initial setup for the KidZo API. Future enhancements will include:
- Additional API endpoints for managing picture books
- Integration with AI services for content generation
- Database integration for storing book data
- Authentication and authorization
- Amazon KDP integration

## License

ISC
