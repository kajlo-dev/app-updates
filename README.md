# app-updates

Repo wyłącznie do dystrybucji aktualizacji aplikacji - jeden folder per aplikacja.

Każda aplikacja ma:
- `<aplikacja>/versioninfo.json` - `{ "versionCode": ..., "versionName": "...", "apkUrl": "..." }`, aktualizowany automatycznie przez CI danej aplikacji.
- Plik instalacyjny (np. APK) publikowany jako [Release](../../releases) o tagu `<aplikacja>` (nie commitowany do gita), nadpisywany (`--clobber`) przy każdym nowym buildzie - stąd stały adres pobierania.

## Aplikacje

- [moj-notesik](moj-notesik/versioninfo.json) - Mój Notesik (Android, Kotlin/Compose)
