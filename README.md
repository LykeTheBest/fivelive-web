<div align="center">

**🌐 Language / Dil:** **English** · [Türkçe](README.tr.md)

</div>

<div align="center">

# 🎮 FiveLive Roleplay — Web Platform

**A full-featured web platform built for a FiveM roleplay community — no framework, just clean code.**

[![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-8.x-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Status](https://img.shields.io/badge/Status-COMING%20SOON-orange?style=for-the-badge)]()

[💬 Discord](https://discord.gg/T6fH3KNDqC)

</div>

---

## 📖 About the Project

This repository contains the source code of a **full-featured web platform** built from scratch for a FiveM roleplay community.

It bundles everything a community needs under a single roof: a **landing site**, a **forum**, a **wiki (knowledge base)**, **application forms**, an **admin panel**, and **payment integration**.

The project is built **without any framework** using plain PHP + HTML + CSS + JavaScript. Its lightweight structure runs on any environment — including shared hosting — without extra configuration.

### Highlights

- ⚡ **Lightweight & Fast** — No heavy frameworks or libraries, only the code that's needed.
- 🔐 **Security-First** — CSRF, rate limiting, HMAC signing, XSS sanitizer, SSRF protection, session fixation protection.
- 🎨 **Multi-Theme** — Multiple themes managed dynamically from the admin panel.
- 🌍 **Bilingual** — Turkish / English (`/tr`, `/en`).
- 📱 **Fully Responsive** — Flawless rendering on phone, tablet, and desktop.
- 🧩 **Modular Architecture** — Router + template system, easy to extend.
- 💳 **Secure Payment Flow** — Webhook verification, automatic credit top-up.
- 🎮 **Discord OAuth** — Discord login with role-based authorization.

---

## ✨ Features

### 🌐 Public Site

| Section | Description |
|---------|-------------|
| **🏠 Home** | Landing page, featured highlights, live counter |
| **📰 News** | Dynamic news list, pagination, detail page |
| **📖 Wiki (Knowledge Base)** | Category + article structure, search, view counter |
| **🤝 Application Form** | AJAX-based form, Discord webhook notification |
| **🎁 Payment Page** | Package purchase flow |
| **📄 Legal Pages** | Privacy Policy, Terms of Service, Refund Policy |
| **🎬 Getting Started Guide** | Step-by-step guide, video, FAQ |
| **❓ FAQ** | Frequently asked questions and answers |
| **🔗 Dynamic Pages** | Custom pages created from the admin panel |
| **📱 Mobile Menu** | Fully functional hamburger menu on small screens |

### 👥 Forum System

| Feature | Description |
|---------|-------------|
| **Category Management** | Infinite-depth subcategories, sorting, section groups |
| **Topics** | Create, edit, delete, pin, lock, change status, move |
| **Replies** | Rich text editor, image upload, quoting, editing, deletion |
| **Bulk Actions** | Select topics → bulk move / status change / reply / lock / pin / delete |
| **Notifications** | Real-time notifications, mark as read, dropdown panel |
| **Trash Bin** | Restore deleted topics / replies / categories |
| **Category Permissions** | Role-based view, write, create topic, lock, move, etc. |
| **Global Permission Matrix** | Panel menu + action-based role permissions |

### 🛡️ Admin Panel

| Module | Description |
|--------|-------------|
| **Overview** | Total topics/users, quick actions, theme management |
| **Categories** | Create, edit, delete, reorder |
| **Penalties** | Ban / Mute, duration, IP-based ban |
| **User Management** | Advanced filtering, role assignment, session termination, info refresh |
| **Category Permissions** | Role × category permission matrix, permission copy |
| **Global Permission Matrix** | Role-based menu/action permissions |
| **Rankings** | Topic count race, weekly snapshot history |
| **Trash Bin** | Restore deleted items |
| **Theme Statistics** | Theme usage distribution, percentage breakdown |
| **Panel Access Roles** | Role-based panel access + per-user override |
| **Active Users** | Users active in the last 5 minutes |
| **Token Status** | Discord token expiration status |
| **Rate Limit Violations** | Active rate limit records |
| **Session Management** | Recent logins, session termination |
| **Upload Quota** | Per-user disk usage |
| **Action Logs** | Log code counters |
| **Anonymous Views** | IP-based anonymous view statistics |
| **IP Ban List** | IP-based ban penalties |
| **Settings Viewer** | View/edit all site settings |
| **Error Log** | Latest PHP error_log lines |
| **Security Logs** | Security event records |

### 💳 Payment Integration

| Feature | Description |
|---------|-------------|
| **Product Management** | Add, edit, delete, enable/disable products |
| **Secure Session** | Token generation with HMAC-SHA256 signing |
| **Webhook Verification** | HMAC signature check, status update |
| **Multiplier Campaign** | Automatic bonus multiplier |
| **Happy Hour** | Percentage-based bonus campaign |
| **Order Management** | Order list, mark as credited, delete |
| **Game Server Callback** | Credit notification to the game server |
| **Logging** | All requests/responses are logged in detail |

### 🎨 Theme System

| Theme | Folder |
|-------|--------|
| **Default** | `maintheme` |
| **Gold Obsidian** | `goldobsidian` |
| **Galaxy** | `galaxy` |
| **Winter** | `winter` |
| **Obsidian Premium** | `obsidianpremium` |

- **Selectable themes** in the picker are set from the admin panel.
- **Default theme** can be set.
- **Forced theme (Force)** — Enforce a theme for all visitors.
- **Per-user theme** — With a lock option.
- **Apply to all users** — Including anonymous visitors.

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology |
|-------|------------|
| **Backend** | PHP 8.x (plain, no framework) |
| **Database** | MySQL 8.x / MariaDB (PDO) |
| **Frontend** | HTML5, CSS3 (Flexbox, Grid, Custom Properties), Vanilla JS (ES6+) |
| **Authentication** | Discord OAuth2 |
| **Image Processing** | GD Library |
| **HTML Sanitizer** | HTMLPurifier (optional) |
| **Icons** | Inline SVG |
| **Fonts** | Google Fonts (Inter / Poppins / HCo Gotham) |

</div>

> The project requires no build tools, package managers, or frontend frameworks.

---

## 📁 Project Structure

```text
fivelive-site/
│
├── index.php                   # Main router + API dispatcher
├── router.php                  # URL router
├── dodopin_webhook.php         # Payment webhook handler
├── ingame_callback.php         # Game server credit callback
├── .env                        # Environment variables
│
├── templates/                  # HTML templates
│   ├── index2.html             # Home page
│   ├── news.html               # News
│   ├── article.html            # News detail
│   ├── category_detail.html    # Category detail
│   ├── topic_detail.html       # Topic detail
│   ├── new_topic.html          # New topic
│   ├── profile.html            # Profile
│   ├── wiki.html               # Wiki home
│   ├── wiki_category.html      # Wiki category
│   ├── wiki_article.html       # Wiki article
│   ├── partnership.html        # Application form
│   ├── donate.html             # Payment page
│   ├── howtoplay.html          # Getting started guide
│   ├── policy.html             # Privacy policy
│   ├── contract.html           # Terms of service
│   ├── chargeback.html         # Refund policy
│   ├── notifications.html      # Notifications
│   ├── maintenance.html        # Maintenance mode
│   ├── 404.html                # 404 page
│   ├── admin_login.html        # Admin login
│   └── admin_dashboard.html    # Admin panel
│
├── static/
│   ├── css/
│   │   ├── maintheme/
│   │   ├── goldobsidian/
│   │   ├── galaxy/
│   │   ├── winter/
│   │   └── obsidianpremium/
│   ├── js/
│   └── uploads/                # User-uploaded images
│
└── vendor/                     # Composer dependencies (optional)
```

---

## 🔒 Security

The platform is built with production in mind and follows a security-first approach:

| Category | Protection |
|----------|------------|
| **CSRF** | Token validation on every POST request |
| **XSS** | HTMLPurifier + built-in whitelist sanitizer |
| **SQL Injection** | All queries use PDO prepared statements |
| **Session Fixation** | `session_regenerate_id()` + UA hash + lifetime check |
| **Rate Limiting** | Multi-layered limits (session + IP + file) |
| **Brute Force** | Attempt limit + account lockout |
| **SSRF** | Host check on webhook URLs, private IP block |
| **Log Injection** | Control characters are stripped |
| **Path Traversal** | Static file paths constrained via `realpath()` |
| **DoS** | POST size limit, image size limit |
| **Clickjacking** | `X-Frame-Options: SAMEORIGIN` |
| **MIME Sniffing** | `X-Content-Type-Options: nosniff` |
| **Webhook Security** | Requests only sent to allowed domains |
| **HMAC** | Signature verification for payment and game callbacks |

---

## 🗺️ Roadmap

- [x] Home page + news
- [x] Forum system (topics/replies)
- [x] Wiki (categories + articles)
- [x] Admin panel
- [x] Discord OAuth
- [x] Multi-theme system
- [x] Payment integration
- [x] Bulk actions
- [x] Trash bin
- [x] Notification system
- [ ] REST API expansion
- [ ] PWA support
- [ ] Additional language support
- [ ] Real-time chat (WebSocket)

---

## 🤝 Contributing

This is a community project and contributions are always welcome!

- 🐛 **Found a bug?** — Open an issue or report it directly on Discord.
- 💡 **Have an idea?** — Open an issue and share your suggestion.
- 🛠️ **Want to contribute?** — For larger changes, please open an issue first to discuss.
- 🔐 **Found a security issue?** — Please do **not** open a public issue; contact us directly on Discord.

---

## 🙏 Acknowledgements

- **HTMLPurifier**, **Discord API** — For the infrastructure they provide.

---

## 📬 Contact

- **Discord:** [discord.gg/T6fH3KNDqC](https://discord.gg/T6fH3KNDqC)

---

<div align="center">

**FiveLive Roleplay Web Platform**

[![Discord](https://img.shields.io/badge/Discord-Join-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/T6fH3KNDqC)

<sub>This README is written to showcase the project itself. ❤️</sub>

</div>
