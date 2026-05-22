# TidyApp

TidyApp is a Windows desktop productivity app for organizing multiple communication workspaces in one local-first environment. It helps you keep work, clients, support, teams, and personal accounts separated without living inside a pile of browser profiles, tabs, and windows.

Current version: `v2.1.0`

## What It Does

- Adds multiple isolated accounts for supported communication platforms.
- Keeps each account in its own local Electron session and storage partition.
- Switches quickly between workspaces from a compact desktop sidebar.
- Supports Command Palette switching with `Ctrl+K`.
- Organizes accounts into groups such as work, personal, clients, and support.
- Supports WhatsApp, Telegram, Instagram, Facebook, and Discord workspaces.
- Keeps account metadata, settings, and license state local to the device.
- Provides a browser fallback preview page when the renderer is opened outside Electron.

## Pro Features

TidyApp Pro is a one-time paid upgrade for larger workspaces and advanced controls.

- Unlimited accounts
- Split View for using two accounts side by side
- Command Palette for fast account and action switching
- Quiet Hours and Priority Notifications
- Workspace groups
- RAM Saver for sleeping inactive workspaces
- App Lock
- Quick Switch Shortcuts
- Auto Restore
- Custom account names, icons, and colors
- Focus Mode
- Advanced themes
- Local backup and import

## Free Plan

The Free plan is designed for small personal workspaces.

- Up to 4 communication accounts
- Basic account switching
- Basic workspace management
- Basic notifications
- Dark mode

## Privacy

TidyApp is privacy-focused by design. It runs locally on the user's device and does not provide unauthorized access, automation, scraping, or circumvention of third-party platform restrictions.

TidyApp does not upload chats, passwords, or browser sessions. Workspace metadata such as names, groups, theme settings, and license state is stored locally.

## Website And Downloads

Official website: [tidyapp.site](https://tidyapp.site)

The Windows installer is published through GitHub Releases and linked from the official website.
The current production website is deployed on Vercel.

## Development

TidyApp is built with Electron, React, TypeScript, and Vite.

```bash
npm install
npm run dev
```

Build the desktop app renderer and Electron bundles:

```bash
npm run build
```

Build a full Windows installer release:

```bash
npm run dist
```

`npm run dist` cleans the `dist` folder before creating a fresh release. If you need to preserve an older upload folder, build with `electron-builder` into a separate output directory and copy only the new release files into `dist/upload/vX.Y.Z`.

Build the website:

```bash
npm run website:build
```

## Release Version

The packaged desktop app version comes from the root `package.json`. For the `v2.1.0` release, the app package version is set to `2.1.0`, so generated builds show and package as version `2.1.0`.

The v2.1.0 upload folder is expected at:

```text
dist/upload/v2.1.0
```

Expected release files:

- `TidyApp-2.1.0-Installer.exe`
- `TidyApp-2.1.0-Installer.exe.blockmap`
- `latest.yml`

## Contact

For product updates, support, or partnership inquiries, use the official TidyApp website.
