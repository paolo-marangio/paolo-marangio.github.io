# Setup instructions — Events portfolio (standalone user site)

This now lives on its own GitHub account (`paolo-marangio`), as a **user
site**, which means it'll be at the domain root:

```
https://paolo-marangio.github.io/
```

No subpath, no connection to `marangiop.github.io` — completely separate.

## 1. Add your images first

Drop your two photos into the `assets/` folder before pushing:

- `assets/profile.jpg` — your headshot
- `assets/precisiontox-dinner.jpg` — the June 2022 dinner photo

(See `assets/README.txt` for details — delete that file once your real
images are in.)

## 2. Create the repository

Log in as `paolo-marangio` on github.com and create a **new repository**
named exactly:

```
paolo-marangio.github.io
```

This exact name is what makes GitHub auto-host it at the root domain, no
extra config needed. Public, no README initialized (we already have one).

## 3. Push this folder

```bash
git init
git add .
git commit -m "Initial events portfolio"
git branch -M main
git remote add origin https://github.com/paolo-marangio/paolo-marangio.github.io.git
git push -u origin main
```

## 4. Pages should enable automatically

Because the repo name matches `paolo-marangio.github.io` exactly, GitHub
Pages usually turns itself on with no manual step. If it doesn't, go to
**Settings → Pages** and set Source to "Deploy from branch: main / root".

## 5. Wait a minute, then visit

```
https://paolo-marangio.github.io/
```

Check the **Actions** tab for a green checkmark first.

---

## Keeping the two sites separate

There are no links from this site to `marangiop.github.io` (your Notes
blog), and none should be added if you want them to stay unconnected —
and now they're on entirely different accounts too, so there's no shared
GitHub namespace linking them either.

## Adding more events later

Just add a new `## Event Name {#anchor-id}` section to `index.md`, and a
matching line in the "In this page" list at the top, same pattern as the
three existing events.
