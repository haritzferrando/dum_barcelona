# Estacionaments DUM Barcelona — Descàrrega automàtica

Aquest repositori descarrega automàticament cada dia el fitxer JSON dels estacionaments de les zones DUM (Distribució Urbana de Mercaderies) de Barcelona, publicat per l'Ajuntament al portal Open Data BCN.

## Contingut

- `.github/workflows/download_dum.yml` — Acció automàtica de GitHub
- `data/` — Fitxers JSON descarregats, un per dia (format: `YYYYMMDD_DUM.json`)

## Com funciona

Cada dia a les 08:00 UTC, GitHub executa automàticament el flux que:
1. Descarrega el fitxer JSON del portal Open Data BCN
2. El desa a la carpeta `data/` amb el nom de la data del dia
3. Fa un commit i puja el fitxer al repositori

## Execució manual

Pots llançar la descàrrega manualment en qualsevol moment des de:
`GitHub → Actions → Descàrrega diària DUM Barcelona → Run workflow`

## Font de les dades

[Open Data Barcelona — Estacionaments DUM](https://opendata-ajuntament.barcelona.cat/data/ca/dataset/estacionaments-dum)

Llicència: Creative Commons Attribution 4.0
