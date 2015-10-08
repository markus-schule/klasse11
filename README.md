# Dokumentenverwaltung

## Shell öffnen
In der Unix-Shell kann man Kommandos eintippen, die vom Computer ausgeführt werden.

## Verzeichnis

### Dateien und Verzeichnis auflisten
`ls (list)` listet Dateien im aktuellen Arbeitsverzeichnis auf

```
$ ls [Enter]
```

```
$ ls -a
```
`ls -a` listet alle Dateien auf (auch unsichtbare, die mit einem `.` beginnen)

### Verzeichnis erstellen
Mit `mkdir (make directory)` kann man neue Verzeichnisse erstellen.

```
$ mkdir mein-ordner
```

Mit `ls` kann das Verzeichnis angezeigt werden

```
$ ls
```

### Verzeichnis wechseln
Mit `cd (change directory)` kann man ein Verzeichnis wechseln

```
$ cd mein-ordner
```


### Verzeichnis . und ..
```
$ ls -a
```
gibt Verzeichnisse und Dateien wieder. Zwei besondere Verzeichnisse sind `(.)` und `(..)`
(.) ist das aktuelle Verzeichnis
(..) ist das übergeordnete Verzeichnis


```
$ cd .
```
bedeutet, dass man im aktuellen Verzeichnis bleibt
```
$ cd ..
```
bedeutet, dass man sich in das nächsthöhere Verzeichnis bewegt.

### Heimverzeichnis und Pfadnamen
`~` ist das Heimverzeichnis.

```
$ cd ~ 
```

`pwd (print working directory)` gibt an, in welchem Verzeichnis man sich gerade befindet
```
$ pwd 
```

### Zusammenfassung

|  Befehl        |  Beschreibung                              |
| -------------- | ------------------------------------------ |
| ls             | list files and directories	                |
| ls -a          | list all files and directories	            |
| mkdir          | make a directory	                          |
| cd `directory` | change to named directory	                 |
| cd             | change to home directory	                  |
| cd ~           | change to home directory	                  |
| cd ..          | change to parent directory	                |
| pwd            | display the path of the current directory	 |


## Dateien 
### Dateien kopieren
`cp (copy)` kopiert eine Datei `file1` in eine andere Datei namens `file2`
```
$ cp file1 file2
```
### Dateien umbenennen / verschieben
`mv (move)` benennt Dateien um oder verschiebt sie

Umbenennen:
```
$ mv ha.txt hausaufgaben.txt
```

Verschieben von `ha.txt` in das Verzeichnis `mathe`:

```
$ mv ha.txt mathe/ha.txt
```

### Dateien und Verzeichnis löschen
`rm (remove)` löscht Dateien vom System

```
$ rm hausaufgaben.txt
```

`rmdir (remove directory)` löscht Verzeichnisse vom System
```
$ rmdir mathe-ordner
```
### Dateien anzeigen
`clear (clear screen)` löscht den Inhalt vom Shell-Fenster

```
$ clear
```

`less` zeigt den Inhalt einer Datei an.

```
$ less hausaufgaben.txt
```
mit Taste [Leertaste] kann man scrollen, mit Taste [Q] kehrt man wieder zurück zur Shell.

### Zusammenfassung

|  Befehl             |  Beschreibung                                  |
| ------------------- | ---------------------------------------------- |
| cp file1 file2      | copy file1 and call it file2                   |
| mv file1 file2      | move or rename file1 to file2                  |
| rm file             | remove a file                                  |
| rmdir directory     | remove a directory                             |
| head file           | display the first few lines of a file          |
| tail file           | display the last few lines of a file           |
| grep 'keyword' file | search a file for keywords                     |
| wc file             | count number of lines/words/characters in file |
|                     |                                                |
