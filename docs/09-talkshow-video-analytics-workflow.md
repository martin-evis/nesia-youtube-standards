# 09 – NESIA Talkshow video analytics workflow

> Status: approved baseline  
> Repo: `martin-evis/nesia-youtube-standards`  
> Scope: bezpečný workflow pre vyhodnocovanie NESIA YouTube videí na základe YouTube Analytics podkladov

## Účel

Tento dokument definuje opakovateľný postup pre analýzu videí NESIA Talkshow.

Cieľom je, aby sa každé nové video nevyhodnocovalo odznova bez štruktúry, ale podľa rovnakého rámca:

- kľúčové metriky,
- správanie divákov,
- zdroje návštevnosti,
- zariadenia,
- publiká,
- retencia,
- porovnanie s predchádzajúcimi dielmi,
- odporúčania pre ďalšiu tvorbu.

## Vstupy

Pri každom videu sa zbierajú tieto vstupy:

```text
Názov videa:
YouTube URL:
Video ID:
Obdobie sledovania:
Cieľ videa:
Platená podpora: áno / nie / neznáme
Dostupné screenshoty z YouTube Analytics:
Poznámky k distribúcii:
```

## Odporúčané screenshoty

Ak sú dostupné, použi screenshoty z týchto sekcií YouTube Analytics:

1. Overview / Prehľad,
2. Engagement / Zapojenie,
3. Audience / Publikum,
4. Reach / Dosah,
5. Traffic sources / Zdroje návštevnosti,
6. Devices / Zariadenia,
7. Geography / Krajiny,
8. Subtitles / Titulky,
9. Returning vs new viewers,
10. Ads / paid traffic, ak bolo video podporené.

## Povinné metriky reportu

Pri každom videu sa snaž vyhodnotiť:

- zobrazenia,
- zhliadnutia,
- jedineční diváci,
- celkový čas pozerania,
- priemerná doba pozerania,
- priemerné percento zhliadnutia,
- retencia alebo udržanie publika,
- podiel nových a vracajúcich sa divákov,
- top zdroje návštevnosti,
- top zariadenia,
- krajiny,
- titulky,
- odberatelia vs. neodberatelia,
- like rate / reakcie, ak sú dostupné.

## Štruktúra výstupu

Každý analytický report má mať túto štruktúru:

1. základné údaje videa,
2. kľúčové výsledky,
3. publikum,
4. zariadenia,
5. zdroje návštevnosti,
6. engagement a retencia,
7. hlavné zistenia,
8. benchmarking s predchádzajúcimi videami,
9. odporúčania.

## Interpretácia

Neinterpretuj video len podľa jedného čísla.

Príklady:

- vysoké zobrazenia môžu byť výsledkom platenej podpory,
- nižšie zhliadnutia pri dlhom videu nemusia znamenať slabý obsah,
- vysoká priemerná doba sledovania je pri talkshow veľmi hodnotná,
- vysoký podiel neprihlásených divákov znamená priestor pre CTA na odber,
- veľký podiel mobile / TV ovplyvňuje titulky, thumbnail a úvod videa.

## Bezpečnostné pravidlo

Repo je verejné. Do GitHubu nevkladaj raw YouTube Studio exporty, interné rozpočty, detailné CTR, neverejné retencie ani screenshoty s citlivými údajmi.

Do GitHubu môže ísť:

- metodika,
- očistený report,
- public-safe zhrnutie,
- šablóna,
- prompt,
- anonymizovaný benchmark.

## Výstup mimo GitHub

Detailné interné reporty, screenshoty a pracovné podklady ukladaj mimo GitHub, napríklad do Google Drive alebo do schváleného interného systému.

Do GitHubu uveď iba bezpečnú referenciu, napríklad:

```text
internal_report_source: Google Drive / DOPLNIŤ
public_safe_summary: yes
raw_export_stored_in_github: no
```
