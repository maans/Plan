# Upload til GitHub

1. Pak ZIP-filen ud.
2. Upload hele indholdet af `Plan-main` til roden af repositoryet `maans/Plan`.
3. Bevar mapperne og lad eksisterende filer blive overskrevet.

Kontrollér især disse filer og mapper:

```text
index.html
README.md
plan-library/catalog.json
plan-library/
docs/manifest_spil.json
spil/kapardy/
plan-assets/
plan.webmanifest
```

Når GitHub Pages er opdateret, genindlæs Plan uden cache. Bibliotekets demoforløb skal nu hentes fra `plan-library/`, og KaPardy skal kunne åbne spil fra `docs/manifest_spil.json`.
