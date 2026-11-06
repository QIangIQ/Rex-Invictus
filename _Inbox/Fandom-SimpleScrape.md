---
title: Fandom-SimpleScrape
type: tool
status: active
tags: [tool, scraping, fandom, python, backup]
date: 2026-11-02
source: C:\Users\qiang\Documents\Fandom-SimpleScrape\main.py; scrape run of 2026-11-02
---

# Fandom-SimpleScrape

Source: `C:\Users\qiang\Documents\Fandom-SimpleScrape\main.py` (github.com/norsizu/Fandom-SimpleScrape, commit ee06592) and the scrape run on 2026-11-02.

Third-party Python tool that saves a whole Fandom wiki as plain-text Markdown files, one per article. Gradio web GUI (`python main.py`). Dependencies: beautifulsoup4 4.12.3, gradio 4.44.0, requests 2.32.3.

## Location
- Installed by accident into `C:\Windows\System32\Fandom-SimpleScrape`, moved to `C:\Users\qiang\Documents\Fandom-SimpleScrape` (move confirmed; nothing left in System32).
- Local edit to `main.py`: the "next page" detection also matches English "next page", not only Chinese 下一页. Benign.

## Safety review (2026-11-02)
- Network: only HTTP GETs to the wiki URL typed in; Gradio analytics turned off (`analytics_enabled=False`); GUI served locally.
- Files: writes only `.md` files into the chosen save folder; `clean_filename` strips `\ / * ? : " < > |`, so no path escape.
- No subprocess, eval, downloads or credential access. Verdict: safe.

## Lessons
- **Fails on current Fandom:** the HTML pages (`/wiki/Special:AllPages`, article pages) sit behind a Cloudflare "Just a moment..." challenge and return 403 to plain requests.
- **Bug:** `base_url = fandom_url.rsplit('/', 1)[0]` gives `https:/` for a root wiki URL like `https://x.fandom.com`; it only works for language sub-paths such as `https://x.fandom.com/zh`.
- **What worked:** the wiki's official MediaWiki API (`https://<wiki>.fandom.com/api.php`, `list=allpages` + `action=parse`) is open and returns 200. A small runner fed the API's HTML into the tool's own `html_to_markdown` converter.
- Converter quirk: some articles show a paragraph twice and stub/template banners are kept as text.

## Runs
- SOFTINF: https://secretsnicholasflamel.fandom.com, 201 articles (main namespace, no redirects), 0 failures, 1.3 MB, into `Rex Invictus\SOFTINF`; since filed under `REX INVICTUS\Flamel Series`.
- MTWABV: https://mtwabv.fandom.com, 896 articles (main namespace, no redirects), 0 failures, 42 MB, into `Rex Invictus\MTWABV`. Same API route. Subpages such as `Victor Elderblood/Chronology` become `Victor ElderbloodChronology.md`, because the converter strips the slash. Spoiler banners and page tab menus are kept as text.

Related: [[Rex Invictus]]
