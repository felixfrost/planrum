# Planrum

Ett webbaserat ritverktyg för tidiga planlösningsskisser. Rita huskropp, rum, innerväggar, dörrar, fönster och möbler i meter. Projekt sparas i webbläsaren och kan delas via länk eller exporteras som JSON och SVG.

## Starta lokalt

Ingen byggprocess krävs. Kör `python3 -m http.server 8080 --directory public` i projektmappen och öppna `http://localhost:8080`.

## Publicera

Firebase Hosting är konfigurerat i `firebase.json`. Kör `firebase deploy --only hosting --project <projekt-id>`.

## Modellunderlag och begränsning

Appen använder LB-Hus modellnamn och publicerad boarea för fem startval:

- [LB Optimal 90](https://www.lbhus.se/vara-hus/lb-optimal-90/)
- [LB Optimal 117](https://www.lbhus.se/vara-hus/lb-optimal-117/)
- [LB Optimal 126](https://www.lbhus.se/vara-hus/lb-optimal-126/)
- [LB Optimal 146](https://www.lbhus.se/vara-hus/lb-optimal-146/)
- [LB Start 161](https://www.lbhus.se/vara-hus/lb-start-161/)

Startskissernas rumsplaceringar och huskroppsformer är illustrativa, inte avritade originalritningar. Optimal 146 har en vinkel och Start 161 en H-form; båda visar de publicerade yttermåtten som måttlinjer, men konturernas indrag är ungefärliga. Appen är fristående från LB-Hus. Exakta konstruktionsmått, bärande väggar, VVS, bygglov och tillval behöver granskas med hustillverkaren. SVG exporteras med fysisk storlek för skala 1:100; kontrollera utskriftsinställningarna.
