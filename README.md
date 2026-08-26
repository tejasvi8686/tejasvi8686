<p align="center">
    <img src="https://raw.githubusercontent.com/tejasvi8686/tejasvi8686/main/assets/banner.gif"
        alt="pixel waterfall banner" width="100%">
</p>

<h1 align="center">Hi, I'm Tejasvi Raj — Frontend Developer 🔥⚡</h1>
<h3 align="center">I build mobile apps, and lately the infrastructure underneath them.<br/>
    I like shipping end to end and finding out what actually breaks on a real device.</h3>

<p align="center">
    <a href="https://tejasviraj.in"><img src="https://img.shields.io/badge/Portfolio-tejasviraj.in-0e75b6?style=flat" alt="portfolio" /></a>
    <a href="https://www.linkedin.com/in/tejasviraj/"><img src="https://img.shields.io/badge/LinkedIn-tejasviraj-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="linkedin" /></a>
    <a href="mailto:tejasviraj8686@gmail.com"><img src="https://img.shields.io/badge/Email-tejasviraj8686-EA4335?style=flat&logo=gmail&logoColor=white" alt="email" /></a>
    <a href="https://cal.com/tejasviraj"><img src="https://img.shields.io/badge/Book%20a%20call-cal.com-000000?style=flat" alt="cal.com" /></a>
    <img src="https://komarev.com/ghpvc/?username=tejasvi8686&label=Profile%20views&color=0e75b6&style=flat" alt="profile views" />
</p>

---

Frontend developer with **2+ years** building and shipping production web and
mobile products with **React, Next.js and React Native (Expo)**. The work has
spanned **BLE hardware integration**, **in-app subscriptions** and **real-time
data sync** — with apps released to the App Store and Play Store, and an
open-source React Native package published to npm.

📍 Noida, India

---

## 📦 react-native-realtime-voice

<p align="center">
    <a href="https://www.npmjs.com/package/react-native-realtime-voice">
        <img src="https://img.shields.io/npm/v/react-native-realtime-voice?style=flat&color=0e75b6&label=npm" alt="npm version" />
    </a>
    <a href="https://www.npmjs.com/package/react-native-realtime-voice">
        <img src="https://img.shields.io/npm/dm/react-native-realtime-voice?style=flat&color=0e75b6" alt="downloads" />
    </a>
    <img src="https://img.shields.io/badge/dependencies-0-brightgreen?style=flat" alt="zero dependencies" />
    <img src="https://img.shields.io/npm/l/react-native-realtime-voice?style=flat&color=blue" alt="license" />
</p>

Voice-to-voice AI agents for React Native / Expo, on OpenAI's Realtime API over
WebRTC. I built the voice layer inside a fitness app, realised the hard parts
weren't app-specific, and pulled them out into a library.

```ts
const voice = useRealtimeVoice({
  auth: { getToken: () => fetch("/api/token").then(r => r.json()) },
  instructions: () => `You are a coach. User: ${user.name}.`,
  tools: [logWaterTool],
});
```

What I cared about while building it:

- **Your OpenAI key never ships.** Ephemeral tokens are the default path; a raw
  key is a dev-only escape hatch that warns loudly. The backend owns the model
  and voice, the app owns the prompt and tools — so product changes don't need a
  backend deploy.
- **Tools carry their own handler.** No schema in one file and a `switch` in
  another. Pass a zod schema, get typed arguments; zod stays optional.
- **Zero runtime dependencies.** Headless core, with the UI kit as a separate
  import built on React Native's own primitives.

Reconnect with backoff, barge-in, tool timeouts and cancellation, duplicate-call
dedupe and typed error codes are handled too. Released through GitHub Actions
with npm trusted publishing (OIDC), so there is no long-lived token to leak.

