# Spolupráce chatů na ArtEli

Hlavní chat drží cíl hry a potvrzená rozhodnutí. Pět pracovních chatů používá společný repozitář, aby jejich výstupy byly dohledatelné a navazovaly na sebe. V současnosti jsou připravené jejich prompty; samotné chaty se zakládají samostatně.

## Odpovědnosti a výstupy

| Role | Hlavní oblast | První výstup |
| --- | --- | --- |
| Projektový manažer | `docs/planning/` | Malý plán prototypu, backlog s kritérii hotovosti a pořadí práce. |
| Grafik | `docs/art/`, `assets/` | Výtvarné směry, pravidla čitelnosti a seznam prvních assetů. |
| Level designér | `docs/levels/` | Návrh malé mapy s volbou cest, běžným cílem a bonusem pro dva. |
| Developer | `docs/technical/`, budoucí herní projekt a pomocné nástroje | Technický základ, návrh architektury a první implementační krok. |
| Tester | `docs/testing/`, budoucí testy | Scénáře testování a kritéria pro oba režimy a výbavu bez textu. |

Pro implementaci mapy koordinuje level designér konkrétní soubory s developerem. Úpravy herních scén, hlavního konceptu a společného plánu se předávají výslovně, aby nevznikly souběžné protichůdné změny.

## Doporučené pořadí začátku

1. Projektový manažer zpřesní malý rozsah a priority.
2. Developer připraví technický návrh; grafik, level designér a tester mohou nezávisle navrhnout své podklady.
3. Nejprve se ověří pohyb, gamepady, kamera a split screen s provizorní grafikou.
4. Postupně přibude boj, parťáci, loot a běžný i společný bonusový cíl.
5. Tester a rodič ověří technické chování i srozumitelnost při skutečném hraní.

Jde o návrh pořadí, který projektový manažer může podle zjištění upravit. Automatické zakládání chatů, posílání zpráv jiným chatům a externí publikování nejsou součástí úvodních promptů.

## Předávání práce

Každý výstup má uvést hotovou práci, soubory, ověření, otevřené otázky a vstup potřebný od další role. Návrhy musí být označené, aby se nepletly s rozhodnutími uživatele. Backlog projektového manažera bude společným přehledem práce; GitHub Issues nebo Projects lze zavést později podle potřeby.

Chaty otevřené ve stejné složce sdílejí pracovní soubory. Před změnou se kontroluje jejich aktuální stav a zachovává práce dalších rolí. Oddělené větve či worktrees řešíme podle konkrétní souběžné práce. Prompty nedávají roli oprávnění přepisovat změny ostatních.

## Podklady k přípravě promptů

Prompty mají vymezený úkol, výstupy a odkazy na relevantní podklady. Společná pravidla jsou soustředěná v `AGENTS.md`, aby se nemusely opakovat v každém úkolu. Jde o vlastní uspořádání tohoto projektu inspirované [doporučením OpenAI Docs pro projektové instrukce](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra).
