# ✨ Spelling Star

A fun, kid-friendly spelling practice app with British English pronunciation. Built as a single HTML file — no build tools, no dependencies, no backend.

**Live app:** https://execbitlz.github.io/spelling-practice/

## Features

- **British English audio** — uses the Web Speech API (`en-GB`) for pronunciation, with normal and slow speed options
- **Teacher Mode** — parents/teachers add words and lock the app into practice-only mode; words persist across sessions via `localStorage`
- **Shareable links** — generate a URL like `https://execbitlz.github.io/spelling-practice/#words=apple,banana,orange` that opens directly into practice mode
- **Mobile-friendly** — responsive layout, 44px touch targets, iOS safe area support, native share sheet via Web Share API
- **Kid-friendly UI** — colourful gradients, floating star animations, confetti on correct answers, encouraging feedback messages
- **3 chances per word** — wrong answers get encouraging feedback and a retry; the correct spelling is revealed after the third attempt
- **Hints** — shows first letter, last letter, and word length
- **Results screen** — score breakdown with option to retry only the mistakes
- **Secret unlock** — tap the title 5 times to return to the setup screen from practice mode

## How to Use

### As a parent/teacher

1. Open the app and add words (type individually or comma-separated)
2. Toggle **Teacher Mode** ON to save words to the device
3. Click **Start Practice** and hand the device to your child
4. Next time the page loads, it skips straight to practice

### Sharing via link

1. Add your words on the setup screen
2. Click **📤 Share Practice Link** — on mobile this opens the native share sheet (WhatsApp, Messages, etc.), on desktop it copies the URL
3. The recipient opens the link and goes straight to practice — no setup needed

## Tech Stack

- Single `index.html` file (HTML + CSS + vanilla JS)
- [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesis) for text-to-speech
- [Web Share API](https://developer.mozilla.org/en-US/docs/Web/API/Navigator/share) for mobile sharing
- `localStorage` for Teacher Mode persistence
- URL hash fragment for shareable word lists
- Hosted on GitHub Pages

## Local Development

Just open `index.html` in a browser. No server required.

```
open index.html
```

## License

MIT
