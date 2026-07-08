# Changelog

## v0.7.0-repo-rename-analytics-workflow – 2026-07-08

### Zmenené

- Repozitár bol premenovaný z `martin-evis/nesia-youtube-publishing-standards` na `martin-evis/nesia-youtube-standards`.
- README bol upravený tak, aby pokrýval širší rozsah: YouTube publikovanie, metadáta, analytiku, benchmarking a opakovateľné workflowy pre NESIA Talkshow.
- Dopĺňa sa explicitná poznámka, že starý názov bol zúžený na publishing, zatiaľ čo nový názov lepšie vystihuje širší účel repozitára.

### Pridané

- `docs/09-talkshow-video-analytics-workflow.md` – workflow pre bezpečnú analýzu videí z YouTube Analytics podkladov.
- `docs/10-talkshow-performance-benchmarking.md` – pravidlá porovnávania výkonu Talkshow videí.
- `templates/talkshow/video-analytics-report-template.md` – šablóna analytického reportu.
- `prompts/talkshow/analyze-youtube-analytics-screenshots.md` – prompt pre spracovanie screenshotov z YouTube Analytics.

### Poznámka

Repo je public. Detailné interné YouTube Studio exporty, screenshoty, rozpočty a citlivé analytické dáta zostávajú mimo GitHub. Do repozitára patria iba očistené súhrny, metodika, šablóny, prompty a public-safe poznámky.

## v0.6.1-sync-descriptions-metadata – 2026-06-15

### Opravené / zosúladené

- Zosúladený stav repozitára v `README.md` z `v0.4.0-public-content-architecture` na `v0.6.1-sync-descriptions-metadata`.
- Zosúladené `source-metadata.yaml` pre zdrojové TALKSHOW videá po doplnení pôvodných YouTube popisov.
- Pri zdrojových videách sú pôvodné popisy označené ako dostupné, hashtagy a kapitoly sú extrahované z dodaných popisov tam, kde boli dostupné.
- Zachované otvorené položky: transcripty / titulky, tagy zo Studia, bezpečný výkon pre čerstvé video a presný dátum publikovania pri Baťa epizóde.

### Poznámka

`v0.4.0-public-content-architecture` zostáva historická architektonická verzia. Aktuálny pracovný stav po doplnení a synchronizácii popisov je `v0.6.1-sync-descriptions-metadata`.

## v0.6.0-complete-original-descriptions – 2026-06-15

### Pridané

- Doplnené pôvodné YouTube popisy pre všetkých 6 zdrojových TALKSHOW videí.
- Doplnené popisy pre videá Matej Šucha, Gabriela Končitíková, BEST OF a Zuzana Šebová.

## v0.5.0-original-descriptions-1-2 – 2026-06-15

### Pridané

- Doplnené pôvodné YouTube popisy pre prvé dve TALKSHOW videá.
- Pri videu `R4A0CzH93XI` boli extrahované hashtagy a kapitoly.
- Pri videu `hKhO7xT_IxQ` bol doplnený pôvodný popis a pripravený podklad na synchronizáciu metadát.

## v0.4.0-public-content-architecture – 2026-06-14

### Pridané

- Zavedená jasná dátová vrstva `content/talkshow/published/` pre publikované TALKSHOW videá.
- Každé zo 6 vstupných videí má samostatný priečinok so súbormi:
  - `source-metadata.yaml`,
  - `raw-input.md`,
  - `source-description.md`,
  - `source-transcript.md`,
  - `analysis.md`,
  - `performance-notes.md`.
- Pridaný verejno-súkromný dátový režim pre public repo.
- Pridané draft pravidlá v `rules/talkshow/`.
- Pridané šablóny pre nové video a existujúci video záznam.
- Pridaný prompt pre tvorbu YouTube publikačného balíka z transcriptu.
- Pridaný validátor `scripts/validate_talkshow_source_records.py`.

### Zmenené

- README prerobené z pôvodnej skeleton dokumentácie na praktický pracovný štandard.
- AGENTS.md rozšírený o pravidlá pre verejný repozitár a oddelenie faktov od analýzy.
- `content/talkshow/missing-data-tracker.md` je hlavný zoznam chýbajúcich údajov.

### Poznámka

Repo je použiteľné aj vo verejnom režime. Interné YouTube Studio dáta však patria mimo public repozitára alebo musia byť anonymizované.

## v0.3.0-talkshow-source-videos-1-6 – 2026-06-14

- Doplnených 6 TALKSHOW videí ako zdrojové prípady.
- Pridané prvé drafty voice of tone, title rules a description rules.

## v0.1.0-talkshow – 2026-06-14

- Založená prvá kostra repozitára pre NESIA YouTube TALKSHOW workflow.
