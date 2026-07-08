# NESIA YouTube Standards

Repo pre štandardizáciu YouTube práce pre NESIA. Aktuálny hlavný formát je **TALKSHOW**.

> Stav tejto verzie: `v0.7.0-repo-rename-analytics-workflow`  
> Dátum aktualizácie: 2026-07-08  
> GitHub účet: `martin-evis`  
> Oblasť: YouTube / obsah / publikovanie / analytika / benchmarking

## Poznámka k premenovaniu repozitára

Tento repozitár sa pôvodne volal:

```text
martin-evis/nesia-youtube-publishing-standards
```

Nový názov je:

```text
martin-evis/nesia-youtube-standards
```

Premenovanie bolo urobené preto, že repozitár už nepokrýva iba YouTube publishing, ale širší štandard práce s YouTube obsahom pre NESIA: publikačné balíky, metadáta, texty, performance poznámky, analytiku, benchmarking a opakovateľné workflowy pre NESIA Talkshow.

## Čo je cieľ repozitára

Repo má byť praktický pracovný štandard pre nové aj existujúce NESIA videá. Pri novom alebo historickom videu má pomôcť pripraviť a udržiavať:

1. 3–5 variantov nadpisu,
2. odporúčaný finálny nadpis,
3. krátky aj dlhý popis,
4. kapitoly / časové značky,
5. hashtagy,
6. tagy / štítky,
7. playlist,
8. thumbnail text a brief pre grafika,
9. pripnutý komentár,
10. interný kontrolný checklist pred publikovaním,
11. bezpečný analytický report,
12. benchmarking medzi jednotlivými videami alebo sériami.

## Zásadné pravidlo

GitHub nie je archív videí. Do repozitára patria **texty, metadáta, pravidlá, šablóny, prompty, analýzy, public-safe performance poznámky a výstupné balíky**.

Do repozitára nepatria veľké video súbory (`mp4`, `mov`, `mkv`) ani nečistené exporty z YouTube Studio. Pri verejnom repozitári sem nepatria ani interné dáta ako detailná retencia, CTR, watch time, zdroje návštevnosti, rozpočty alebo neverejné kontakty.

Ak sa pracuje s internými YouTube Analytics screenshotmi, do GitHubu sa ukladá iba očistený súhrn, metodika, šablóna alebo anonymizovaná interpretácia.

## Aktuálny rozsah

Aktuálna verzia obsahuje 6 zdrojových TALKSHOW videí:

| # | Video | Typ | Stav |
|---:|---|---|---|
| 1 | `R4A0CzH93XI` | full episode | pôvodný popis, hashtagy a kapitoly doplnené |
| 2 | `hKhO7xT_IxQ` | full episode | pôvodný popis, hashtagy a kapitoly doplnené |
| 3 | `KdZ-HHPUpWs` | full episode + audience interaction | pôvodný popis, hashtagy a kapitoly doplnené |
| 4 | `wnlNvGYrnhw` | full episode + music segment | pôvodný popis, hashtagy a kapitoly doplnené; chýba presný deň publikovania |
| 5 | `7MfOiVWXNJg` | best-of compilation | pôvodný popis a hashtagy doplnené; kapitoly nie sú v popise |
| 6 | `LU2foQMJVsg` | full episode + music segment | pôvodný popis, hashtagy a kapitoly doplnené; výkon treba doplniť neskôr |

Detailné dáta sú v:

```text
content/talkshow/published/
```

## Odporúčaná štruktúra

```text
.
├── README.md
├── AGENTS.md
├── CHANGELOG.md
├── docs/
│   ├── 00-public-repo-mode.md
│   ├── 06-content-data-model.md
│   ├── 07-storage-policy.md
│   ├── 08-iteration-workflow.md
│   ├── 09-talkshow-video-analytics-workflow.md
│   └── 10-talkshow-performance-benchmarking.md
├── content/
│   └── talkshow/
│       ├── README.md
│       ├── missing-data-tracker.md
│       ├── drafts/
│       └── published/
│           ├── index.md
│           └── YYYY-MM-DD-videoid-slug/
│               ├── source-metadata.yaml
│               ├── raw-input.md
│               ├── source-description.md
│               ├── source-transcript.md
│               ├── analysis.md
│               └── performance-notes.md
├── rules/
│   └── talkshow/
│       ├── voice-of-tone-draft-v0.4.md
│       ├── title-rules-draft-v0.4.md
│       ├── description-rules-draft-v0.4.md
│       ├── metadata-rules-draft-v0.4.md
│       └── thumbnail-rules-draft-v0.4.md
├── templates/
│   └── talkshow/
│       ├── new-video-brief-template.md
│       └── video-analytics-report-template.md
├── prompts/
│   └── talkshow/
│       ├── create-youtube-pack-from-transcript.md
│       └── analyze-youtube-analytics-screenshots.md
├── outputs/
└── scripts/
```

## Ako repo používať

1. Pri novom TALKSHOW videu najprv vytvor brief podľa `templates/talkshow/new-video-brief-template.md`.
2. Doplň transcript alebo pracovné poznámky.
3. Použi prompt `prompts/talkshow/create-youtube-pack-from-transcript.md`.
4. Výstup ulož do `outputs/talkshow/`.
5. Po publikovaní doplň finálny záznam do `content/talkshow/published/`.
6. Pri väčšej zmene aktualizuj `CHANGELOG.md`.
7. Pri vyhodnocovaní videa použi `docs/09-talkshow-video-analytics-workflow.md` a šablónu `templates/talkshow/video-analytics-report-template.md`.
8. Pri porovnávaní viacerých videí použi `docs/10-talkshow-performance-benchmarking.md`.

## Aktuálne otvorené položky

- Doplnit transcripty / titulky pre 6 zdrojových videí.
- Doplnit tagy zo Studia, ak budú dostupné.
- Doplniť bezpečný public výkon pre video `LU2foQMJVsg`.
- Overiť presný dátum publikovania videa `wnlNvGYrnhw`.
- Skontrolovať hashtag `#matejsucha` pri videu `wnlNvGYrnhw`, keďže bol ponechaný podľa dodaného pôvodného popisu.
- Pri ďalších Talkshow dieloch dopĺňať bezpečné performance poznámky a benchmarking bez interných exportov.
