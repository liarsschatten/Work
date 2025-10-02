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
- ## find
- ## hostname
- ## pause
- ## runas
- ## shutdown
- ## sort
- ## taskkill
- ## tasklist
-
- # Netzwerk Befehle