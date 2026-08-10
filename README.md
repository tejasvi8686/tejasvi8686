<p align="center">
    <img src="https://github.com/Kamasah-Dickson/Kamasah-Dickson/assets/86136379/f0ea5680-1c02-4cd6-b3e8-ec06e282ea5f"
        alt="pixel-night-banner">
</p>

<h1 align="center">Hello there, I'm Tejasvi Raj — React Native / Expo Developer 🔥⚡</h1>
<h3 align="center">I build mobile apps, and lately the infrastructure underneath them.
    I like shipping things end to end and finding out what actually breaks on a real device.</h3>

<p align="center">
    <img src="https://komarev.com/ghpvc/?username=tejasvi8686&label=Profile%20views&color=0e75b6&style=flat"
        alt="tejasvi8686" />
</p>

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

## 🛠 What I work with

| | |
|---|---|
| **Mobile** | React Native · Expo · TypeScript · EAS |
| **State** | Redux Toolkit · Redux Persist |
| **Backend** | Supabase · PostgreSQL · Edge Functions |
| **AI** | OpenAI Realtime API · GPT-4o · WebRTC · function calling |
| **Web** | React · Next.js · Tailwind |

<p align="center">
    <img src="https://skillicons.dev/icons?i=react,ts,js,redux,nodejs,nextjs,supabase,postgres,firebase,tailwind,sass,html,css,vite,express,git,github,figma&perline=9"
        alt="skills logos" />
</p>

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
    📫 <a href="mailto:tejasviraj8686@gmail.com">tejasviraj8686@gmail.com</a>
</p>
