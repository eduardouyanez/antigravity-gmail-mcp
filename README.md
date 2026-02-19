# Antigravity Gmail MCP

![Gmail MCP](https://img.shields.io/badge/MCP-Gmail-db4437?style=for-the-badge&logo=gmail)
![Antigravity Optimized](https://img.shields.io/badge/Antigravity-Optimized-blueviolet?style=for-the-badge)

[Español](#español) | [English](#english)

---

## Español

Servidor MCP de Gmail optimizado para su uso con el agente **Antigravity**. Esta versión incluye soporte documentado para **configuración multi-cuenta** (ej. Trabajo y Personal) y un flujo de autenticación simplificado.

### 🚀 Características
- **Lectura y Envío de Correos**: Integración completa con las APIs de Gmail.
- **Soporte Multi-cuenta**: Instrucciones para manejar múltiples tokens y llaves de OAuth.
- **Autenticación Automática**: Flujo de OAuth 2.0 integrado.

### 🛠️ Configuración Multi-cuenta
Para usar múltiples cuentas en Antigravity, debes definir los servidores por separado en tu `mcp_config.json`:

```json
"gmail-work": {
  "command": "node",
  "args": ["C:/ruta/a/antigravity-gmail-mcp/dist/index.js"],
  "env": {
    "GMAIL_OAUTH_PATH": "C:/ruta/a/credentials/gmail-work-keys.json",
    "GMAIL_CREDENTIALS_PATH": "C:/ruta/a/credentials/gmail-work-token.json"
  }
},
"gmail-personal": {
  "command": "node",
  "args": ["C:/ruta/a/antigravity-gmail-mcp/dist/index.js"],
  "env": {
    "GMAIL_OAUTH_PATH": "C:/ruta/a/credentials/gmail-personal-keys.json",
    "GMAIL_CREDENTIALS_PATH": "C:/ruta/a/credentials/gmail-personal-token.json"
  }
}
```

---

## English

Gmail MCP server optimized for the **Antigravity** agent. This version includes documented support for **multi-account setup** (e.g., Work and Personal) and a simplified authentication flow.

### 🚀 Features
- **Read and Send Emails**: Full integration with Gmail APIs.
- **Multi-account Support**: Instructions for managing multiple OAuth keys and tokens.
- **Auto Authentication**: Integrated OAuth 2.0 flow.

### 🛠️ Multi-account Setup
To use multiple accounts in Antigravity, define the servers separately in your `mcp_config.json` as shown in the Spanish section above.

### 📄 License
MIT License. Created for the Antigravity community.
