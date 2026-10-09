# Zawartość katalogu `skills`

Katalog zawiera sześć samodzielnych pakietów umiejętności dla pracy z polskimi i unijnymi zagadnieniami prawnymi. Każdy plik `.skill` jest archiwum ZIP z katalogiem głównym o nazwie umiejętności i plikiem `SKILL.md`, który opisuje jej zastosowanie oraz sposób działania. W zależności od pakietu archiwum zawiera także materiały referencyjne, skrypty, schematy, szablony lub testy.

## Pakiety

### `analiza-fto.skill` — analiza czystości patentowej

Pomaga ocenić ryzyko patentowe (Freedom to Operate) dla produktów i działalności B2B w Polsce i Europie. W pakiecie znajdują się:

- instrukcja umiejętności (`SKILL.md`);
- materiały o bazach patentowych, klasyfikacjach IPC/CPC i scenariuszach ryzyka;
- przykład analizy oraz szablon raportu;
- skrypt `generate_fto_report.py` do generowania raportu.

### `analiza-kontradyktoryjna.skill` — analiza argumentacji prawnej

Służy do krytycznej, kontradyktoryjnej oceny argumentów prawnych, w tym identyfikowania słabości i możliwych kontrargumentów. Pakiet zawiera:

- instrukcję (`SKILL.md`) oraz opracowania dotyczące błędów prawnych, kategorii ataków, cytowania, stylu, trybów analizy i źródeł prawa;
- szablony raportu oraz specyfikacje DOCX i JSON;
- skrypty do ekstrakcji argumentu, walidacji cytowań i generowania raportu DOCX.

### `analiza-rozumowania.skill` — analiza struktury rozumowania

Analizuje strukturę logiczną polskich tekstów prawnych za pomocą deterministycznego silnika GTMØ. Zawiera instrukcję i plik instalacyjny, a także bibliotekę `lib/` obejmującą:

- segmentację tekstu, lematyzację, embedding i klasyfikację segmentów;
- reguły klasyfikacji w `leksykon.json`;
- obliczanie metryk GTMØ i skrótów;
- potok analizy oraz generator raportu DOCX.

### `eu-pl-law-tracker.skill` — śledzenie prawa UE i prawa polskiego

Pomaga ustalać status aktów UE i powiązanych z nimi polskich aktów wdrażających, korzystając z oficjalnych źródeł, takich jak EUR-Lex, ISAP i RCL. Pakiet zawiera:

- instrukcję i README pakietu;
- materiały referencyjne dotyczące identyfikatorów EUR-Lex, wyszukiwania, wiarygodności źródeł i polskich aktów;
- skrypty do identyfikowania aktów, parsowania tekstu oraz ekstrakcji dat i relacji;
- testy jednostkowe dla skryptów.

### `legal-abduction.skill` — hipotezy konkurencyjne i macierz dowodów

Wspiera etapowe porządkowanie dokumentów, twierdzeń, obserwacji i hipotez oraz przygotowanie macierzy dowodów i planu testów. Jest oznaczony jako wersja ewaluacyjna przeznaczona wyłącznie do syntetycznych przypadków. W pakiecie znajdują się:

- instrukcje i dokumentacja użycia, instalacji, formatu pakietu sprawy oraz ograniczeń;
- moduły Pythona w `legal_abduction/` i skrypt uruchomieniowy `la.py`;
- schematy JSON i schemat bazy SQLite;
- szablony oraz pliki językowe polskie i angielskie;
- skrypty do sprawdzania jakości i walidacji pakietu.

Umiejętność proponuje wyniki do oceny przez człowieka — nie zatwierdza ich samodzielnie. Dane konkretnej sprawy należy przechowywać poza katalogiem umiejętności.

### `szukaj-orzeczen.skill` — wyszukiwanie orzeczeń

Służy do wyszukiwania orzeczeń sądowych i przygotowywania raportów tematycznych na podstawie serwisu SAOS oraz orzeczeń NSA. Pakiet zawiera instrukcję (`SKILL.md`) i skrypty do wyszukiwania orzeczeń, pobierania wyników z SAOS, pobierania danych z serwisu NSA oraz tworzenia raportu tematycznego.

## Uwagi

- Pliki `.skill` są samodzielnymi archiwami; skrypty i materiały pomocnicze znajdują się wewnątrz odpowiedniego archiwum.
- Umiejętności wspierają analizę i weryfikację materiałów, ale ich wyniki mają charakter pomocniczy i nie zastępują porady prawnika ani rzecznika patentowego.
