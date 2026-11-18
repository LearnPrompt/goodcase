# goodcase

English | [中文](README.md)

[![Site](https://img.shields.io/badge/site-goodcase.ai-orange)](https://goodcase.ai/?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=badge)

**The open-source repo of [goodcase.ai](https://goodcase.ai/?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=tagline), an AI Prompt Case Collection.**

```bash
npx skills add LearnPrompt/goodcase --skill goodcase
```

That one line installs the goodcase query skill into your agent. It works with Claude Code, Codex, Cursor and anything else that reads SKILL.md. Then just ask in plain words:

- Show me a few viral AI video cases
- Find a prompt for glass-texture images
- Use the second one, but with my topic

The skill queries the public API of [goodcase.ai](https://goodcase.ai/?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=hero) and comes back with each case's source, creator, full prompt, stability score and cost band. No API key needed. If the API is unreachable, it falls back to the offline snapshot bundled with the skill and states the snapshot date in its answer.

To see cases next to their originals, go to [awesome-seedance](https://github.com/LearnPrompt/awesome-seedance?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=hero). To see where each skill stands today, go to [goodcase.ai/skills](https://goodcase.ai/skills?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=hero).

## What is in this repo

Two things.

The goodcase query skill above, in `skills/goodcase`.

And 112 skills extracted from popular cases on goodcase.ai, in `skills/generated`. Each skill is one directory with a SKILL.md and its example cases: 70 for video, 27 for image, 15 for web. To install a single one, put its slug into this command:

```bash
npx skills add LearnPrompt/goodcase --skill product-ad-shot-design
```

The slug is the directory name under `skills/generated`, and also the last segment of that skill's page URL on goodcase.ai.

## What Stable means

A skill marked Stable has had at least 3 of its example cases rerun, with 80% or more of them scoring 70 or higher.

Stable describes reruns of the examples' original prompts. New content you generate with the skill has not been tested.

As of 2026-11-19, 48 of the 112 extracted skills are Stable. That count covers the whole site: video, image and web. It changes as more reruns come in, and [goodcase.ai/skills](https://goodcase.ai/skills?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=stable) has the current state. Of the rest, some have fewer than 3 examples tested so far and are marked Awaiting tests, some were tested and fell below the bar, and some cannot be tested yet.

## Cases and side-by-side reruns

To look before you install, go to [LearnPrompt/awesome-seedance](https://github.com/LearnPrompt/awesome-seedance?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=cases). It is the Seedance case library: every case links its original post and carries the full prompt, and the reruns of the same prompt on another model sit alongside, including the ones that went badly.

That repo only covers video, so its skill counts are video-only and will not match the site-wide counts here.

## Run the site locally (optional)

This repo is also the open-source edition of the goodcase.ai site. Clone it and the same UI runs with a bundled set of real sample cases. No environment variables required.

```bash
git clone https://github.com/LearnPrompt/goodcase.git
cd goodcase
npm ci
npm run dev
```

Open http://localhost:3000 for the homepage, case library, case detail pages and creator pages. The data pipeline, review console and automated collection behind the live site are internal and not part of this repo. For the full dataset, call the live public API, also without a key:

```bash
curl -s "https://goodcase.ai/api/public/cases?take=3&locale=en"
```

Integration docs are at [goodcase.ai/connect](https://goodcase.ai/connect?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=site). To plug in your own data, copy `.env.example` to `.env.local` and fill in your own Supabase project URL and keys; for the schema, see the `/api/public` routes and the row types in `src/lib/cases.ts`. Deploy it like any Next.js app, on Vercel or any platform that runs Node.js.

## Acknowledgments

Every skill's examples come from creators who published their work in the open. Sources and credits are in each skill's `references/cases.md`. Thank you for sharing the prompts.

The install command runs on the [vercel-labs/skills](https://github.com/vercel-labs/skills) CLI.

Cases, stability scores and rerun data come from [goodcase.ai](https://goodcase.ai/?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=thanks).

## License


Code: MIT, see [LICENSE](./LICENSE). Copyright LearnPrompt.

The sample cases, prompts and media bundled with this repository are not covered by MIT: the images and videos under `public/media/goodcase/` (including its `avatars` folder), and the case text in `skills/generated/**/references/cases.md`, remain the property of their original creators and are included only for attribution and reproducibility.

Curation and metadata (categories, tags, scores, retest records, translations and editorial notes) are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); attribute GoodCase.ai.

If you are a creator and do not want your work listed here, or you spot a wrong attribution, leave a note at [goodcase.ai/connect#feedback](https://goodcase.ai/connect?utm_source=goodcase-repo&utm_medium=github&utm_campaign=readme-en&utm_content=license#feedback) (pick the "content" type and include the case link) or open an Issue on this repository. We will take the case down or correct it promptly.

See [CONTRIBUTING.md](./CONTRIBUTING.md) for how to contribute and [SECURITY.md](./SECURITY.md) for reporting vulnerabilities.
