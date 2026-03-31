# SmartSpot: Predikce obsazenosti lokálního hřiště

Tento projekt je závěrečnou prací pro kurz Building AI. (Projekt kurzu o vývoji umělé inteligence)

## Souhrn
SmartSpot je koncept aplikace využívající umělou inteligenci k předpovídání vytíženosti místního multifunkčního hřiště. Cílem je pomoci sousedům naplánovat si sportovní aktivity tak, aby se vyhnuli přeplněným hodinám a efektivně využívali veřejný prostor. Rozsah projektu je přibližně 250 znaků.

## Pozadí
V naší čtvrti je pouze jedno moderní hřiště, které využívají fotbalisté, basketbalisté i rodiny s dětmi. Často se stává, že lidé přijdou s vybavením, ale hřiště je beznadějně plné.
* **Problém:** Neefektivní využívání času a zklamání uživatelů při náhodné návštěvě.
* **Četnost:** Problém nastává denně, zejména během slunečných odpolední a víkendů.
* **Motivace:** Chci podpořit aktivní životní styl v komunitě tím, že odstraním nejistotu "bude tam volno?".
* **Důležitost:** Lepší správa veřejných zdrojů, posílení komunity a snížení frustrace obyvatel.

## Jak se používá?
Uživatel otevře jednoduchou webovou aplikaci předtím, než vyrazí z domova. 
1. **Zobrazení aktuálního stavu:** AI na základě dostupných dat odhadne aktuální zaplněnost (např. 80 % – "téměř plno").
2. **Předpověď:** Uživatel si může v kalendáři vybrat konkrétní čas a uvidí pravděpodobnost volného místa na základě historických trendů a předpovědi počasí.
3. **Cílová skupina:** Místní sportovci, amatérské týmy, trenéři mládeže a rodiče s dětmi.

## Data a techniky umělé inteligence
Jelikož se zaměřuji na logický návrh bez programování, projekt by teoreticky využíval následující zdroje a metody:
* **Zdroje dat:**
    * Historická data o obsazenosti (ruční záznamy od správce nebo anonymní data z Wi-Fi hotspotu).
    * Data o počasí z veřejných API (teplota, srážky, vítr).
    * Kalendářní data (státní svátky, školní prázdniny, lokální akce).
* **Techniky AI:**
    * **Lineární regrese:** Pro určení korelace mezi počasím a počtem návštěvníků.
    * **Analýza časových řad:** Pro identifikaci pravidelných týdenních cyklů (např. pravidelné tréninky v úterý odpoledne).
    * **Rozhodovací stromy:** Pro klasifikaci stavu hřiště (Volno / Částečně obsazeno / Plno).

## Výzvy
* **Ochrana soukromí:** Systém nesmí používat biometrická data nebo identifikovat konkrétní osoby (např. přes kamerový systém), pouze počítat anonymní objekty.
* **Nepředvídatelné události:** AI nedokáže bez ručního zásahu předpovědět náhlou uzavírku hřiště kvůli havárii nebo údržbě.
* **Přesnost dat:** Bez automatických senzorů (IoT) bude sběr dat na začátku náročný a model může být méně přesný.

## Co dál?
Projekt by se mohl v budoucnu rozrůst na celou síť sportovišť v rámci města. Dalším krokem by byla integrace s jednoduchými IoT senzory pro automatické sčítání lidí v reálném čase, což by model výrazně zpřesnilo. K realizaci by byla potřeba pomoc vývojáře se znalostí Pythonu a odborníka na datové senzory.

## Poděkování
* Inspirace: Kurz Elements of AI a Building AI (University of Helsinki & Reaktor).
* Šablony pro README a dokumentaci z komunity GitHub.
