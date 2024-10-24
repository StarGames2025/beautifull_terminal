# BeautifulTerminal

**BeautifulTerminal** ist eine Python-Bibliothek, die die Terminalausgabe automatisch verschönert, indem sie Farben basierend auf dem Inhalt der Nachrichten hinzufügt. Diese Bibliothek verbessert die Lesbarkeit deiner Konsolenanwendungen und macht es einfacher, Protokollausgaben und Nachrichten zu verstehen. Nach dem Import ist keine zusätzliche Einrichtung erforderlich!

## Funktionen

- **Automatische Farben**:
  - Fehler werden in Rot angezeigt.
  - Warnungen werden in Gelb angezeigt.
  - Erfolgsmeldungen werden in Grün angezeigt.
  - Normale Nachrichten werden in Weiß angezeigt.

- **Einfache Integration**:
  - Importiere einfach die Bibliothek, und sie funktioniert sofort.

- **Anpassbar**:
  - Du kannst die Farbcodes leicht ändern, um deinen Vorlieben gerecht zu werden.

## Installation

Um die Bibliothek zu installieren, verwende `pip`:

```bash
pip install beautifull_terminal
```

## Erste Schritte

Nach der Installation kannst du die Bibliothek schnell in deinen Python-Skripten verwenden. Folge diesen einfachen Schritten:

1. **Importiere die Bibliothek**:
   ```python
   import beautifull_terminal
   ```

2. **Gib Nachrichten aus**:
   Verwende die `print`-Funktion wie gewohnt. Die Bibliothek wendet automatisch die entsprechenden Farben basierend auf dem Inhalt deiner Nachrichten an.

## Verwendung

Hier sind einige Beispiele, wie man die Bibliothek verwendet:

```python
import beautifull_terminal

# Beispiele für die Verwendung der Bibliothek
print("Das ist eine normale Nachricht.")  # Standardfarbe: Weiß
print("Fehler: Etwas ist schiefgelaufen!", color="red")  # Fehlertext in Rot
print("Warnung: Sei vorsichtig!", color="yellow")  # Warnung in Gelb
print("Erfolg: Vorgang abgeschlossen!", color="green")  # Erfolg in Grün
```

### Ausgabe-Beispiele

- Normale Nachricht: Weiß
- Warnung: Gelb
- Fehler: Rot
- Erfolg: Grün

### Verwendung der `color`-Option

Die `print`-Funktion von `BeautifulTerminal` unterstützt eine optionale `color`-Parameter, mit dem du die Farbe des ausgegebenen Texts direkt angeben kannst. Beispiel:

```python
import beautifull_terminal

print("Dieser Text ist normal.")  # Standardfarbe: Weiß
print("Dieser Text ist rot!", color="red")  # Text in Rot
print("Dieser Text ist gelb!", color="yellow")  # Text in Gelb
print("Dieser Text ist grün!", color="green")  # Text in Grün
```

Wenn du eine ungültige Farbe angibst, wird die Standardfarbe verwendet. Dies gibt dir die Flexibilität, den Text nach deinen Wünschen zu gestalten.

## Anpassung

Du kannst die Farbcodes in der Bibliothek ändern, um das Erscheinungsbild der Ausgaben zu verändern. Dies ermöglicht es dir, die Bibliothek an dein bevorzugtes Terminal-Design oder persönliche Vorlieben anzupassen. Ändere einfach das `COLORS`-Dictionary in der `BeautifulTerminal`-Klasse.

## Deaktivierung

Wenn du die Farbausgabe vorübergehend deaktivieren musst, kannst du dies tun:

```python
import beautifull_terminal as bt
bt.disable()  # Farbausgabe vorübergehend deaktivieren
```

Um die Farbausgabe wieder zu aktivieren:

```python
bt.enable()  # Farbausgabe wieder aktivieren
```

## Kompatibilität

Die `BeautifulTerminal`-Bibliothek ist mit jedem Terminal kompatibel, das ANSI-Escape-Codes unterstützt, was die meisten modernen Terminal-Emulatoren umfasst. Sie funktioniert jedoch möglicherweise nicht korrekt auf älteren Systemen oder in Umgebungen, die ANSI-Codes nicht unterstützen.

## Danksagungen

- Diese Bibliothek wurde von dem Bedarf an besserer Lesbarkeit der Terminalausgaben inspiriert.
- Besonderer Dank geht an die Mitwirkenden und die Open-Source-Community für ihre kontinuierliche Unterstützung und Vorschläge.

## Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert. Siehe die [LICENSE](LICENSE) Datei für weitere Details.

## Beiträge

Beiträge sind willkommen! Wenn du Vorschläge für Verbesserungen oder zusätzliche Funktionen hast, zögere nicht, ein Problem zu eröffnen oder einen Pull-Request einzureichen.

## Kontakt

Für Fragen oder Feedback wende dich bitte über das [GitHub-Repository](https://github.com/StarGames2025/beautifull_terminal) an uns.