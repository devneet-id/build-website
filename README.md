# Build Website

**Forged through Rune. Built upon PHP.**

A small runite that builds a website without a framework. Write the page in many small files, and Rune bundles them into one: `dist/index.php`.

**[Explore Rune ↗](https://github.com/devneet-id/rune)**

---

## Made with Rune

This app is a **runite**: one file named `cast`, engraved from the origin runes of **[Rune](https://github.com/devneet-id/rune)**, a lore-driven, modular concept beneath PHP.

| Rune | Role in this app |
| ---- | ---------------- |
| Aether | opens and closes the flow |
| Chanter | registers the casts |
| Whisper | speaks to the user |
| Weaver | fills the templates while bundling |
| Crafter | bundles `src/` into `dist/index.php` |
| Forger | copies the website into `ready/` |
| Cipher | gives every bundle its hash |
| Keeper | remembers the shards in `.echoes` |
| Specter | serves and watches beside the flow |

Want to engrave your own? Start from the **[Rune repository](https://github.com/devneet-id/rune)**.

### Requirements

* PHP 8.1+
* Composer

### Install

```bash
composer install
php cast start
```

Then open `http://127.0.0.1:8000`.

---

## The Website

```
src/
├── index.head.html   goes into <head>
├── index.html        goes into <body>
├── index.css         becomes <style>
├── index.js          becomes <script>
└── index.php         runs on top, before the page
dist/
├── index.php         the bundle (php cast build)
└── assets/
    └── background.jpg
```

* Edit only `src/`. `dist/index.php` is made by `php cast build`.
* Put images and fonts in `dist/assets/`. The page reads them as `assets/...`.
* **The background** is `dist/assets/background.jpg`. Drop your own image there, no rebuild needed. Without it, the page falls back to a dark gradient.

---

## Registered Casts

| Cast | Description |
| ---- | ----------- |
| `build` | Bundle `src/` into `dist/index.php`. |
| `serve` | Serve `dist/` on `127.0.0.1:8000`. |
| `watch` | Rebuild when `src/` changes. |
| `start` | Build, then serve and watch. |
| `store` | Keep the assets as shards. |
| `ready` | Make `ready/` for production. |

---

## Try it

Run every command inside this folder.

**The main screen** — every cast with its echo:

```bash
php cast
```

**Build** — many files become one:

```bash
php cast build
```

**Develop** — `serve` and `watch` run until **Ctrl+C**:

```bash
php cast serve                            # http://127.0.0.1:8000
php cast watch                            # rebuild on every change in src/
php cast start                            # build, then serve & watch in their own windows
```

**Ship** — a folder you can upload to any PHP host:

```bash
php cast ready                            # build + store, then copy into ready/
```

**Share** — the runite and its shards as one relic:

```bash
php cast store
php cast reliquary --runite-relic         # cast -> cast.rune
```

**Built-in casts of Rune** — every runite carries them:

```bash
php cast grimoire --rune=Crafter          # look inside the builder
php cast grimoire --arcane                # every step of the last run
php cast reliquary --shards               # the files that travel with the relic
```

---

## What you learn

| Cast | Lesson |
| ---- | ------ |
| `build` | Crafter: item, seed, shard, spark |
| `serve`, `watch`, `start` | Specter: a dev server, an observer, casts beside the flow |
| `store` | Keeper: shards travel with the relic |
| `ready` | Forger: copy files and folders |

**A website is many files, Rune makes it one.**

---

## References

* [Rune](https://github.com/devneet-id/rune) — Application foundation and tooling.
* [Rune Lore](https://github.com/devneet-id/rune-lore) — The full documentation, from the void to the beyond.

---

**Built to create. Designed to evolve.**

**DEVNEET ©**
