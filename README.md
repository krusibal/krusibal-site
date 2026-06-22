# Ivan Žujović — statički sajt

## V3 sadržaj
- glavni hero zadržava informativni ulaz „Da li je ovaj rad za mene?“
- sekundarni hero CTA je preciziran: „Znam temu — ulazno mapiranje“
- duplirani vizuelni CTA za mapiranje zamenjen je tihim tekstualnim linkom
- generički Linktree link je uklonjen iz footera svih stranica
- Linktree ostaje samo kao operativni korak u kontekstualnim CTA-ovima (mapiranje, 1:1, radionice i biznis)
- tekstovi ličnih CTA-ova su precizirani: „Zakaži ulazno mapiranje“ i „Pošalji upit za rad 1:1“

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

## Napomena o Linktree CTA-ovima
Trenutni lični CTA-ovi vode na postojeći profil `linktr.ee/krusibal`, jer su tamo aktivni operativni tokovi. Kada napraviš zasebne deljive URL-ove za mapiranje i 1:1, zameni samo odgovarajuće `href` vrednosti u:
- `ulazno-sistemsko-mapiranje/index.html`
- `rad-1-na-1/index.html`
- `radionice/index.html`
