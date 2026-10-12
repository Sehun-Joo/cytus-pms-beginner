# Cytus × PMS — Beginner / Normal

**[Open or import the table](https://sehun-joo.github.io/cytus-pms-beginner/)**

24 charts across 12 songs from Cytus and Cytus II, using the normal PMS table's Lv1–45 and 45+ range. Three charts are Lv20 or below: Fading Star 12, conflict 13 and B.B.K.K.B.K.K. 15. No confirmed five-button matches were found. The upper levels are challenging; start with the Lv1–20 browser filter.

Add the public page URL to your player's difficulty-table settings. Browser filters do not change imports. Only chart metadata is hosted; use the credited package/chart links to obtain playable files.

## Selection and sources

Checked 2026-10-12 against the [Japanese Cytus chapter list](https://wikiwiki.jp/cytus/曲名リスト), [Japanese Cytus II song list](https://wikiwiki.jp/cytus-2/楽曲一覧), and [Japanese BMS crossover list](https://w.atwiki.jp/laser_bm/pages/86.html). Paid packs and collaborations were considered. Game presence is based on these community references, not an official complete catalog or a guarantee of current regional availability.

Chart ratings, hashes and credits are preserved from the 7,291-row [normal PMS snapshot](https://pmsdatabase.github.io/pmsdatabase/pmsdatabase_score.json). `catalog.json` records reviewed hashes and game evidence; builds never automatically include substring matches. `source-normal.json` retains the reference snapshot, including its chart metadata enrichment.

Included songs: Acquire, B.B.K.K.B.K.K., Black Lair, conflict, Fading Star, Halcyon, L, Laplace, Oriens, Parousia, R.I.P., and バステット.

Version differences are explicit: **B.B.K.K.B.K.K. uses the original 2013 BMS**, whereas [Cytus II contains the 2023 remake](https://wikiwiki.jp/cytus-2/B.B.K.K.B.K.K.%20%282023%20Remake%29). **バステット uses the original BOFXVI BMS**, whereas [Cytus II has a named edit](https://wikiwiki.jp/cytus-2/バステット%20%28Cytus%20II%20Edit%29). These are familiar-song inclusions, not assertions of identical audio.

Title collisions were rejected: L9 (paraoka versus Ice), Qualia (Junk versus KIVΛ), Leviathan (cittan* versus NeLiME), Realize (Aliesrite* versus Persona), Myosotis (椿. versus M2U), Saudade (mocha versus Nhato), and others. Artist identity matters as well as spelling.

## Local database audit

Read-only SQLite queries checked 20,549 PMS records / 16,528 unique hashes, joining song information for note counts, duration and density. Mode 9 and every `.pms` file were considered, including five-button PMS stored as mode 9. Title and prefix searches produced 486 candidate hashes; a separate near-spelling pass checked normal-table titles. Candidates were reviewed against artist identity and normal/insane/excluded source hashes.

No additional confirmed beginner charts resulted. FREEDOM DiVE, AXION, Ascension to Heaven and Aragami had only insane-table matches in this library. Old raw file levels were not mistaken for current normalized ratings. Other tracked songs with no normal match appear in the site's coverage section. This does not establish that no easier charts exist elsewhere.

Private database paths and audit dumps remain local and are not published. Neither game database was modified.

## Rebuild

Python 3, standard library only:

```sh
python build.py --base-url https://sehun-joo.github.io/cytus-pms-beginner
```

GitHub Pages deploys `dist` on main-branch pushes. Matching changes require an intentional review of `catalog.json`. Independent fan table; not affiliated with Rayark or the source maintainers.
