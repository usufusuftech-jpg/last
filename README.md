# ConnectChat — Emoji & GIF Real-Time Chat

A modern, highly responsive real-time chat web application built using React, Vite, and Tailwind CSS. The app features multiple chat rooms, and strictly enforces the **Emoji and GIF only** chat rule. It includes a built-in admin dashboard for system monitoring, user management, and message moderation.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=YOUR_GITHUB_REPO_URL_HERE)

> [!NOTE]
> **To enable Vercel One-Click Deploy:**
> Replace `YOUR_GITHUB_REPO_URL_HERE` in the button link above with your URL-encoded GitHub repository link (e.g., `https%3A%2F%2Fgithub.com%2Fusername%2Freponame`).

---

## Features

- **Emoji & GIF Only**: Enforces that users cannot send alphabetical letters. Only emojis, symbols, and curated/searched GIFs (powered by GIPHY API) are permitted.
- **In-Memory Store with LocalStorage Backup**: Fully client-side state architecture that synchronizes in real-time across multiple tabs using the `BroadcastChannel` API and persists across refreshes using `localStorage`.
- **Admin Control Panel**: Access an administrative dashboard to lock/unlock rooms, delete messages, ban/unban users, review logs, and monitor real-time sync performance.
- **Google OAuth Integration**: Log in securely using Google OAuth, or use a custom nickname.

---

## Deployment to Vercel

You can deploy ConnectChat instantly to Vercel:

1. Push this code repository to your GitHub account.
2. Click the **Deploy with Vercel** button above or import the repository manually in your Vercel Dashboard.
3. Configure the following environment variable (Optional):
   - `VITE_GOOGLE_CLIENT_ID`: Your Google OAuth Client ID if you want to support Google Sign-in on your custom domain.

---

## Admin Panel Access

- **Admin Path**: `/admin/login`
- **Authorized Admin Name**: `ABUUSUF5758`
- Regular users cannot bypass this login or register using this username from the homepage simple login interface.

---

## Tech Stack

- **Core**: React 19, TypeScript 5, Vite 7
- **Styling**: Tailwind CSS v4
- **Real-Time Sync**: Web BroadcastChannel API
- **Deployment**: Vercel
