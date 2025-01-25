# Server Mentis Boilerplate

This is a server boilerplate built with TypeScript and Fastify, suitable for a REST API project. It integrates various tools for efficient development, server-side functionality, and database operations.
Tools and Libraries Used

1. Fastify (@fastify/*)

    @fastify/cookie: Middleware for handling cookies in Fastify applications.
    @fastify/jwt: For handling JWT authentication, providing a simple way to issue and verify JSON Web Tokens.
    @fastify/rate-limit: A plugin to prevent abuse by limiting the rate of incoming requests to the server.
    fastify: A web framework highly focused on performance and low overhead for building APIs.

2. Database

    mysql2: A MySQL client for Node.js with promises support, allowing the server to interact with MySQL databases.
    drizzle-kit: A database migration and schema management tool that integrates seamlessly with Fastify.

3. Security

    bcrypt: Used for securely hashing passwords before storing them in the database.

4. Development Tools

    nodemon: A tool that monitors changes in the source files and automatically restarts the server. Great for development.
    tsx: A fast alternative to ts-node, used for running TypeScript files in development.
    typescript: The TypeScript compiler, enabling type safety and enhanced development experience.

5. Environment Management

    dotenv: Used to load environment variables from a .env file into the application. This helps configure sensitive information like API keys, DB credentials, etc.

## Available Scripts

    npm run serve: Starts the server with nodemon for automatic restarts on file changes.
    npm run build: Compiles TypeScript files into JavaScript using the TypeScript compiler (tsc).
    npm run start: Starts the server in production mode using Node.js, after building the project.
    npm run generate: Generates new migrations or database changes using drizzle-kit.
    npm run migrate: Pushes the migration changes to the database.

## Installation

    Clone the repository:

git clone https://github.com/your-username/server-mentis.git
cd server-mentis

Install the dependencies:

npm install

## Create a .env file to configure your environment variables.

Run the server in development mode:

    npm run serve

Project Structure

    src/: Contains the source code for the application.
    dist/: Contains the compiled JavaScript code after running npm run build.
    node_modules/: Contains all the installed dependencies.
    .env: The environment file for storing sensitive keys and configurations.
