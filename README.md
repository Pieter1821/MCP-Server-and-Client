# MCP Server and Client

A Node.js project implementing a Model Context Protocol (MCP) server and client for resource and tool management, user data handling, and prompt-based operations.

## Features
- MCP server with resource, tool, and prompt registration
- User data management (CRUD operations)
- Client for interacting with the MCP server
- TypeScript and JavaScript support

## Prerequisites
- [Node.js](https://nodejs.org/) (v18+ recommended)
- [npm](https://www.npmjs.com/)

## Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```

   The following packages will be installed:
   - @inquirer/prompts
   - @modelcontextprotocol/sdk
   - dotenv
   - zod
   - @modelcontextprotocol/inspector (dev)
   - @types/node (dev)
   - ts-node (dev)
   - tsx (dev)
   - typescript (dev)
3. **Build the server:**
   ```bash
   npm run server:build
   ```

## Usage
### Run the server (development)
```bash
npm run server:dev
```

### Run the client
- The client connects to the server using the built files.
- You can run the client code in `src/client/client.ts` (TypeScript) or use the built JS in `build/client/client.js`.

## Scripts
- `npm run server:build` — Compile TypeScript to JavaScript
- `npm run server:build:watch` — Watch and compile on changes
- `npm run server:dev` — Run the server in development mode
- `npm run server:inspect` — Run the server with MCP Inspector

## Project Structure
```
├── build/
│   ├── server.js
│   └── client/
│       └── client.js
│   └── data/
│       └── users.json
├── src/
│   ├── server.ts
│   └── client/
│       └── client.ts
│   └── data/
│       └── users.json
├── package.json
├── tsconfig.json
```

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Create a new Pull Request

## License
This project is licensed under the ISC License.

## Contact
For questions or support, open an issue on GitHub.
