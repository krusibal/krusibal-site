# Krusibal — statički sajt

Početna verzija javnog sajta za Ivan Žujović / Krusibal.

## Šta je uključeno

- statičke HTML stranice, bez frameworka i bez build procesa;
- mobile navigacija i jedinstven CSS;
- SEO osnova: title/meta opis, canonical URL, robots.txt, sitemap.xml, Person JSON-LD;
- odvojene javne stranice za glavne formate rada;
- 404 stranica;
- `CNAME.example`, koji se aktivira tek kada se poveže domen.

## Lokalni pregled

```bash
cd krusibal-site
python3 -m http.server 8080
```

Zatim otvori `http://localhost:8080`.

## Objavljivanje preko GitHub Pages

1. Na GitHub-u napravi **prazan public** repository: `krusibal-site`.
2. Iz ovog foldera pošalji sadržaj u `main` granu:

```bash
cd krusibal-site
git init
git add .
git commit -m "Initial Krusibal site"
git branch -M main
git remote add origin git@github.com:TVORJ_GITHUB_NALOG/krusibal-site.git
git push -u origin main
```

3. U repository-ju otvori `Settings → Pages`.
4. Pod `Build and deployment` izaberi **Deploy from a branch**.
5. Izaberi granu `main` i folder `/(root)`.
6. Sačekaj da GitHub objavi privremenu adresu `https://TVORJ_GITHUB_NALOG.github.io/krusibal-site/`.

## Domen — ne raditi pre testiranja privremene GitHub Pages adrese

Kada je sadržaj potvrđen, tek onda:

1. u `CNAME.example` ukloni komentare i preimenuj fajl u `CNAME`;
2. u GitHub `Settings → Pages` upiši `krusibal.rs` kao Custom domain;
3. u mCloud DNS panelu dodaj GitHub Pages DNS zapise prema aktuelnim GitHub uputstvima;
4. proveri HTTPS u GitHub Pages podešavanjima;
5. tek posle toga podesiti `ivanzujovic.rs` da preusmerava na kanonski domen.

## Sadržaj koji treba proveriti pre objave

- da li se na stranicama koriste tačni nazivi kvalifikacija;
- gde treba da vode CTA dugmad za mapiranje, rad 1:1 i radionice;
- da li želiš da se trenutne cene javno vide na sajtu ili samo u prijavi;
- da li je „IoPT-informed pristup” formulacija koju želiš na javnoj stranici.
