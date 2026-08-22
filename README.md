# TechBeam — web

Statická jednostránka pre TechBeam. Bez build stepu — čistý HTML/CSS/JS
v jednom súbore (`index.html`), nasadzovaný cez GitHub Pages.

## Čo doplniť

Všetko, čo nevieme, je v kóde označené ako placeholder — vyzerá takto:
`[ VÁŠ E-MAIL ]`. Hľadaj v `index.html` triedu `ph` alebo hranaté zátvorky:

| Kde | Čo doplniť |
|---|---|
| Sekcia `#tim` | `[ ROLA ]` pri každom zo štyroch mien |
| Sekcia `#projekty` | `[ STAV ]` a `[ JEDNOVETOVÝ POPIS PROJEKTU ]` pre Maturant |
| Sekcia `#projekty` | `[ ĎALŠÍ PROJEKT ]` — alebo celý blok `.slot` zmaž |
| Pätička `#kontakt` | `[ VÁŠ E-MAIL ]`, `[ VÁŠ TELEFÓN ]` |
| Sekcia `#partneri` | Reálne logá Freedu / Examino / The Spot (teraz sú to wordmarky v našom fonte) |

Pri každom placeholderi je slovenská verzia priamo v HTML a anglická
v atribúte `data-en` — treba prepísať obidve.

## Jazyky

Slovenčina je napísaná priamo v HTML, angličtina žije v atribútoch
`data-en`. Prepínač SK/EN je v navigácii, voľba sa pamätá v `localStorage`.
Nový preložiteľný text = pridaj mu `data-en="..."`.

## Lokálne spustenie

```
python3 -m http.server 8000
```

Potom otvor <http://localhost:8000>.

## Nasadenie

Push do `main` spustí workflow `.github/workflows/deploy.yml`,
ktorý web publikuje na GitHub Pages.