[npm](https://www.npmjs.com/package/react-native-realtime-voice) ·
[source](https://github.com/tejasvi8686/react-native-realtime-voice)

---

## 💼 Experience

### Frontend Developer · Appeneure — Noida, India
`Sep 2024 – Present`

- Built both the **Next.js web app** and the **React Native (Expo) mobile app**
  for a gym operations platform — cleaning task workflows, equipment monitoring,
  incident reporting and staff workload dashboards, with OTP authentication,
  role-based routing and real-time sync via Supabase, Strapi and React Query
- Delivered the MVP and production release of a **Bluetooth-connected baby
  monitor app**: `react-native-ble-plx` for live temperature, humidity and
  battery telemetry, plus TOG clothing recommendations, alerts, multi-device
  pairing and family sharing on Supabase
- Building the mobile app and Next.js admin panel for a **Norwegian fitness
  client** — RevenueCat for in-app subscription management, and the
  coach–athlete data flows
- Built an **AI fitness app** with generated workout plans, macro and water
  tracking, camera-based meal logging and sleep/recovery analytics, plus its
  Next.js admin dashboard
- Set up **EAS Build and GitHub Actions** pipelines for automated TestFlight and
  Play Store releases, replacing a manual build process; web deployed via Vercel

### Frontend Developer Intern · Own Technologies — New Delhi, India
`Nov 2023 – Feb 2024`

- Built a learning platform from scratch in React.js, Redux and SCSS, including
  note purchase and download flows for students and an application flow for teachers
- Created a reusable component library and responsive SCSS layouts, and added API
  error handling with user-facing fallback states

---

## 🚀 Projects

### [VolteX](https://github.com/tejasvi8686/Volex_Ecommerce) · [live ↗](https://volex-ecommerce.vercel.app)
`Next.js · Node.js · Express · PostgreSQL · Prisma`

Full-stack e-commerce platform — a Next.js storefront over an Express REST API
and a Prisma/PostgreSQL data layer, with role-based access control middleware and
an admin panel covering catalogue, orders and notification management.

---

## 🏆 Achievements

🥇 **1st Place — AI Feature Planner Hackathon (2025)** — first among 50+ teams
for a web app that generates feature suggestions for any product idea, built end
to end in 24 hours on the OpenAI API.

---

## 🛠 Tech

| | |
|---|---|
| **Languages** | TypeScript · JavaScript |
| **Web** | React · Next.js (App Router) · Tailwind CSS · shadcn/ui · Redux Toolkit · React Query |
| **Mobile** | React Native · Expo · Expo Router · EAS Build · RevenueCat · react-native-ble-plx |
| **APIs & Data** | GraphQL · REST · Supabase · PostgreSQL · Prisma · Firebase · Strapi · Node.js · Express |
| **Tools** | Git · GitHub Actions · Vercel · Postman · Figma · Claude Code · Codex |

<p align="center">
    <img src="https://skillicons.dev/icons?i=ts,js,react,nextjs,tailwind,redux,nodejs,express,graphql,supabase,postgres,prisma,firebase,vercel,git,github,figma,postman&perline=9"
        alt="skills logos" />
</p>

---

## 🎓 Education

**B.Tech, Computer Science** — Dr. K. N. Modi Institute of Engineering &
Technology · Graduated Sep 2024

---

## 📊 Stats

<p align="center">
    <img src="https://github-readme-stats.vercel.app/api?username=tejasvi8686&show_icons=true&theme=tokyonight&hide_border=true" />
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=tejasvi8686&layout=compact&langs_count=10&theme=tokyonight&hide_border=true&count-private=true" />
</p>

<p align="center">
    <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=tejasvi8686&theme=tokyonight" />
</p>

<p align="center">
    <img src="https://github-readme-streak-stats.herokuapp.com?user=tejasvi8686&theme=tokyonight&hide_border=true" />
    <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=tejasvi8686&theme=tokyonight" />
</p>

<p align="center">
    <img src="https://raw.githubusercontent.com/tejasvi8686/tejasvi8686/output/github-contribution-grid-snake-dark.svg"
        alt="contribution snake" />
</p>

---

<p align="center">
    📫 <a href="mailto:tejasviraj8686@gmail.com">tejasviraj8686@gmail.com</a> ·
    🌐 <a href="https://tejasviraj.in">tejasviraj.in</a> ·
    📅 <a href="https://cal.com/tejasviraj">Book a call</a>
</p>
