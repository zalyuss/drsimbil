# Animații premium + Craiova — DRS Imobil

**Data:** 2026-06-07
**Fișier afectat:** `index.html` (single-file, fără librării externe)
**Stil:** elegant & subtil, premium. Respectă `prefers-reduced-motion`.

## Obiectiv
Site-ul DRS Imobil (showcase imobiliar, Craiova) trebuie să arate „ca la carte" —
animații fine de nivel premium și menționarea clară a localizării în Craiova
(inclusiv SEO local). Totul se adaugă peste structura existentă fără a strica
ce funcționează deja.

## Constrângeri
- Un singur fișier `index.html`, fără dependențe externe (rapid, curat).
- Doar 4 poze reale: `poze/living.jpg`, `poze/bucatarie.jpg`, `poze/dormitor1.jpg`, `poze/baie1.jpg`.
- Fără date inventate (firma se prezintă pe ideea de cinste).
- Toate animațiile se dezactivează corect la `prefers-reduced-motion: reduce`.

## Funcționalități

### 1. Intro la încărcare (preloader)
Cortină full-screen espresso (~1.2s) cu logo „DRS Imobil" care apare fin + linie
teracotă care se trage. Apoi cortina alunecă în sus și dezvăluie hero-ul.
Apare o singură dată per încărcare. La reduced-motion: ascunsă instant.

### 2. Hero — titlu cinematic + parallax
- Titlul apare cuvânt cu cuvânt (ridicare fină, staggered).
- Pozele din slideshow se mișcă lent la scroll (parallax discret).
- Zoom foarte lent (Ken Burns) pe poza activă din slideshow.
- Slideshow-ul existent rămâne funcțional.

### 3. Galerie cu lightbox
Click pe card (cameră) → poza se deschide mare, centrat, fundal întunecat,
tranziție lină. Navigare: săgeți ‹ ›, tastatură (←/→/Esc), swipe pe mobil.
Sursa pozelor și titlurile se iau din cardurile existente.

### 4. „Despre" — 3 garanții animate
Cele 3 valori existente (Doar case / Vânzare în siguranță / Alături de tine)
primesc apariție animată elegantă (linie teracotă care se trage + text în
cascadă). Fără numere/cifre inventate.

### 5. Butoane magnetice + microinteracțiuni
- CTA principale urmăresc fin cursorul la hover (efect magnetic, doar desktop /
  dispozitive cu mouse — `(hover: hover)`).
- Microanimații fine la hover pe telefon și linkuri.

### 6. Craiova peste tot (conținut + SEO)
- `<title>`: „DRS Imobil · Case de vânzare în Craiova".
- Meta description, og:title/description, hero kicker, contact, footer: menționează Craiova.
- Adresă: „Craiova · Zona Selgros, Aleea Ficusului nr. 5".
- JSON-LD `RealEstateAgent` cu `addressLocality: Craiova`, telefon, adresă.

## Ce NU se schimbă
Structura HTML de bază, paleta de culori, fonturile, textele esențiale și cele
4 poze reale. Totul se adaugă incremental.

## Verificare
- Site-ul se deschide în browser și arată corect pe desktop + mobil (responsive).
- Preloader apare o dată și dispare.
- Titlul hero apare animat; parallax/Ken Burns vizibile la scroll.
- Lightbox: deschide, navighează (săgeți/tastatură/swipe), închide.
- Butoane magnetice funcționează pe desktop, normale pe mobil.
- Cu `prefers-reduced-motion: reduce` totul e static și utilizabil.
- „Craiova" apare în titlu, hero, contact, footer; JSON-LD valid.
