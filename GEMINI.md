# GEMINI.md: ivellios-panel

To repo jest PUBLICZNE. Nie wpisuj tu żadnych tokenów, adresów prywatnych, haseł, danych domu
ani jawnego kodu panelu (zawiera dane prywatne).

## Co tu jest
Tylko zaszyfrowany plik `ivellios-panel-v3.enc` (panel Home Assistant, Lit 3), pobierany do HA
przez `downloader.download_file` z adresu raw GitHuba, przypiętego do SHA commita. HA
odszyfrowuje go lokalnie skryptem `/config/ivellios_panel_tool.py`.

## Zasady
- Nie edytuj pliku ręcznie. Źródło jest w repo `home-assistant-bibice`, katalog `panel/v3`.
  Zmieniaj tam, potem `npm run build && node tools/encrypt.mjs`, kopiuj tu TYLKO `.enc`.
- NIGDY nie dodawaj do tego repo jawnego `.js`, `.map`, źródeł ani zrzutów. Przed każdym
  commitem sprawdź `git diff --cached --stat`: ma być jeden plik `.enc` (albo README/GEMINI.md).
- Każdy commit z `.enc` to wydanie panelu. Wdrażaj tylko za zgodą Darka, z opisem po polsku.
- Dalsze kroki (pobranie, odszyfrowanie, podbicie `?v=<sha>`, kontrola sha16) są w `GEMINI.md`
  repo `home-assistant-bibice`, sekcja „Panel Ivellios v3”.