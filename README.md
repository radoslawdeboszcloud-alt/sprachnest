# Sprachnest und mehr – strona wizytówka

Pierwsza wersja statycznej strony wizytówki inspirowana układem radoIT (one-page),
zawierająca przykładowe treści oraz logo marki.

## Co zawiera obecna wersja

- jasny motyw oparty o kolory z logo,
- logo osadzone w lewym górnym rogu,
- sekcje: hero, o nas, oferta, kontakt,
- przełącznik języka PL / DE.

## Podgląd lokalny

```bash
python3 -m http.server 4173
```

Następnie otwórz: `http://localhost:4173`

## Publikacja publicznie na GitHub Pages

Repo ma gotowy workflow: `.github/workflows/deploy-pages.yml`, który publikuje stronę automatycznie.

### Co trzeba zrobić na GitHub (jednorazowo)

1. Wgraj to repo na GitHub (push).
2. Ustaw repo na **Public**:
   - `Settings` → `General` → `Danger Zone` → `Change repository visibility` → **Make public**.
3. Włącz Pages z GitHub Actions:
   - `Settings` → `Pages` → `Build and deployment` → `Source: GitHub Actions`.
4. Wypchnij commit do gałęzi `main` (albo `work`).
5. Po kilku minutach strona będzie pod adresem:
   - `https://<twoj-login>.github.io/<nazwa-repozytorium>/`

## Krok 2 (plan)

W pliku `formularz-template.txt` jest szablon, który klient może wypełnić.
W kolejnym etapie podmienimy przykładowe treści na dane z formularza.
