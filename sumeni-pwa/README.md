# Šumění

Mixér relaxačních zvuků (PWA). Každý zvuk má vlastní hlasitost a režim:
smyčka, nebo interval s náhodnou pauzou v rozsahu od–do sekund.

## Nasazení na GitHub Pages

1. Na GitHubu vytvoř nový repozitář, např. `sumeni` (Public; Pages na Private repu vyžaduje placený účet).
2. Nahraj obsah této složky do kořene repa (Add file > Upload files, nebo `git push`).
3. Settings > Pages > Source: **Deploy from a branch**, Branch: `main`, složka `/ (root)` > Save.
4. Za 1–2 minuty běží na `https://<uživatel>.github.io/sumeni/`.

## Instalace na Android

1. Otevři adresu v Chrome > menu ⋮ > **Přidat na plochu** / **Instalovat aplikaci**.
2. Nastavení > Aplikace > Chrome > Baterie > **Neomezeno** (aby hrála i se zhasnutým displejem).

## Data

Zvuky a mixy se ukládají v prohlížeči (IndexedDB) na daném zařízení, do repa se nic nenahrává.
Smazáním dat Chrome / odinstalací PWA zmizí.

## Aktualizace

Po změně `index.html` zvyš `VERSION` v `sw.js` (např. `sumeni-v2`), jinak telefon drží starou verzi z cache.
Nová verze se projeví po druhém otevření aplikace.
