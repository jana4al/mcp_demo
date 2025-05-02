# MCP Server

This project is a demonstration of MCP and showcases the integration of GitHub's Model Context Protocol (MCP) server. The primary goal of this project is to explore how MCP can be utilized to perform multiple actions using an intelligent agent.

## Features

- **GitHub MCP Integration**: Showcases how to use the GitHub MCP server for automating tasks and enhancing productivity.

## GitHub MCP Server

The GitHub MCP server is a powerful tool that allows developers to interact with GitHub repositories programmatically. By leveraging MCP, you can:

- Automate repository management tasks.
- Create and manage issues, pull requests, and branches.
- Perform code reviews and manage workflows.

### How to Use MCP in This Project

1. **Setup**: Ensure you have Docker installed and configured. The MCP server is run as a Docker container.
2. **Configuration**: Update the `settings.json` file to include your GitHub Personal Access Token (PAT) for authentication.
3. **Run MCP Server**: Use the following command to start the MCP server:
   ```bash
   docker run -i --rm -e GITHUB_PERSONAL_ACCESS_TOKEN=<your_token> ghcr.io/github/github-mcp-server
   ```
4. **Interact with MCP**: Use the integrated agent to perform actions like creating repositories, managing issues, and more.

## Project Structure

- **src/**: Contains the main application code.
  - **app/**: Includes components such as `home`, `user-create`, and `user-profile`.
  - **styles.css**: Global styles for the application.
  - **main.ts**: Entry point for the Angular application.
- **public/**: Static assets like `favicon.ico`.
- **server.ts**: Server-side logic for the application.

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/jana4al/mcp_demo.git
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```
4. Open the application in your browser at `http://localhost:4200`.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
