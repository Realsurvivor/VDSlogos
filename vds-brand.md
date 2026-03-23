---
name: vds-brand
description: |
  Complete Van de Socials brand style guide. Use this skill whenever designing anything for Van de Socials:
  websites, landing pages, social media graphics, presentations, emails, documents, or any other visual output.

  Use when:
  - Building web pages or components for Van de Socials
  - Creating presentation slides
  - Designing social media content
  - Making any visual asset in the VDS huisstijl
  - Asking "what font/color/logo should I use for Van de Socials?"

  Keywords: van de socials, vds, huisstijl, brand, logo, design, social media agency
---

# Van de Socials — Brand Style Guide

## Brand Identity

Van de Socials is een **social media bureau** gericht op groei via short-form content en strategie. De toon is **jeugdig, energiek en professioneel**. Het design is **bold en direct** — hoge contrasten, sterke typografie, geen franjes.

---

## Kleuren

Gebruik **uitsluitend** deze vijf officiële kleuren. Gebruik nooit andere kleuren tenzij expliciet gevraagd.

| Naam     | Hex       | RGB              | Gebruik                                      |
|----------|-----------|------------------|----------------------------------------------|
| Orange   | `#faa700` | 250, 167, 0      | Primaire accentkleur, CTA-knoppen, highlights |
| Green    | `#064449` | 6, 68, 73        | Achtergronden, headers, primaire vlakken      |
| Black    | `#231f20` | 35, 31, 32       | Donkere achtergronden, tekst op lichte vlakken |
| White    | `#ffffff` | 255, 255, 255    | Tekst op donkere vlakken, lichte achtergronden |
| Grey     | `#ebedec` | 235, 237, 236    | Lichte achtergrond (alternatief voor wit)     |

### Gradient

```css
background: linear-gradient(135deg, #faa700, #fa7300);
```

De gradient loopt van orange (`#faa700`) naar een diepere oranje (`#fa7300`). Gebruik voor:
- Primaire CTA-knoppen
- Highlight blokken
- Accentelementen (badges, icoontjes, dividers)

### CSS Tokens

```css
:root {
  --orange:   #faa700;
  --orange2:  #fa7300;
  --gradient: linear-gradient(135deg, #faa700, #fa7300);
  --green:    #064449;
  --black:    #231f20;
  --white:    #ffffff;
  --grey:     #ebedec;
}
```

### Kleurcombinaties — Regels

| Achtergrond | Tekst/Logo    | Toegestaan |
|-------------|---------------|------------|
| Green       | Wit           | ✅         |
| Green       | Orange        | ✅         |
| Black       | Wit           | ✅         |
| Black       | Orange        | ✅         |
| Orange/Gradient | Zwart     | ✅         |
| Grey        | Zwart         | ✅         |
| White       | Zwart         | ✅         |
| White       | Orange        | ⚠️ alleen groot/bold (contrast te laag voor kleine tekst) |
| White       | Green         | ✅         |
| Orange      | Wit           | ❌ (onvoldoende WCAG contrast)  |

---

## Typografie

**Enig toegestaan lettertype: Montserrat** (Google Fonts)

```html
<link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,400;0,500;0,600;0,700;0,800;0,900;1,700&display=swap" rel="stylesheet">
```

```css
font-family: 'Montserrat', sans-serif;
```

### Typescale

| Naam     | Gewicht | Grootte | Gebruik                        |
|----------|---------|---------|--------------------------------|
| Display  | 900     | 48–96px | Hero titels, grote statements  |
| Kop 1    | 800     | 32–48px | Paginatitels                   |
| Kop 2    | 700     | 22–32px | Sectietitels                   |
| Body     | 400     | 15–16px | Lopende tekst                  |
| Label    | 700     | 11–13px | Tags, eyebrows, uppercase labels |

### Typografie regels

