## NS Lookup (nslookup)
	- Nach dem Eingeben von nslookup kann man DNS Einträge suchen
		- Man kann nach folgenden Sachen suchen
			- Name eines Rechners
			- Name eines Rechners.*domain*
			- IPv4 Adresse eines Rechners
			- IPv6 Adresse eines Rechners
- ## CD
	- Der Befehl **cd (change directory)** wird verwendet, um das aktuelle Arbeitsverzeichnis zu ändern
- ## CD Syntax:
- ```cmd
  cd [/d] [<drive>:][<path>]
  cd [..]
  chdir [/d] [<drive>:][<path>]
  chdir [..]
  ```
-
- ## CD Parameter:
- |**Parameter**                     | **Description**| 
  |---------------------------|-----------------|
  | `/d`                            | Ändert das aktuelle Laufwerk, sowie das aktuelle Verzeichnis für ein Laufwerk|
  | `<drive>:`| Gibt Laufwerk an, angezeigt oder geändert soll, wenn es vom Laufwerk unterscheidet|
  |`<path>`| Gibt den Pfad zu dem Verzeichnis an, das Sie anzeigen oder ändern möchten|
  |`[...]`|Gibt an, dass Sie zum übergeordneten Ordner wechseln möchten.|
- ## CLS (Clear)
	- Löscht das Eingabeaufforderungsfenster
-
- ## DIR(Directory)
	- Zeigt eine Liste der Dateien und Unterverzeichnisse eines Verzeichnisses an
- ## Syntax:
	- ```cmd
	  dir [<drive>:][<path>][<filename>] [...] [/p] [/q] [/w] [/d] [/a[[:]<attributes>]
	  [/o[[:]<sortorder>]] [/t[[:]<timefield>]] [/s] [/b] [/l] [/n] [/x] [/c] [/4] [/r]
	  ```
- ## DIR Parameter:
- |**Parameter** | **Description**|
  |`[<drive>:]`| Gibt das Laufwerk an, für das eine Auflistung angezeigt werden soll|
  |`[<path>]`| Gibt das Verzeichnis an, für das eine Auflistung angezeigt werden soll|
  |`[<filename>]`|Gibt eine bestimmte Datei an, die für die Auflistung angezeigt werden soll|
  |`/p`| Zeigt jeweils einen Bildschirm der Auflistung an.|
  |`/p`| Zeigt Dateibesitzinformationen an.|
  |`/w`| Zeigt die Auflistung im breiten Format an|
  |`/d`| Zeigt die Liste im gleichen Format wie `/w` an, aber die Dateien sind nach Spalten sortiert|
  |`a[[:] <attributes>]`| Zeigt nur die Namen dieser Verzeichnisse und Dateien mit angegebenen Attributen an.
  **d** - Verzeichnisse
  **h** - Versteckte Dateien
  **s** - Systemdateien
  **I** - Punkte reparsieren
  **r** - Schreibgeschütze Dateien
  **a** - Dateien, die zur Archivierung bereit sind
  **i** - Nicht inhaltlich indizierte Dateien|
  
  |`/o[[:]<sortorder]`| Sortiert die Ausgabe nach sortorder, die eine beliebe Kombination der fehlenden Werte sein kann: 
  **n** - Alphabetisch nach Namen
  **e** - Alphabetische nach Erweiterung
  **g** - Gruppenverzeichnisse zuerst
  **s** - Nach Größe, kleinste zuerst
  **d** - Nach Datum/Uhrzeit, älteste zuerst|
-
- ## exit
	- Beendet den Befehlsinterpreter oder das aktuelle Batchskript
	- |**Parameter** | **Description**|
	  |`/b`| Beendet das aktuelle Batchskript|
	  |`<exitcode>`| Gibt eine numerische Zahl an.|
	-
- ## find
	- Sucht nach einer Textzeichenfolge in einer Datei oder Dateien und zeigt Textzeilen an, die die angegebenen Zeichenfolgen enthalten.
- ## find Syntax:
- ```cmd
  find [/v] [/c] [/n] [/i] [/off[line]] <"string"> [[<drive>:][<path>]<filename>[...]]
  ```
- ## find Parameter:
- |**Parameter**|**Description**|
  |`/v`| Zeigt alle Zeilen an, die nicht die angegebene `<string>` enthalten|
  |`/c`| Zählt die Zeilen, die die angegebene `<string>` enthalten, und zeigt die Summe an|
  |`/n`| Steht vor jeder Zeile mit der Zeilennummer der Datei.|
  |`/i`| Gibt an, dass bei der Suche die Groß-/Kleinschreibung nicht beachtet wird|
  |`/off[line]`| Überspringt keine Datei, für die der Offline-Attributsatz festgelegt ist|
  |`<"string">`| required. Gibt die Gruppe von Zeichen an, nach denen Sie suchen möchten|
  |`[<drive:>:] [<path>] <filename>`| Gibt den Speicherort und den Namen der Datei an, in der die Zeichenfolge gesucht wird|
-
- ## hostname
	- Zeigt den Hostnamenteil des vollständigen Computernamens an.
- ## hostname Syntax:
- ```cmd
  hostname
  ```
- ## pause
	- Hält die Verarbeitung eines Batchprogrammes an, zeigt die Eingabeaufforderung an.
- ## pause Syntax:
- ```cmd
  pause
  ```
- ## runas (Changed to Run as administrator)
	- Ermöglicht es einem Benutzer, bestimmte Tools und Programme mit anderen Berechtigungen als denen auszuführen, die die aktuelle Anmeldung des Benutzers bietet.
- ## runas Syntax:
- ```cmd
  runas [{/profile | /noprofile}] [/env] [{/netonly | /savecred}] [/smartcard]
  [/showtrustlevels] [/trustlevel] /user:<UserAccountName> "<ProgramName> <PathToProgramFile>"
  ```
- | **Parameter**      | **Description**                                                                 |
  |----------------|------------------------------------------------------------------------------|
  | `/profile`     | Lädt das Benutzerprofil                                                      |
  | `/noprofile`  | Gibt an, dass das Benutzerprofil nicht geladen werden soll                   |
  | `/env`         | Nutzt die aktuelle Netzwerkumgebung statt der lokalen Umgebung               |
  | `/netonly`     | Nur Remotezugriff                                                             |
  | `/savecred`    | Zeigt, ob Anmeldedaten gespeichert wurden                                   |
-
-
- ## shutdown
- ## sort
- ## taskkill
- ## tasklist
-
- # Netzwerk Befehle