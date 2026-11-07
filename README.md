# abonur/homebrew-tap

Homebrew formulae for [abonur](https://github.com/abonur) projects.

## whatsapp-mcp

[WhatsApp archive and MCP server](https://github.com/abonur/whatsapp-mcp) for Claude and other AI assistants, on Mac and Linux.

```bash
brew install abonur/tap/whatsapp-mcp
whatsapp-mcp install-service
whatsapp-mcp link
```

`install-service` starts the background service; `link` asks for your phone number and gives you a code to type in WhatsApp (Linked devices > Link a device > Link with phone number instead).

After `brew upgrade whatsapp-mcp`, run `whatsapp-mcp install-service` again to restart the service on the new version.

## How the formula is updated

Each release of abonur/whatsapp-mcp attaches a generated `whatsapp-mcp.rb`. The `update` workflow here checks every hour for a new release and commits that file to `Formula/`. Run it by hand from the Actions tab to publish a release right away.
