# Ivan Žujović — statički sajt

## V2 sadržaj
- jasna lična pozicija bez javnog korišćenja naziva Krusibal
- odvojena stranica za sistemsko mapiranje za biznis
- ispravljeni canonical URL-ovi za svaku stranicu
- Open Graph meta podaci i deljiva naslovna slika
- nova navigacija: Lični rad / Za biznis / Radionice / O meni / Prvi korak

## Objavljivanje
GitHub Pages: `main` → `/(root)`.

Za lokalni pregled:
```bash
python3 -m http.server 8080
```
pa otvori `http://localhost:8080`.

## Pre povezivanja domena
Ne preimenovati `CNAME.example` u `CNAME`.

## Posle povezivanja domena
1. U GitHub Pages u polje Custom domain uneti `krusibal.rs`.
2. Tek kad GitHub potvrdi domen, napraviti fajl `CNAME` sa samo: `krusibal.rs`.
3. U mCloud DNS panelu dodati zapise po GitHub Pages uputstvu.
4. Kada HTTPS postane dostupan, uključiti Enforce HTTPS.