- Letter-spacing bij labels/eyebrows: `0.08em` tot `0.15em` + `text-transform: uppercase`
- Line-height body: `1.6–1.7`
- Line-height headings: `1.0–1.2`
- Letter-spacing display: `-0.02em` (negatief voor compactheid)

---

## Logo's

Alle logo's staan op GitHub en zijn direct bruikbaar via URL:

**Base URL:** `https://raw.githubusercontent.com/Realsurvivor/VDSlogos/main/`

### Beschikbare varianten

| Bestand | Beschrijving | Beste gebruik |
|---------|-------------|---------------|
| `vandeSocials_Logo_Standard_FullColor_RGB_DEF.png` | Horizontaal logo, kleur (oranje badge + groene tekst) | Lichte achtergronden, drukwerk |
| `vandeSocials_Logo_Standard_Diapositief_RGB_DEF.png` | Horizontaal logo, wit | Donkere achtergronden (black, green) |
| `vandeSocials_Logo_Circle_FullColor_RGB_DEF.png` | Cirkellogo, kleur (oranje/groen) | Lichte achtergronden |
| `vandeSocials_Logo_Circle_Black_RGB_DEF.png` | Cirkellogo, zwart | Witte/lichte achtergronden |
| `vandeSocials_Logo_Circle_White_RGB_DEF.png` | Cirkellogo, wit | Donkere achtergronden (black, green) |
| `vandeSocials_Logo_Circle_Diapositief_RGB_DEF.png` | Cirkellogo, wit/transparant | Donkere achtergronden, slotslides |
| `vandeSocials_Logo_Square_White_RGB_DEF.png` | Vierkant/horizontaal, wit | Banners, headers op donker |
| `vandeSocials_Logo_favicons_alpha-02.png` | Favicon/icoon variant | Browser tabs, app icons |

### Logo gebruik per achtergrond

| Achtergrond | Gebruik dit logo |
|-------------|-----------------|
| **Green** (`#064449`) | `vandeSocials_Logo_Circle_White_RGB_DEF.png` of `Standard_Diapositief` |
| **Black** (`#231f20`) | `vandeSocials_Logo_Circle_Diapositief_RGB_DEF.png` of `Standard_Diapositief` |
| **Orange/Gradient** | `vandeSocials_Logo_Circle_White_RGB_DEF.png` |
| **White** (`#ffffff`) | `vandeSocials_Logo_Standard_FullColor_RGB_DEF.png` of `Circle_Black` |
| **Grey** (`#ebedec`) | `vandeSocials_Logo_Standard_FullColor_RGB_DEF.png` of `Circle_Black` |

### Logo regels

- Houd minimaal **20% witruimte** rondom het logo vrij
- Verander **nooit** de kleur of verhoudingen van een logo
- Voeg **geen** effecten toe (slagschaduwen, outlines, filters)
- Gebruik altijd de aangeleverde variant — niet zelf namaken

---

## Design Stijl

### Tone

Bold, direct, modern. Geen onnodige decoratie. Hoge contrasten. Voelt energiek maar professioneel.

### Border-radius

Afgeronde hoeken: `20px` voor kaarten/blokken, `100px` voor knoppen en badges.

### Borders

Subtiel: `1px solid rgba(255,255,255,0.1)` op donkere achtergronden, `1px solid rgba(35,31,32,0.1)` op lichte.

### Spacing

8px-systeem: `8 / 16 / 24 / 32 / 48 / 64 / 96px`

---

## Componenten

### Primaire knop

```css
background: linear-gradient(135deg, #faa700, #fa7300);
color: #231f20;
font-family: 'Montserrat', sans-serif;
font-weight: 700;
font-size: 13–14px;
padding: 11px 22px;
border-radius: 100px;
border: none;
```

### Secundaire knop

```css
background: #064449;
color: #ffffff;
/* zelfde overige stijl als primair */
```

### Ghost knop

