# Dokumentenverwaltung

## Shell öffnen
In der Unix-Shell kann man Kommandos eintippen, die vom Computer ausgeführt werden. Die Shell ist `case-sensitive`. Das bedeutet, dass zwischen Groß-und Kleinschreibung unterschieden wird.

**Beispiel**: `Liste ≠ liste`

Kommandos in der Shell starten immer mit dem Prompt-Zeichen `$`.

## Verzeichnis

### Dateien und Verzeichnis auflisten
`ls` (list) listet Dateien im aktuellen Arbeitsverzeichnis auf
```
$ ls
```

```
$ ls -a
```
`ls -a` listet alle Dateien auf (auch unsichtbare, die mit einem `.` beginnen)

### Verzeichnis erstellen
Mit `mkdir` (make directory) kann man neue Verzeichnisse erstellen.

```
$ mkdir mein-ordner
```

Mit `ls` kann das Verzeichnis angezeigt werden

```r
$ ls
```

### Verzeichnis wechseln
Mit `cd` (change directory) kann man ein Verzeichnis wechseln

```
$ cd mein-ordner
```


### Verzeichnis "." und ".."
```
$ ls -a
```
gibt Verzeichnisse und Dateien wieder. Zwei besondere Verzeichnisse sind `.` und `..`.

* `.` ist das aktuelle Verzeichnis
* `..` ist das übergeordnete Verzeichnis


```
$ cd .
```
bedeutet, dass man im aktuellen Verzeichnis bleibt
```
$ cd ..
```
bedeutet, dass man sich in das nächsthöhere Verzeichnis (Elternverzeichnis) bewegt.

### Heimverzeichnis und Pfadnamen
`~` ist das Heimverzeichnis.

```
$ cd ~ 
```

`pwd` (print working directory) gibt an, in welchem Verzeichnis man sich gerade befindet
```
$ pwd 
```

### Zusammenfassung (I)

|  Befehl          |  Beschreibung                              |
| --------------   | ------------------------------------------ |
| `ls            ` | listet Dateien und Verzeichnisse auf	                |
| `ls -a         ` | listet alle  Dateien und Verzeichnisse auf	            |
| `mkdir         ` | erstellt ein Verzeichnis	                          |
| `cd directory`   | wechseln zu Verzeichnis `directory`	                 |
| `cd            ` | wechseln zu Heimverzeichnis	                  |
| `cd ~          ` | wechseln zu Heimverzeichnis	                  |
| `cd ..         ` | wechseln zu Elternverzeichnis	                |
| `pwd           ` | zeigt den Pfad zum aktuellen Verzeichnis an	 |


## Dateien 
### Dateien kopieren
`cp` (copy) kopiert eine Datei `datei1` in eine andere Datei namens `datei2`
```
$ cp datei1 datei2
```
### Dateien umbenennen / verschieben
`mv` (move) benennt Dateien um oder verschiebt sie

Umbenennen von `ha.txt` in `hausaufgaben.txt` :
```
$ mv ha.txt hausaufgaben.txt
```

Verschieben von `ha.txt` in das Verzeichnis `mathe`:

```
$ mv ha.txt mathe/ha.txt
```

### Dateien und Verzeichnis löschen
`rm` (remove) löscht Dateien vom System

```
$ rm hausaufgaben.txt
```

`rmdir` (remove directory) löscht Verzeichnisse vom System
```
$ rmdir mathe-ordner
```
### Dateien anzeigen
`clear` (clear screen) löscht den Inhalt vom Shell-Fenster

```
$ clear
```

`less` zeigt den Inhalt einer Datei an.

```
$ less hausaufgaben.txt
```
mit Taste [Leertaste] kann man scrollen, mit Taste [Q] kehrt man wieder zurück zur Shell.

### Zusammenfassung (II)

|  Befehl                 |  Beschreibung                                  |
| -------------------     | ---------------------------------------------- |
| `cp datei1 datei2    `  | kopiert `datei1` und nennt die Kopie `datei2`  |
| `mv datei1 datei2    `  | `datei1` zu `datei2` umbenennen oder verschieben   |
| `rm datei            `  | löscht eine Datei                              |
| `rmdir verzeichnis   `  | löscht ein Verzeichnis                         |
| `head datei          `  | zeigt die ersten Zeilen von `datei` an         |
| `tail file           `  | zeigt die letzten Zeilen von `datei` an        |
| `grep 'suchwort' datei` | sucht in `datei` nach `suchwort`               |
| `wc datei            `  | zählt Anzahl der Zeilen, Wörter, Zeichen in `datei` |
