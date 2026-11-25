# GEMINI.md: ivellios-panel

To repo jest publiczne. Nie wpisuj tu żadnych tokenów, adresów prywatnych, haseł ani
konfiguracji domu.

## Co tu jest
Tylko zbudowany plik `ivellios-panel-v3.js` (panel Home Assistant, Lit 3), pobierany do HA
przez `downloader.download_file` z adresu raw GitHuba, przypiętego do SHA commita.

## Zasady
- Nie edytuj tego pliku ręcznie. Źródło jest w repo `home-assistant-bibice`, katalog
  `panel/v3`. Zmieniaj tam, buduj (`npm run build`), kopiuj wynik tutaj.
- Każdy commit tutaj to wydanie panelu. Wdrażaj tylko za zgodą Darka, z opisem po polsku, co
  się zmieniło w wyglądzie lub działaniu.
- Po commicie zapisz SHA. Dopiero z tym SHA robisz pobranie w HA i podbicie `?v=<sha>` w
  zasobie dashboardu (opis kroków w `GEMINI.md` repo `home-assistant-bibice`).
- Nie pushuj niczego poza zbudowanym plikiem i ewentualnym README.
