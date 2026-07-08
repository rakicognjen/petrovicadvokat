# Sajt — Advokat Marko A. Petrović

Astro projekat, statičan sajt, 9 stranica, SEO optimizovan (meta tagovi, sitemap, robots.txt, JSON-LD structured data — Attorney + Article schema).

## Pokretanje lokalno

```bash
npm install
npm run dev
```

Sajt će biti dostupan na http://localhost:4321

## Build za produkciju

```bash
npm run build
```

Statični fajlovi se generišu u `dist/` folderu — mogu se otpremiti na bilo koji hosting (Netlify, Vercel, cPanel, itd.)

## Pre lansiranja — obavezno proveriti

1. **Domen**: u `astro.config.mjs` je postavljen placeholder `https://advokatpetrovic.rs` — zameniti pravim domenom (koristi se za sitemap i kanonske URL-ove).
2. **Fotografije**: sajt trenutno koristi grafički "§" motiv umesto fotografije advokata (nismo imali profesionalnu fotografiju). Preporuka: dodati profesionalnu fotografiju u hero sekciju na početnoj i "O advokatu" stranici.
3. **Kontakt forma**: forma na `/kontakt` trenutno otvara email klijent posetioca (mailto) — radi bez servera, ali za bolje korisničko iskustvo preporučujem povezivanje sa servisom poput Web3Forms ili Formspree.
4. **Radno vreme**: postavljeno Pon–Pet 09:00–17:00 — proveriti da li je tačno.
5. **Pravni sadržaj**: tekstovi o oblastima prava i članci su opšteg, informativnog karaktera — preporučujem da ih advokat pregleda pre objavljivanja, posebno delove o rokovima i procedurama.

## Struktura stranica

1. `/` — Početna
2. `/o-advokatu` — O advokatu
3. `/oblasti-prava/gradjansko-pravo` — Građansko pravo
4. `/oblasti-prava/upravno-pravo` — Upravno pravo
5. `/oblasti-prava/krivicno-pravo` — Krivično pravo
6. `/blog` — Pravni saveti (lista članaka)
7. `/blog/prava-okrivljenog-u-krivicnom-postupku`
8. `/blog/zalba-na-resenje-upravnog-organa`
9. `/kontakt` — Kontakt
