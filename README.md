# xxxhbt — What's Your Ideal Type?

A playful, Korean-language questionnaire that turns **talking about your ideal type** into a short interactive experience.

[Try the quiz](https://xxxhbt.vercel.app)

## Why I built it

Describing a preference from scratch can be surprisingly difficult. This project gives that conversation a little structure: one question at a time, a few different ways to answer, and a summary at the end.

The visual direction uses pink accents, rounded cards, expressive Korean typography, and small animations to keep the experience light and personal.

## The experience

The quiz contains **15 questions** covering appearance, dating preferences, communication, hobbies, conflict resolution, and dealbreakers. It ends with an optional one-line description.

Four input patterns support different kinds of answers:

- **Single choice** for a preferred option.
- **Multiple choice** for a collection of preferences.
- **A range slider** for preferred height, with a live value display.
- **Free text** for a description in your own words.

Previous/next navigation keeps answers available while moving between questions. A progress indicator tracks the flow. The result groups the responses into basic preferences, relationship style, and dealbreakers, followed by the written description. A Canvas confetti animation marks completion, and a restart button clears the answers.

## Built with

**HTML · CSS · JavaScript · Canvas 2D API**

The application is contained in a single `index.html`, with no framework, package installation, or build step. A question configuration array drives the different input layouts, and JavaScript updates the current card and result view.

Google Fonts supplies **Moirai One** and **Bagel Fat One**.

## Run locally

Open `index.html` in a modern browser, or use a local static server:

```sh
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Answer handling

Answers stay in JavaScript memory for the current page session. The implementation does not save them to browser storage or submit them to a server; refreshing the page resets the quiz. Google Fonts is loaded separately for typography.

The result is a summary of the choices made, rather than a calculated personality score or a generated match.

## What this project explores

How can a small interface make self-expression easier? The project uses a conversational sequence and varied inputs to help someone turn vague preferences into something they can read, reflect on, and talk about.
