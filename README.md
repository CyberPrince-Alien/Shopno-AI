<div align="center">
  <img src="assets/shopno_logo.png" alt="Shopno AI CLI Logo" width="132" />

  <h1>Shopno AI CLI</h1>

  <p>
    <strong>Premium managed AI coding agent platform for developers.</strong><br>
    Cloud models, local Ollama, subscriptions, secure gateway, and professional binary distribution.
  </p>

  <p>
    <img alt="Platform" src="https://img.shields.io/badge/platform-Windows%20%7C%20Mac%20%7C%20Linux-22d3ee?style=for-the-badge">
    <img alt="License" src="https://img.shields.io/badge/license-Proprietary-f59e0b?style=for-the-badge">
    <img alt="Owner" src="https://img.shields.io/badge/by-Sourov%20%2F%20Cyber%20Prince-8b5cf6?style=for-the-badge">
  </p>

  <p>
    <a href="https://surveymentor.org/shopno/register.php"><strong>Create Account</strong></a>
    |
    <a href="https://surveymentor.org/shopno/login.php"><strong>Login</strong></a>
    |
    <a href="https://surveymentor.org/shopno/support.php"><strong>Support</strong></a>
    |
    <a href="https://surveymentor.org/shopno/version_history.php"><strong>Version History</strong></a>
  </p>
</div>

---

## What Is Shopno AI CLI?

Shopno AI CLI is a professional AI command center for coding, project work, local automation, and managed cloud AI access.

Users do not need to bring provider API keys. They log in with a Shopno account, choose an enabled model, and work through the protected Shopno SaaS gateway. Admins keep control of subscriptions, quotas, model access, provider keys, downloads, announcements, support messages, maintenance mode, and payment approvals.

Shopno is built for a real software business: users get a polished CLI experience, while the owner keeps server-side control of cost, security, and product access.

---

## Command Center Preview

```text
READY  Shopno AI Coding Agent

+----------------------------------------------------------------+
| SHOPNO COMMAND CENTER                                          |
| Active Model: managed-model                                    |
+----------------------------------------------------------------+
| [1] START SHOPNO CLI (54 Features Enabled)                     |
|      Launch with active or last used model                     |
|                                                                |
| [2] CHOOSE MODEL FOR USE                                       |
|      Managed model catalog - no API key required               |
|                                                                |
| [3] OLLAMA LOCAL                                               |
|      Auto-install, model puller, local runtime                 |
|                                                                |
| [4] REMOTE CONTROL WITH WHATSAPP                               |
|      Pair WhatsApp and operate Shopno remotely                 |
|                                                                |
| [5] SAVED PROFILES                                             |
| [6] LOGOUT USER                                                |
| [7] EXIT COMMAND                                               |
+----------------------------------------------------------------+
```

---

## Core Features

| Area | What Shopno Provides |
| --- | --- |
| Managed Cloud Models | Users choose model names only; API keys and provider routing stay hidden. |
| Secure SaaS Gateway | Server-side auth, device binding, tier checks, quota enforcement, and fallback. |
| Local Ollama | Unlimited local model usage on the user's own machine. No SaaS quota counted. |
| Subscription System | Free, Pro, and Ultra access can be controlled from the admin panel. |
| Model Tier Control | Admin can enable/disable models and assign Free/Pro/Ultra access. |
| Key Vault | Provider keys and account tokens are stored server-side and protected. |
| Device Lock | One account, one active device, with logout-all-session recovery. |
| Download Portal | Windows, Mac, Linux links and version history are admin controlled. |
| Support Flow | Customers can send support messages and admins can reply. |
| Email System | SMTP settings, password reset, announcements, renewal/upgrade notices. |
| Maintenance Mode | Admin can pause the public app safely during updates. |
| Binary Release | Public users receive only the packaged executable and docs. |

---

## Cloud vs Local Usage

| Mode | Cost Source | Quota? | Best For |
| --- | --- | --- | --- |
| `CHOOSE MODEL FOR USE` | Shopno SaaS cloud gateway | Yes | Managed premium cloud models |
| `OLLAMA LOCAL` | User's own computer | No | Unlimited local/offline usage |
| WhatsApp Remote + Cloud Profile | Shopno SaaS cloud gateway | Yes | Remote control with managed models |
| WhatsApp Remote + Ollama Profile | User's own computer | No | Remote local automation |

