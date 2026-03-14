# conan-skill-news

> News headlines skill for [Conan AI](https://github.com/AmrLotfy/Conan-ai).

[![npm](https://img.shields.io/npm/v/conan-skill-news?color=crimson)](https://www.npmjs.com/package/conan-skill-news)
[![License: MIT](https://img.shields.io/badge/license-MIT-gold.svg)](LICENSE)

Top headlines by topic or category, powered by [NewsAPI](https://newsapi.org). Supports Arabic sources.

```
You: what's happening in tech today?
Conan: 📰 Top **tech** news

       1. **Meta releases Llama 4 with 10M token context window**
          TechCrunch · Mar 14
          Meta's latest open-source model sets a new record for context length...
          🔗 techcrunch.com/...

       2. **Apple announces M4 Ultra chip**
          The Verge · Mar 14
          🔗 theverge.com/...
```

---

## Install

```bash
conan skill install conan-skill-news
```

## Setup

Get a free API key at [newsapi.org](https://newsapi.org) (100 requests/day free), then:

```bash
conan config set newsApiKey YOUR_KEY
```

---

## Usage

```
"what's the latest tech news?"
"top world headlines"
"news about artificial intelligence"
"arabic news"
```

---

## Categories

| Category | Sources |
|---|---|
| `tech` | TechCrunch, The Verge, Wired, Ars Technica |
| `world` | BBC, Reuters, Al Jazeera, AP |
| `sports` | BBC Sport, ESPN, Fox Sports |
| `business` | Bloomberg, Financial Times, WSJ |
| `arabic` | Al Jazeera English, BBC Arabic |

---

## Parameters

| Parameter | Type | Required | Description |
|---|---|---|---|
| `query` | string | — | Topic or keywords to search |
| `category` | string | — | `tech` · `world` · `sports` · `business` · `arabic` |
| `count` | number | — | Number of headlines (1–5, default 5) |

---

## License

MIT · [Amr Lotfy](https://github.com/AmrLotfy)
