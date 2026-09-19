# 📚 Daily Study Log Generator

A tiny, single-file web app that turns a few taps into a ready-to-post daily study log — built for a study tracking community where everyone posts progress in the same format every day.

No sign-up, no backend, no install. Open it in a browser, fill it in, copy the result.

## ✨ Features

- **Subject picker** — Physics ⚡, Chemistry 🧪, Math 📐, Biology 🧬, English 📖, each with its own emoji
- **Chapter, classes, question bank, and exam status** — filled in with taps and a text field, no typing formatting by hand
- **Live Dhaka-time date & timestamp** — always correct regardless of the visitor's own device timezone
- **One-tap "Generate"** — builds the exact post text from your inputs
- **One-tap "Copy to clipboard"** — no manual selecting/copying
- Fully responsive — works just as well on a phone as a laptop
- Nothing is saved or sent anywhere — everything runs locally in the browser

## 🖥️ Live demo

[*Website*](https://hamimtalukder.github.io/Study-log-generator/)

## 🛠️ Built with

- **HTML5** — structure
- **CSS3** (plain, no framework) — layout, gradients, animations
- **JavaScript** (vanilla, no libraries) — interactivity, live clock, text generation, clipboard copy
- **Google Fonts** — [Unbounded](https://fonts.google.com/specimen/Unbounded) (headings/UI) & [Space Mono](https://fonts.google.com/specimen/Space+Mono) (the generated log text)

Everything lives in a single `index.html` file — no build step, no dependencies to install.

## 📋 How it works

1. Pick your subject
2. Type the chapter name, then mark it Completed / Not completed
3. Set how many classes you attended, then mark the status
4. Choose Partial/Full chapter for the question bank, then mark the status
5. Mark whether the exam was given
6. Tap **✨ Generate my log**
7. Tap **📋 Copy to clipboard** and paste it straight into the group


## 📁 Project structure

```
study-log-generator/
├── index.html   # everything — HTML, CSS & JS in one file
└── README.md
```

## ✏️ Customizing

- **Subjects / emojis** — edit the `.chip` buttons in the HTML and the `SUBJECTS`-style data attributes (`data-subject`, `data-emoji`)
- **Colors** — all colors are CSS variables at the top of the `<style>` block (`--lime`, `--pink`, `--bg-a`, etc.)
- **Post format** — the exact text is built in the `buildText()` function in the `<script>` block

## 🙌 Credits

Made by **Hamim Talukder S0T0n** for the daily study log community, so nobody has to hunt for the right emoji or retype the format by hand.