Ollama Local is intentionally unlimited because it uses the user's own CPU/GPU/RAM and local model runtime.

---

## User Flow

1. Download the official release ZIP.
2. Run `Shopno-CLI.exe`.
3. Login with a Shopno account.
4. Select `CHOOSE MODEL FOR USE` for managed cloud models.
5. Select `OLLAMA LOCAL` for unlimited local models.
6. Start Shopno CLI and work from the command center.

If the same account is active on another device, Shopno shows a device conflict and lets the user clear all previous sessions before logging in again.

---

## Model Access

Shopno can expose premium model names while hiding all provider details.

Users may see model names such as:

- Llama 3.3 70B Versatile
- Step 3.7 Flash
- Step 3.5 Flash
- Nemotron 3 Super 120B
- Nemotron 3 Nano 30B
- GPT OSS 120B
- DeepSeek V4 Flash
- Qwen 3.5 397B
- Kimi K2.6
- Claude Haiku 4.5
- GPT-5 Mini
- Gemini 3.5 Flash
- Gemini 3.1 Pro
- Local Ollama Models

The exact list is controlled from the admin panel by plan, availability, and business cost.

---

## Plans

| Plan | Best For | Access |
| --- | --- | --- |
| Free | Trial users | Limited admin-selected access |
| Pro | Active developers | Managed cloud models with generous daily fair-use |
| Ultra | Heavy users and teams | Higher quota and premium model tier access |

Plan prices, quotas, expiration, payment approval, model access, and upgrade notices are controlled from the Shopno admin panel.

---

## Download Package

Recommended public release contents:

```text
Shopno-CLI.exe
README.md
LICENSE.md
USER_GUIDE.md
SECURITY.md
BINARY_DISTRIBUTION.md
assets/shopno_logo.png
```

Do not publish:

```text
src/
Admin Panel Shopno/
.shopno/
.env
build/
database exports with real credentials
provider keys
OAuth tokens
vault secrets
server config files
```

---

## Security Model

Shopno is designed so public users never receive your provider keys.

- Provider credentials stay on the server.
- New keys are encrypted before storage.
- CLI users receive only a device-bound Shopno session.
- Gateway requests validate auth token and active device.
- Model lists show model names only.
- Provider routing and fallback order are not exposed to users.
- Second-device login is blocked unless sessions are cleared.
- Public release packages must not contain source, cache, `.shopno`, `.env`, or secrets.

Read [`SECURITY.md`](SECURITY.md) before publishing a release.

---

## GitHub Pages Landing

A static GitHub Pages landing page is available in:

```text
github-pages/index.html
```

It can run from a GitHub Pages domain. Login, register, support, dashboard, download portal, and version history redirect to the live Shopno server:

```text
https://surveymentor.org/shopno
```

When the final domain is ready, update `SHOPNO_SERVER` inside `github-pages/index.html`.

---

## Documentation

| File | Purpose |
| --- | --- |
| [`USER_GUIDE.md`](USER_GUIDE.md) | User login, model selection, fair-use, and local mode |
| [`SECURITY.md`](SECURITY.md) | Release safety, key handling, and device binding |
| [`BINARY_DISTRIBUTION.md`](BINARY_DISTRIBUTION.md) | What to include in public ZIP releases |
| [`LICENSE.md`](LICENSE.md) | Proprietary commercial license |

---

## License

Shopno AI CLI is proprietary commercial software owned by **Sourov**, also known as **Cyber Prince**.

Users may run the official binary with an active Shopno account, subscription, trial, or written permission. Source code, admin panel code, server files, credentials, provider tokens, gateway internals, and private build assets must not be copied, modified, reverse engineered, republished, or redistributed.

See [`LICENSE.md`](LICENSE.md) for full terms.

---

## Owner

```text
Product: Shopno AI CLI
Owner: Sourov
Internet Name: Cyber Prince
Type: Proprietary SaaS + Binary AI Coding Agent
```

<div align="center">
  <strong>Shopno AI CLI</strong><br>
  Managed AI coding for serious developers.
</div>
