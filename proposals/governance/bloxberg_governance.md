# Governance Modell (draft)

## Übersicht

Das Governance Modell beruht auf drei Säulen:

1. **Mitbestimmungsrechte**

   * Verwaltungsrechte: neue Proposals vorschlagen, Entscheidungen durchführen oder umsetzen

   * Kontrollrechte: Ratifizierung der Entscheidungen, dem Entscheidungsprozess und desen Performance folgen
 
2. **Verantwortung**: Die Mechanismen, wodurch sich die Mitglieder verpflichten und für deren Aktionen und Entscheidungen verantwortlich gemacht werden.

3. **Anreize**: Alle Gründe und Mechanismen, wodurch die Mitglieder aufgefordert werden, sich an die Richtlinien zu halten

Um Änderungen im Governance Modell vorzunehmen wird ein Quorum von 75% oder mindestens 7 Organisationen benötigt. Die Wahl findet off-chain statt, typischerweise während des Summits. Eine Änderungsantrag muss über 75% der Stimmen erhalten zu haben um in Kraft zu treten.


## Mitbestimmungsrechte

Um ein Mitglied zu werden, die Organisation muss folgende Kriterien erfüllen:
* die Organisation muss z.B. in Forschungsbereich tätig sein
* durch die Mitglieder mehrheitlich abgestimmt worden sein
 
Alle Mitglieder haben das Recht, eine off- oder on-chain Veranstaltung zu initiiren.

### Entscheidungsalgorithmus

Der Entscheidungsalgorithmus hat das Ziel, die Mitglieder zu motivieren, sich an deren Aufgaben zu halten, so wie sie im Governance Model definiert sind.

Alle Gründungsmitglieder starten mit einem Stimmgewicht von 100, während die neuen Mitglider bei 0 starten.

Eine über ein Proposal abgegebene Stimme erhöht das Stimmgewicht, d.h.

~~~
stimmgewicht = stimmgewicht + 100 / (Anzahl der Proposals im Monat)
~~~
während ein verpasste Proposal verringert das Stimmgewicht, d.h.

~~~
stimmgewicht = stimmgewicht - 100 / (Anzahl der Proposals im Monat)
~~~

### Neue Mitglieder

Neue Mitglieder werden jeden Monat (oder alle 4 Wochen) von Iron Throne zur Wahl gestellt. Die Organisation muss vorher einen Formular ausfüllen, um seine Kandidatur zu beantragen.

Die Wahl findet on-chain statt. Um die Wahl zu ratifizieren, ein Quorum von 50% der gesamten Stimmgewichte muss vorhanden sein oder mindestens 3 abstimmende Mitglieder.

Falls der Kandidat über 50% der Stimme erhalten hat, wird er angewiesen, einen eigenen Knoten zu erstellen, der von Iron Throne ins Netzwerk aufgenommen wird.

### Iron Throne

Ein Konsortiumsmitglied hat das Iron Throne für ein Jahr. Währenddessen hat er die Aufgabe hat, die Ergebnisse der Wahlen umzusetzen, bzw. neue Mitglieder hinzuzufügen oder Mitglieder zu entfernen.

Der Iron Thron Mitglied organisert das Summit, ein physisches Treffen, wo sich alle Mitglieder treffen und evtl. Entscheidungen fällen.

Die Wahl zu Iron Throne braucht ein Quorum von über 75% der Mitglieder oder mindestens 3 Organisationen. Die Wahl findet off-chain statt, bzw. während des Summits. Die Organisation mit über 50% der Stimmen wird die neue Iron Throne Besitzerin.


## Verantwortung
Strafen können den Mitgliedern verhängt werden, die sich nicht an das Governance halten. Der Ausschluss eines Mitglieds muss von den anderen Mitglieder durch Wahl zugestimmt werden.

Strafen können durch folgende Aktionen ausgelöst werden:
* Knoten ist für mehr als 3 Monaten offline
* Knoten spamt das Netzwerk
* der Mitglied hält sich nicht an das Governance-Modell
* der Mitglied muss dem Manifesto zustimmen

Der Ausschluss eines Mitglieds erfolgt off-chain und folgt dem Entscheidungsalgorithmus. Ein Quorum von 75% wird bei der Wahl benötigt oder mindestens 7 Organisationen. Wenn über 75% der Stimmen für den Ausschluss fallen, muss der Iron Thron den betroffenen Knoten aus dem Netzwerk entfernen.

Falls es zu der Situation kommt, dass der Besitzer des Iron Throne seinen Status nach einer Iron Throne Abstimmung nicht abgeben will, wird das Netzwerk geforked. 


## Anreize
Die Netzwerk-Mitgliedschaft bringt folgende Vorteile mit sich:

* die mächtige Netzwerk Infrastruktur in Anspruch zu nehmen
* ein enger und dezentralisierter Austausch mit anderen Organisationen
* Mitglieder sind in dem Entscheidungsprozess mitbeteiligt
