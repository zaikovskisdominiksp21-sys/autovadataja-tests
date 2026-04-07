# autovadataja-tests

## Ievads

Interaktīvs autovadītāja teorijas apmācību tests, kurā tiek parādīti ceļu satiksmes noteikumu jautājumi ar attēliem. Rīks palīdz gatavoties CSDD teorijas eksāmenam, nodrošinot taimeri, tūlītēju atgriezenisko saiti un galīgo rezultātu novērtējumu.

🔗 **[Rīku saraksts](https://rtk2023.github.io/riki/)** | 🔗 **[GitHub projekts](https://github.com/rtk2023/riki)**

---

## Pārskats

### Projekta arhitektūra

```
autovadataja-tests/
├── index.html      # Galvenā HTML lapa — trīs ekrāni (sākums, tests, rezultāti)
├── style.css       # Visi stili — responsīvs dizains, animācijas
├── script.js       # Testa loģika — jautājumi, taimeris, rezultāti
├── image/          # Jautājumu attēli (1.png – 10.png)
└── README.md       # Šī dokumentācija
```

### Kā rīks darbojas

1. **Sākuma ekrāns** — lietotājs redz testa informāciju un nospiež "Sākt testu"
2. **Testa ekrāns** — parādās jautājums ar attēlu un 3 atbilžu varianti; pēc atbildes tiek parādīts pareizais variants
3. **Rezultātu ekrāns** — tiek aprēķināts rezultāts, norādīts vai tests izturēts (≥7/10 = izturēts)

### Failu apraksts

| Fails | Apraksts |
|---|---|
| `index.html` | Trīs ekrānu struktūra ar Latvijas valsts fontu un atbilžu pogām |
| `style.css` | CSS mainīgie, responsīvs `grid` izkārtojums, animācijas taimerī |
| `script.js` | Jautājumu masīvs, taimeris (`setInterval`), atbilžu apstrāde, rezultāti |
| `image/` | PNG attēli katram jautājumam — ceļa zīmes, situācijas uz ceļa |

---

## Iespējamie uzlabojumi

- Pievienot vairāk jautājumu (pilnais CSDD tests ir 30 jautājumi)
- Sajaukt jautājumu un atbilžu secību nejauši (`Math.random`)
- Pievienot video jautājumus (kā norādīts uzdevuma nosaukumā)
- Saglabāt rezultātu vēsturi `localStorage`
- Pievienot jautājumu kategorijas (ceļa zīmes, noteikumi, pirmā palīdzība)
- Pieejamības uzlabojumi — klaviatūras navigācija, ARIA atribūti

### Zināmie defekti

- Attēli tiek ielādēti no lokālā `image/` mapes — jāpārvieto uz CDN vai ārēju avotu, ja rīks tiek publicēts GitHub Pages vidē bez bildēm repozitorijā

---

## Resursi

- [MDN Web Docs — JavaScript](https://developer.mozilla.org/lv/docs/Web/JavaScript)
- [W3C Validator](https://validator.w3.org/)
- [Google Lighthouse / PageSpeed](https://pagespeed.web.dev/)
- [WAVE Pieejamības pārbaude](https://wave.webaim.org)
- [CSDD Teorijas jautājumi](https://www.csdd.lv)

---


