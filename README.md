# Hlášení závad košů (Obec Běloky)

Jednostránková landing page pro nahlášení závad veřejných košů přes QR kód.
Formulář odesílá data přes Formspree a automaticky rozlišuje konkrétní koš
podle parametru v URL.

## Použití

1. Vytvořte si formulář ve službě Formspree a zkopírujte endpoint.
2. V souboru `index.html` nahraďte `https://formspree.io/f/your-form-id`
   za svůj endpoint.
3. Vygenerujte QR kódy pro jednotlivé koše ve tvaru:
   `https://<vase-domena>/index.html?bin=KOS-123`

Parametr `bin` nebo `kos` se automaticky propíše do formuláře a zobrazí na stránce.

## Obsah formuláře

- Popis závady (povinné)
- Kontaktní e-mail (povinné)
- Fotografie závady (volitelné)

## Logo / znak obce

Znak obce je uložen lokálně v `assets/znak.png` a používá se v hlavičce stránky.

## Spuštění

Projekt je čisté HTML/CSS/JS, stačí soubor `index.html` nasadit na hosting
(např. GitHub Pages) a vygenerovat QR kódy.
