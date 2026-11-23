# Kaamerakaart

Androidi installitav PWA, mis kuvab asukoha järgi Eesti avalikke Transpordiameti teekaameraid ja nende värskeimaid kaadreid.

## Avaldamine GitHub Pagesis

1. Loo GitHubis tühi repositoorium ja laadi selle kausta sisu `main` harusse.
2. Ava repositooriumis **Settings → Pages** ja vali allikaks **GitHub Actions**.
3. Workflow avaldab `dist/` kausta automaatselt.

Androidis ava avaldatud HTTPS-aadress Chrome'is ja vali **Install app** või **Lisa avakuvale**.

## Kohalik eelvaade

Serveeri `dist/` kausta HTTP-serveriga (service worker ei tööta `file://` aadressilt).

Andmeallikas: Transpordiamet / Tark Tee. Rakendus kuvab perioodiliselt uuenevaid kaadreid, mitte pidevat videovoogu. Kõigi maailma avalike kaamerate täielikku registrit ei eksisteeri; uus andmepakkuja saab lisada `app.js` faili.
