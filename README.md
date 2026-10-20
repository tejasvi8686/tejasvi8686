<p align="center">
  <img src="https://raw.githubusercontent.com/tejasvi8686/tejasvi8686/main/assets/banner.gif"
       alt="pixel waterfall banner" width="100%">
</p>

<h1 align="center">Hi, I'm Tejasvi Raj 👋</h1>
<h3 align="center">React Native developer. I build mobile apps end to end and ship them<br/>
to the App Store and Google Play — often with AI inside.</h3>

<p align="center">
  <a href="https://tejasviraj.in"><img src="https://img.shields.io/badge/Portfolio-tejasviraj.in-0e75b6?style=flat" alt="portfolio" /></a>
  <a href="https://www.linkedin.com/in/tejasviraj/"><img src="https://img.shields.io/badge/LinkedIn-tejasviraj-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="linkedin" /></a>
  <a href="mailto:tejasviraj8686@gmail.com"><img src="https://img.shields.io/badge/Email-tejasviraj8686-EA4335?style=flat&logo=gmail&logoColor=white" alt="email" /></a>
</p>

---

- 📱 **Mobile apps that go live.** React Native (Expo) apps on the **App Store and
  Google Play**, released through EAS Build + GitHub Actions pipelines to
  TestFlight and the Play Console.
- 📡 **Hardware and real-time.** A Bluetooth baby monitor app that reads live
  sensor data over BLE, and real-time AI voice over WebRTC.
- 🤖 **AI features, not just AI tools.** An open-source voice-AI library on npm,
  photo-based meal analysis, AI workout plans, and a 1st-place hackathon win.
- 🧩 **The whole product.** Next.js admin dashboards and Node.js / Supabase
  backends behind the apps.

📍 Noida, India · 2+ years building production mobile and web apps

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

**Let any React Native app talk to AI by voice — without shipping your OpenAI key.**

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

## 💼 What I've built at work

`Frontend Developer · Appeneure, Noida · Sep 2024 – Present` — client projects, so the code is private.

- **Bluetooth baby monitor** — React Native app, from MVP to the App Store and
  Google Play: live temperature, humidity and battery data over BLE
  (`react-native-ble-plx`), multi-device pairing, alerts and family sharing.
- **AI fitness app** — photo-based meal analysis, AI workout plans, macro and
  water tracking, sleep/recovery analytics, a real-time AI voice coach, and a
  Next.js admin dashboard.
- **Gym operations platform** — React Native app + Next.js web dashboard with
  OTP login, role-based access and real-time sync (Supabase, Strapi, React Query).
- **Subscriptions** — RevenueCat on iOS and Android for a coaching app, plus its
  coach–athlete features.
- **Release automation** — EAS Build + GitHub Actions pipelines to TestFlight
  and Google Play, replacing manual builds.

---

## 🚀 Side projects

### [AINewsly](https://github.com/tejasvi8686/AINewsly)
`React Native · Expo · Reanimated · Node.js · Express · MongoDB · Ollama (Gemma 3)`

Swipe-through news app that shows a title, a short summary and a "why it
matters" line for every story. The Expo app has a full-screen swipe feed, saved
and liked articles stored on the device, skeleton loading and haptics, plus a
Next.js landing page. Stories and summaries come from my Express + MongoDB API,
which uses Gemma 3 on Ollama to summarise RSS feeds and YouTube transcripts.

### [VolteX](https://github.com/tejasvi8686/Volex_Ecommerce) · [live ↗](https://volex-ecommerce.vercel.app) · in progress
`Next.js · React · Express · Prisma · PostgreSQL`

E-commerce platform for electronics, built with
[@Rajasva-Raj-CODE](https://github.com/Rajasva-Raj-CODE). I built the Express +
Prisma API and most of the React admin dashboard (catalogue, orders,
notifications), and we built the Next.js storefront together. The API is in
progress: the PostgreSQL schema, OTP + JWT login with refresh tokens,
role-based access, rate limiting and email team invites are done.

---

## 🏆 Achievements

🥇 **1st place out of 50+ teams — AI Feature Planner Hackathon (2025).** Built in
24 hours: a web app that suggests features for any product idea, on the OpenAI API.

---

## 🛠 Tech

| | |
|---|---|
| **Mobile** | React Native · Expo · Expo Router · EAS Build · RevenueCat · react-native-ble-plx · WebRTC |
| **Web** | React · Next.js (App Router) · Tailwind CSS · shadcn/ui · Redux Toolkit · React Query |
| **APIs & Data** | Node.js · Express · REST · GraphQL · Supabase · PostgreSQL · Prisma · MongoDB · Firebase · Strapi |
| **AI** | OpenAI API · OpenAI Realtime API · Ollama |
| **Languages** | TypeScript · JavaScript |
| **Tools** | Git · GitHub Actions · Vercel · Sentry · Postman · Figma · Claude Code · Codex |

<p align="center">
  <img src="https://skillicons.dev/icons?i=ts,js,react,nextjs,tailwind,redux,nodejs,express,graphql,supabase,postgres,prisma,firebase,vercel,git,github,figma,postman&perline=9"
       alt="skills logos" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/tejasvi8686/tejasvi8686/output/github-contribution-grid-snake-dark.svg"
       alt="contribution snake" />
</p>

---

<p align="center">
  📫 <a href="mailto:tejasviraj8686@gmail.com">tejasviraj8686@gmail.com</a> ·
  🌐 <a href="https://tejasviraj.in">tejasviraj.in</a> ·
  💼 <a href="https://www.linkedin.com/in/tejasviraj/">LinkedIn</a>
</p>
