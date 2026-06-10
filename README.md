# Password-Analyzer-and-Vault
🔐 Client-side password analyzer, generator &amp; AES-256 encrypted vault — runs entirely in your browser. No server, no tracking, no account needed.

# 🔐 VaultKey — Password Security Suite

A fully client-side password security tool built with vanilla HTML, CSS, and JavaScript.
No server. No database. No account. Everything runs in your browser.

## ✨ Features

### 🔍 Password Analyzer
- Shannon entropy calculation
- Real-time strength score (0–100)
- Crack time estimate at 10 billion guesses/sec
- 10-point security checklist
- Common password breach detection (offline)
- Actionable improvement suggestions

### ⚡ Password Generator
- Cryptographically secure (WebCrypto API)
- Adjustable length: 8–64 characters
- Toggle uppercase, lowercase, numbers, symbols
- Automatically picks the strongest candidate
- One-click copy or save directly to vault

### 🔒 Encrypted Vault
- AES-256-GCM encryption
- PBKDF2-SHA256 key derivation (480,000 iterations — OWASP recommended)
- Random 32-byte salt + 12-byte IV generated fresh on every save
- Stored in browser localStorage only — never sent anywhere
- Search, copy, reveal, and delete entries
- Lock/unlock with master password

## 🛡 Security Model

| Property | Detail |
|---|---|
| Encryption | AES-256-GCM |
| Key derivation | PBKDF2-SHA256 |
| Iterations | 480,000 |
| Salt | 32 bytes, random per save |
| IV | 12 bytes, random per save |
| Storage | Browser localStorage only |
| Network requests | Zero |

## 🚀 Usage

clone and open locally:

```bash
git clone https://github.com/YOUR-USERNAME/password-vault.git
cd password-vault
open index.html
```
## ⚠️ Important Notes

- Your vault ID is generated once at creation. **Save it** — it cannot be recovered.
- Vault data lives in your browser's localStorage. Clearing browser data will delete it.
- This is a personal/educational tool. For production use, consider a dedicated
  password manager like Bitwarden or 1Password.

## 📄 License

MIT — free to use, modify, and distribute.
