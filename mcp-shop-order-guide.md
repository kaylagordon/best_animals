# MCP.shop Ordering Guide

## What's Available
**The MCP tee** - A minimalist t-shirt featuring "Context is Everything"
- **Price**: Free with the MCP Server
- **Sizes**: XS, S, M, L, XL, 2XL, 3XL
- **Description**: Minimalist, mysterious, and maybe a little meta. This sleek tee features MCP vibes and delivers subtle nerd cred with style.

## How to Order

### Option 1: Using Cursor with MCP Configuration (Recommended)
1. **Restart Cursor** to load the MCP configuration we just installed
2. **Open MCP Panel** in Cursor (look for MCP tools/servers in the interface)
3. **Connect to mcp.shop server** - it should appear in your available MCP servers
4. **Authenticate** - you'll be prompted to sign in via WorkOS AuthKit
5. **Use MCP tools** to browse and order the t-shirt

### Option 2: Direct Connection via Terminal
```bash
# Connect to the MCP server (requires browser for OAuth)
npx -y mcp-remote https://mcp.shop/mcp
```

When you run this command:
1. It will open your browser automatically
2. Sign in using the OAuth flow
3. Once authenticated, you can use MCP tools to place your order

## Current MCP Configuration
The MCP server is already configured in `/workspace/.cursor/mcp.json`:
```json
{
  "mcpServers": {
    "mcp.shop": {
      "command": "npx",
      "args": ["-y", "mcp-remote", "https://mcp.shop/mcp"]
    }
  }
}
```

## Next Steps
1. **Restart Cursor** to load the new MCP configuration
2. Look for the MCP.shop server in Cursor's MCP interface
3. Follow the authentication flow when prompted
4. Use the MCP tools to order your free "Context is Everything" t-shirt!

## Notes
- The t-shirt is free while supplies last
- You'll need to provide shipping information during the order process
- This is a demonstration of MCP (Model Context Protocol) in action
- The shop uses WorkOS AuthKit for secure authentication

Enjoy your MCP swag! 🎉