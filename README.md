# Tehnosen – E-trgovina (prodavnica)

Frontend demo prodavnice na srpskom jeziku, namenjen pregledanju proizvoda i simulaciji kupovine. Projekat koristi lokalni Node.js mock API; nije povezan sa stvarnim sistemom za plaćanje ili produkcionom bazom podataka.

## Funkcionalnosti

- Katalog proizvoda sa opisima, detaljima i recenzijama
- Pretraga, filtriranje i sortiranje proizvoda
- Korpa za kupovinu sa podešavanjem količine
- Registracija i prijavljivanje preko lokalnog mock API-ja
- Checkout forma sa validacijom podataka i simulacijom slanja porudžbine
- Validacija demo promotivnih kodova
- Kontakt forma

## Tehnološki stek

- HTML, CSS i JavaScript
- React za prikaz korpe
- Node.js za lokalni razvojni server i mock API
- JSON fajlovi za demo podatke o proizvodima i lokalno stanje mock API-ja

## Pokretanje lokalno

Potrebni su Node.js i npm. Iz korena repozitorijuma pokreni:

```bash
npm run dev
```

Ova komanda pokreće frontend server i mock API. Otvori prodavnicu na `http://localhost:8093`. Mock API sluša na `http://localhost:3001`.

Za zaustavljanje oba servera pritisni `Ctrl+C` u terminalu u kom je pokrenut `npm run dev`.

Ako je neki od portova zauzet, zaustavi prethodni proces iz njegovog terminala (najčešće `Ctrl+C`), pa ponovo pokreni komandu. Nemoj istovremeno pokretati dodatne instance istih servera na istim portovima.

## Napomena o demo verziji

Checkout samo demonstrira korisnički tok i šalje demo porudžbinu lokalnom mock API-ju. Ne unosi stvarne lične ili platne podatke; projekat ne obrađuje stvarna plaćanja i nije namenjen produkcionoj upotrebi.

## Struktura projekta

- `index.html` — početna tačka sajta
- `css/` — stilovi
- `js/` — navigacija i logika korisničkog interfejsa
- `src/api/apiClient.js` — klijent za lokalni mock API
- `api_response.json` — demo katalog proizvoda
- `postman/mocks/mock.js` — lokalni mock API
