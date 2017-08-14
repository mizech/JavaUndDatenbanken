# JAVA UND DATENBANKEN

Zertifikatsprüfung 

Java und Datenbanken - FernUniversität in Hagen

Klausur vom 25.03.2017

Klausurort Frankfurt

---------------------------------------------------------------------------

## Aufgabe 1:

Erläutern sie bitte den Zusammenhang zwischen der Programmiersprache Java,
JDBC/ODBC und SQL.

## Aufgabe 2:

Was versteht man unter Indizes in der Datenbankwelt?
Welche Vorteile bieten Sie?

Erläutern Sie bitte kurz.

## Aufgabe 3:

Um Datenbanken in Java-Anwendungen nutzten zu können, steht eine Vielzahl
von Datenbankmanagementsystemen (DBMS) zur Auswahl. Im Kurs haben Sie
drei gängige DBMS kennengelernt:

- MS Access
- MySQL
- Oracle

Worin unterscheiden sich diese drei Systeme bzw. was zeichnet sie jeweils aus?

## Aufgabe 4:

Vervollständigen Sie bitte den folgenden Quellcode:

```java
sql = "___ s.Thema, s.Beschreibung, v.Termin, v.Ort"
    + "___ Seminar s, Veranstaltungen v"
    + "___ s.SemNr = v.SemNr";
```

## Aufgabe 5:

Um Ergebnismengen von SQL-Anweisungen in Java verwalten zu können,
kommen Objekte vom Typ ResultSet zum Einsatz.
Nennen und erläutern Sie bitte zwei Methoden der Klasse ResultSet, um
Werte unterschiedlichen Typs von Ergebnismengen auslesen zu können.


## Aufgabe 6:

Das JDBC besteht, neben den in Aufgabe 5 erwähnten ResultSets, aus den vier
Komponenten Treiber (Driver), JDBC Driver Manager, Connection und 
Statement. Erläutern Sie bitte kurz, welche Aufgaben die einzelnen 
Komponenten in einem Java-Programm übernehmen:

1. Treiber (Driver):

2. JDBC Driver Manager:

3. Connection:

4. Statement:

## Aufgabe 7:

Was bewirkt das Schlüsselwort DISTINCT in SQL-Anweisungen?

## Aufgabe 8:

Vervollständigen Sie das folgende Beispiel so, dass alle Personen mit der
ID 10 gesucht werden.

```java
PreparedStatement pre_stmt = con.prepareStatement
("SELECT Namen FROM Teilnehmer WHERE VerID = ?)";

pre_stmt.setint(___,___)

prs_stmt.executeQuery();
```

## Aufgabe 9:

Was versteht man unter JavaBeans?
Warum werden Sie bei der Arbeit mit Datenbanken eingesetzt?

## Aufgabe 10:

Warum werden Daten XML-basiert gespeichert? Welche Vorteile ergeben sich
dadurch gegenüber der datenbankbasierten Speicherung?

## Aufgabe 11:

Angenommen, Sie haben eine Tabelle Kundenverwaltung mit den folgenden
Spalten:

|KNr|Vorname|Nachname|GebDatum|Ort|PLZ|Straße|
|---|-------|--------|--------|---|---|------|
|1  |Max    |Mustermann|01.01.1960|Ulm|12345|Musterstraße|
|2|Tina|Musterfrau| | | | |

Wie könnte ein XML-Dokument aussehen, in dem die Kundendaten dieser
Tabelle gespeichert sind? PLZ und Hausnummer sollen dabei als 
Attribute gespeichert werden. Alle anderen Kundendaten als Elemente.

Ergänzen Sie:

```xml
<?xml version="1.0" encoding="ISO-8859-1" ?>
<Kundenverwaltung>
</Kundenverwaltung>
```

Aufgabe 12:

Wie müssen Getter()- und Setter()-Methoden einer JavaBean-Klasse
aussehen, um Kundendaten aus der Tabelle Kundenverwaltung (siehe
Aufgabe 11) zu speichern, bzw. bereitzustellen?

Deklarieren Sie außerdem alle benötigten Variablen für die 
Methodenaufrufe.

``` java
public class Kunden {
	// Variablendeklarationen
	// Getter()- und Setter()-Methoden
}
```

-----------------------------------------------------------------------


