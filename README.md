<img src="https://askmywa.com/assets/icon-192.png" width="72" height="72" alt="askmywa logo">

# Ruwad-io/homebrew-tap

Homebrew formulae for [RUWAD](https://ruwad.io) projects.

## askmywa (WhatsApp MCP)

[WhatsApp archive and MCP server](https://github.com/Ruwad-io/askmywa) for Claude and other AI assistants, on Mac and Linux.

```bash
brew install ruwad-io/tap/askmywa
askmywa install-service
askmywa link
```

`install-service` starts the background service; `link` asks for your phone number and gives you a code to type in WhatsApp (Linked devices > Link a device > Link with phone number instead).

After `brew upgrade askmywa`, run `askmywa install-service` again to restart the service on the new version.

## How the formula is updated

Each release of Ruwad-io/askmywa attaches a generated `askmywa.rb`. The `update` workflow here checks every hour for a new release and commits that file to `Formula/`. Run it by hand from the Actions tab to publish a release right away.