```css
background: transparent;
color: currentColor;
border: 1.5px solid rgba(255,255,255,0.1); /* of rgba(35,31,32,0.1) op licht */
```

### Badge/Tag

```css
font-size: 10–11px;
font-weight: 700;
letter-spacing: 0.06em;
text-transform: uppercase;
padding: 5px 12px;
border-radius: 100px;
```

Varianten: oranje (gradient), groen (`#064449` + wit), subtiel (achtergrond kleur).

---

## Thema's

### Donker thema

```css
--bg:        #231f20;
--bg-card:   #2e2a2b;
--bg-subtle: #332e2f;
--text:      #ffffff;
--muted:     rgba(255,255,255,0.45);
--border:    rgba(255,255,255,0.1);
```

### Licht thema

```css
--bg:        #ebedec;
--bg-card:   #ffffff;
--bg-subtle: #dfe1e0;
--text:      #231f20;
--muted:     rgba(35,31,32,0.45);
--border:    rgba(35,31,32,0.1);
```

---

## Presentatie Slides

### Aanbevolen slide-types

| Type | Achtergrond | Logo |
|------|-------------|------|
| **Titelslide** | Green `#064449` | `Circle_White` rechtsboven |
| **Inhoud/bullets** | Bg-card (donker of licht) | `Circle_Black` in header |
| **Statistieken** | Green `#064449` | — |
| **Quoteslide** | Orange gradient | `Circle_Black` transparant rechtsonder |
| **Afsluitslide** | Black `#231f20` | `Circle_Diapositief` rechtsboven |

### Slide layout regels

- Beeldverhouding: **16:9**
- Titel op afsluitslide: groot wit, accentwoord in orange
- Eyebrow boven titel: uppercase, klein, orange
- Contactinfo onderaan: gescheiden door een subtiele `border-top`
- Nummering: oranje cijfer + hoofdletters tekst

### Statistieken opmaak

Grote statistieken (bijv. `+340%`) altijd in:
- Font: Montserrat 900
- Kleur: `#faa700` (orange) of `linear-gradient(135deg, #faa700, #fa7300)`
- Achtergrond: green of dark

---

## Social Media Formaten

| Platform | Formaat | Afmetingen |
|----------|---------|------------|
| Instagram Feed vierkant | 1:1 | 1080 × 1080 px |
| Instagram Feed portret | 4:5 | 1080 × 1350 px |
| Instagram Story / Reel | 9:16 | 1080 × 1920 px |
| LinkedIn post | liggend | 1200 × 628 px |
| LinkedIn banner | panorama | 1584 × 396 px |
| Facebook post | liggend | 1200 × 630 px |
| TikTok video | 9:16 | 1080 × 1920 px |
| YouTube thumbnail | 16:9 | 1280 × 720 px |

---

## Do's & Don'ts

### ✅ Wel doen

- Gebruik **alleen** de vijf officiële kleuren
- Gebruik **Montserrat** als enig lettertype
- Kies het juiste logo op basis van de achtergrondkleur (zie tabel)
- Gebruik de gradient voor primaire CTA's en accentelementen
- Houd tekst op donker vlak altijd wit
- Gebruik uppercase + letter-spacing voor labels en eyebrows

### ❌ Niet doen

- Geen andere lettertypes (niet Inter, niet Roboto, niet Arial)
- Geen kleuren buiten het palet
- Geen wit logo op witte of lichte achtergrond
- Geen oranje logo op oranje achtergrond
- Geen zwart logo op groene of zwarte achtergrond
- Geen slagschaduwen of filters op logo's
- Geen andere verhoudingen of kleuren op logo's toepassen

---

## Referenties

- **Huisstijl HTML pagina:** `https://raw.githubusercontent.com/Realsurvivor/VDSlogos/main/huisstijl.html`
- **Logo repository:** `https://github.com/Realsurvivor/VDSlogos`
- **Website ter inspiratie:** `https://vandesocials.nl`
