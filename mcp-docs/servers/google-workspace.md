# Google Workspace MCP Server

Instructions for setting up the Google Workspace MCP server (Docs, Sheets, Calendar, etc.).

## Prerequisites

1. **Google Cloud Project**: Create a project in the [Google Cloud Console](https://console.cloud.google.com/).
2. **Enable APIs**: Enable Google Docs API, Google Drive API, etc.
3. **OAuth Credentials**: Create "Desktop app" OAuth credentials and download the `credentials.json` file.

## Configuration

1. Place `credentials.json` in the server directory.
2. Run the server and complete the OAuth flow in your browser.

```bash
npx -y @modelcontextprotocol/server-google-workspace
```
