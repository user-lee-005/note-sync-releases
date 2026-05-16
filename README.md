# ObsidianSync

**Sync your Obsidian vaults with Git — right from your Android device.**

ObsidianSync is a lightweight Android app that bridges Obsidian and Git, giving you full version control over your notes without relying on Obsidian Sync or third-party plugins.

---

## ✨ Features

- 🔐 **PAT Authentication** — Login with GitHub or GitLab Personal Access Tokens
- 📂 **Repository Browser** — Browse and clone your repos with a searchable dropdown
- 📝 **Vault Linking** — Link any Obsidian vault to a cloned Git repository
- 🔄 **One-tap Sync** — Bidirectional sync between vault and repo (Pull / Push / Full Sync)
- 📁 **Configurable Storage** — Choose where repos are stored on your device
- ⚙️ **Commit Templates** — Customize commit messages with auto-timestamps
- 🧹 **Repo Management** — Clear repos, delete individual clones, manage storage

## 📱 Download

👉 **[Download latest APK from Releases](https://github.com/user-lee-005/obsidian-sync-releases/releases/latest)**

> Requires Android 8.0 (API 26) or higher.

## 🚀 Getting Started

1. **Install** the APK on your Android device
2. **Login** with your GitHub or GitLab Personal Access Token
3. **Clone** a repository from your account
4. **Select** your Obsidian vault folder
5. **Link** the vault to the repo
6. **Sync** with one tap!

### How to generate a PAT

**GitHub:**
1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. Generate a **classic** token with `repo` scope
3. Copy and paste into the app

**GitLab:**
1. Go to GitLab → Preferences → Access Tokens
2. Create a token with `read_api`, `read_repository`, `write_repository` scopes
3. Copy and paste into the app

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Language | Kotlin |
| UI | Jetpack Compose + Material 3 |
| Git Engine | JGit 6.8.0 |
| DI | Hilt |
| Auth Storage | EncryptedSharedPreferences |
| CI/CD | GitHub Actions |

## 📋 Permissions

| Permission | Why |
|---|---|
| `INTERNET` | Git operations (clone, pull, push) and API calls |
| `MANAGE_EXTERNAL_STORAGE` | Read/write Obsidian vault files on external storage |
| `READ/WRITE_EXTERNAL_STORAGE` | Legacy support for Android 10 and below |

## ⚠️ Notes

- **Uninstall old APK before updating** — each CI build generates a new debug signing key
- The app stores repos in internal storage by default (auto-cleaned on uninstall). Custom storage locations are preserved after uninstall.
- Grant "All Files Access" permission when prompted for vault sync to work properly

## 📄 License

This project is proprietary. APK downloads are provided for personal use.

---

**Built by [@user-lee-005](https://github.com/user-lee-005)**
