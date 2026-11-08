# blocogames.github.io

The public website for Bloco Games: a studio page listing the games, one folder per game (landing page and privacy policy), and `app-ads.txt` for AdMob.

```
index.html           studio page, links to each game
app-ads.txt          one AdMob line, covers every game in the AdMob account
style.css            shared styles
blokkari/index.html  Blokkari's page
blokkari/privacy.html
```

## Before publishing

Contact email: danielserva+blocogames@gmail.com. Privacy policy effective date: November 8, 2026 (update it whenever the policy changes).

- `app-ads.txt`: replace its contents with the line AdMob gives you.

## Publishing

1. On GitHub, signed in as `blocogames`, create a public repository named exactly `blocogames.github.io`.
2. Push the contents of this folder to it:
   ```bash
   cd site
   git init -b main && git add . && git commit -m "Bloco Games site"
   git remote add origin https://github.com/blocogames/blocogames.github.io.git
   git push -u origin main
   ```
3. In the repository, go to *Settings → Pages*, set the source to *Deploy from a branch*, `main`, `/ (root)`.
4. After a minute, check `https://blocogames.github.io/blokkari/privacy.html` and `https://blocogames.github.io/app-ads.txt`.
5. In Play Console, set the website to `https://blocogames.github.io` and Blokkari's privacy policy to `https://blocogames.github.io/blokkari/privacy.html`.

## Adding a game

Copy `blokkari/` to a new folder named after the game, update its text, icon and privacy policy, and add a card for it in `index.html`. `app-ads.txt` doesn't change.
