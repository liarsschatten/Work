# Einführung
	- Git ist ein Programm welches zur Versionierung verwendet wird.
		- Versionierung bedeutet das jede einzelne Version des Entwicklungsfortschritts behalten wird.
		- Des Weiteren werden alle Änderungen dokumentiert heißt es ist sofort ersichtlich was wann implementiert wurde.
		- Das sorgt dafür dass die Fehler leichter ersichtlich sind.
- # Erstellung
	- Globale Einstellungen
		- ```git
		  # Setze deinen Benutzernamen
		  git config --global user.name "Dein Name"
		  
		  # Setze deine E-Mail-Adresse
		  git config --global user.email "deine@email.com"
		  ```
	- Erstellen eines Lokalen Git Repositories
		- ```git
		  git init
		  ```
	- Man kann auch ein Remote Repository in ein lokales Repository klonen
		- ```git
		  git clone ""
		  ```
- # Staging Area
	- Die *Staging Area* ist der Bereich wo Dateien hervorgehoben werden welche in den nächsten Commit gehören.
		- Fügt alle Dateien der *Staging Area* hinzu.
			- ```git
			  gitgit add .
			  ```
		- Fügt eine ausgewählte Datei der *Staging Area* hinzu.
			- ```git
			  git add "File Name"
			  ```
		- **.gitignore**
			- Das ist eine Datei welche die Namen von Dateien und Ordner enthält die beim nächsten Commit ausgelassen werden.
- # Commit
	- ```git
	  git commit -m "Commit Kommentar"
	  ```
		- Dieser Befehl erstellt einen Commit
			- Ein Commit ist ein Punkt in der Versionshistorie zu dem man jederzeit zurückspringen kann
		- Ein Commit enthält:
			- Alle Änderungen die der *Staging Area* seit dem letzten Commit hinzugefügt wurden
			- Den Kommentar: Er sollte Kurz und Knapp alle Änderungen beschreiben
- # Branches
	- Ein Branch ist ein Abzweig vom Hauptcode in welchem man experimentieren kann ohne den Hauptcode zu beeinflussen.
	- Dieses Feature wird vor allem wichtig wenn man mit mehreren Personen an einem Projekt arbeitet.
	- ## Branch erstellen
		- Einen Branch erstellt man so
			- ```git
			  git branch Branchname
			  ```
		- Damit ist der Branch erstellt aber man ist noch nicht in ihn gewechselt das geht so
			- ```git
			  git checkout Branchname
			  ```
			- Dann kann man in dem Branch losarbeiten
	- ## Merge und Rebase
		- Wenn man dann das Feature fertig hat, will man das Feature wieder in den Main Branch einpflegen. Dafür nutzt man den Merge Befehl.
			- ```git
			  # bringt dich zurück in den Main Branch
			  git checkout main
			  
			  # das merged das neue Feature in den Main Branch
			  git merge neuesFeature
			  ```
		- Einen Rebase macht man dahingegen nur wenn man aufräumen will und sich sicher ist das man die Historie nicht mehr braucht.
			- ```git
			  git rebase
			  ```
	- ## Good Practices
		- Grundsätzlich gehört es sich für jedes Feature einen neuen Branch zu erstellen und diesen dann in den Main Branch zu mergen.
		- Das ist besonders wichtig wenn man zu mehreren arbeitet.
- # Remote Repository
	- Ein Remote Repository ist an sich nur eine Kopie des aktuellen Standes die woanders aufbewahrt wird.
	- ## Remote Hinzufügen
		- In diesem Schritt fügt man ein Remote Repository
			- ```git
			  git remote add link
			  ```
			- Danach fragt git nach dem Username da gibt man seinen Username an
			- Zuletzt will Git noch ein Passwort wichtig hier geht es nicht um das Account Passwort sondern um einen generierten Schlüssel
	- ## Push
		- Lädt alle Commits ins Remote Repository hoch
			- ```git
			  git push 
			  ```
			- Alternativ muss man hinter dem Push mit einem Leerzeichen getrennt das Repository angeben wenn man mehrere Repositories eingepflegt hat.
	- ## Fetch und Pull
		- Git Fetch zieht sich die gesamte Historie des Remote Repositories
			- ```git
			  git fetch 
			  ```
		- Git Pull zieht nur die Änderungen und Merged diese mit dem Lokalen Repository
			- ```git
			  git pull origin
			  ```
			- Das sorgt dafür dass die lokalen Änderungen erhalten bleiben.
-