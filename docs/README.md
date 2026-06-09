# Aufgabe 2: Information Retrieval Decision Support

## Design Mockup 
<img width="2539" height="1237" alt="image" src="https://github.com/user-attachments/assets/0da2bb28-9900-4c9d-9d74-695a052331ac" />

## Live Test der Search Machine

[MedInfo](https://chbo70.github.io/medical-search-engine/#gsc.tab=0&gsc.sort=)

## Übersicht der Datenquellen

Da wir die Suchmaschine für PatientInnen, bzw. Personen mit nicht medizinischem Fachwissen, ausgelegt haben, beinhalten die Quellen dementsprechend leicht verständliche Informationen. Die meisten Websites die hinzugefügt wurden beinhalten klassische Reiter wie Krankheiten, Symptome, Diagnose, etc. wo mit möglichst einfachen Termen eine Thema erklärt wird. Wir haben zwei Websites, afgis[^1] und einen Meduni-Wien Blog[^2] gefunden, die einen Überblick über Websites mit medizinisches Wissen geben. Diese haben viele Websites aufgelistet und evaluiert. Wir sind dann alle durchgegangen und haben uns die mit den meisten Informationen herausgeschrieben und in die Google Programmable Search Engine eingetragen.

## Generelle Überlegung basierend auf Web/Literatur-Recherche

### Was macht die ideale medizinische Suchmaschine aus?

Die ideale Suchmaschine fungiert wie ein digitaler, kompetenter Assistenzarzt. Die Datenbasis sollte sich ausschließlich aus verifizierten Quellen zusammensetzen. Medizinische Suchen sind oft angstgetrieben. Die Sprache sollte daher beruhigend, sachlich und frei von unnötigem Fachbegriffen sein. Alle Ergebnisse sollten mit einer seriösen, bekannten Quelle verknüpft sein, damit Vertrauen entsteht.

### Wie kommen User schnell zu hochqualitativen Antworten?

Um ein besseres Ergebnis zu ermöglichen, sollte die Suchmaschine mehr als nur ein einfaches auflisten von Links enthalten. So könnten beispielsweise bei Fragen ein Symptom Checker dynamisch nachfragen, was für Beschwerden da sind. Es ist ebenfalls wichtig, dass die Suchmaschine von einer Umschreibungen des Problems auf den medizinischen Fachbegriff kommt.

### Für welche Personengruppen sollen solche Tools verfügbar gemacht werden, und wie?

Prinzipiell sollte so ein Tool allen Menschen zugänglich sein, muss aber für spezifische Gruppen angepasst werden. So wollen meist jüngere Leute eine schnelle knappe Antwort um sich einen Überblick zu verschaffen mit der Möglichkeit auch eine tiefere Erklärung zu bekommen. Für ältere Menschen ist ein Benutzerfreundliches Design sehr wichtig. Es sollte große Texte und leichte Navigation ermöglichen, evtl. auch eine Vorlesefunktion. Für Sprachbarrieren eignet sich heutzutage eine KI, die die Ergebnisse in die Zielsprache umwandeln kann. Aber auch für Ärzte oder medizinisches Personal kann eine Suchmaschine von Vorteil sein. Diese beinhaltet dann mehr Fachbegriffe und verweist auf tiefgreifende Studien.

### Wie würde die Suchmaschine am besten verfügbar gemacht?

So wie in der letzten Aufgabe eignet sich eine API die man an alle möglichen Schnittstellen anbinden kann, am besten. Auch hier ist kommt es auf die Personengruppen an. So eignet sich für die schnelle Suche bei jungen Menschen der Browser. Der ist schnell erreicht und kann mit einem evtl. umschalten in einen medizinischen Modus gezielt die API verwenden. Bei älteren Personen eignet sich eine App besser, die schön strukturiert ist, Ergebnisse speichern kann, um das Wiederfinden von chronischen Krankheiten zu erleichtern. Für Ärzte und medizinisches Personal eignet sich eine Integration in einem bereits bestehenden KIS oder EHR, um spezifische Information zum offenen Tab zu bekommen.

## Evaluierung

### 5 Fragen

**1. bluthochdruck senken ohne medikamente was hilft wirklich**
- Ergebnis 1:
	- Ja, liefet erwartete Suchergebnis, fast gleiche Überschrift
- Ergebnis 2:
	- Ja, liefet erwartete Suchergebnis
- Ergebnis 3:
	- Ja, liefet erwartete Suchergebnis

| Typ | Ergebnis 1 | Ergebnis 2 | Ergebnis 3 | 
|-----------------|--------|--------|--------|
| Authority | Ja | Ja | Ja | 
| Complementarity | Nein | Ja | Ja | 
| Confidentiality | Ja | Ja | Ja| 
| Attributon | Ja | Ja | Ja | 
| Justifiability | Ja | Ja | Ja | 
| Transparency | Ja | Ja | Ja | 
| Financial <br/>Disclosure | Ja | Ja | Ja | 
| Advertisment <br/>Policy | Ja | Ja | Ja |


**2. herzschwäche woran erkenne ich dass es schlimmer wird**
-   Ergebnis 1:
    -   Ja, liefet erwartete Suchergebnis
-   Ergebnis 2:
    -   Nein, wechselt zur Herzrythmusstörungen
-   Ergebnis 3:
    -   Ja, liefet erwartete Suchergebnis

| Typ | Ergebnis 1 | Ergebnis 2 | Ergebnis 3 | 
|-----------------|--------|--------|--------|
| Authority | Ja | Ja | Ja | 
| Complementarity | Nein | Ja | Nein | 
| Confidentiality | Ja | Ja | Ja | 
| Attributon | Ja | Ja | Ja | 
| Justifiability | Ja | Ja | Ja | 
| Transparency | Ja | Ja | Ja | 
| Financial <br/>Disclosure | Ja | Ja | Ja | 
| Advertisment <br/>Policy | Ja | Ja | Ja |

**3. was bedeutet ein erhöhter cholesterin wert im blutbild**
-   Ergebnis 1:
    -   Ja, liefet erwartete Suchergebnis
-   Ergebnis 2:
    -   Ja, liefet erwartete Suchergebnis
-   Ergebnis 3:
    -   Ja, liefet erwartete Suchergebnis

| Typ | Ergebnis 1 | Ergebnis 2 | Ergebnis 3 | 
|-----------------|--------|--------|--------|
| Authority | Ja | Ja | Ja | 
| Complementarity | Ja | Nein | Ja | 
| Confidentiality | Ja | Ja | Ja| 
| Attributon | Ja | Ja | Ja | 
| Justifiability | Ja | Ja | Ja | 
| Transparency | Ja | Ja | Ja | 
| Financial <br/>Disclosure | Ja | Ja | Ja | 
| Advertisment <br/>Policy | Ja | Ja | Ja |


**4. krämpfe und atemnot nach einen langem flug gefährlich**
- Ergebnis 1:
	- Trifft nicht wirklich das gewünschte Ergebnis
- Ergebnis 2:
	- Nein, es kommt nicht mal das Wort Flug vor
- Ergebnis 3:
	- Nein, es handelt sich um eine Tauchkrankheit

| Typ | Ergebnis 1 | Ergebnis 2 | Ergebnis 3 |
|-----------------|--------|--------|--------|
| Authority 			| Ja | Ja | Ja |
| Complementarity | Nein | Nein | Nein |
| Confidentiality | Ja | Ja | Ja |
| Attributon			| Ja | Ja | Ja |
| Justifiability	| Ja | Ja | Ja |
| Transparency 		| Ja | Ja | Ja |
| Financial <br/>Disclosure	| Ja | Ja | Ja |
| Advertisment <br/>Policy 	| Ja | Ja | Ja |

**5. kribbeln auf der lippe bei früchte**
- Ergebnis 1:
	- Ja, liefet brauchbares Ergebnis
- Ergebnis 2:
	- Nein, handelt zumindest von Lippen
- Ergebnis 3:
	- Nein, ist was ganz anderes

| Typ | Ergebnis 1 | Ergebnis 2 | Ergebnis 3 |
|-----------------|--------|--------|--------|
| Authority 			| Ja | Ja | Ja |
| Complementarity | Nein | Nein | Nein |
| Confidentiality | Ja | Ja | Ja |
| Attributon			| Ja | Ja | Ja |
| Justifiability	| Ja | Ja | Ja |
| Transparency 		| Ja | Ja | Ja |
| Financial <br/>Disclosure	| Ja | Ja | Ja |
| Advertisment <br/>Policy 	| Ja | Ja | Ja |

**Anmerkungen:**
- Viele Ergebnisse kamen immer von den gleichen Quellen obwohl 14 Unterschiedliche hinzugefügt wurden. Da ist die Frage welchen Grund das genau hat.
- Manche Punkte waren auf der initialen Seite nicht klar ersichtlich oder wir waren uns nicht ganz sicher ob alle Punkte erfüllt wurden, wurden aber von uns trotzdem als Ja eingestufft.

### Eigene Überlegungen
Man könnte die ersten 3 Ergebnisse statt einer Binären Klassifizierung mittels einem Gradienten von 0-2 einstufen, um eine genauere Aussage zu bekommen. Zusätzlich könnte man dieses auf zB. 10 Anfragen erweitern und herausfinden ob die besten 3 Antworten wirklich oben stehen. Dazu würde noch dazukommen manuell zu überprüfen ob die Suchmaschine auch wirklich alle wichtigen Dokumente findet oder manche durch andere Formulierungen übersieht. Daher sollte auch auf Vokabular & Ontologien geprüft werden, da diese im medizinischen Kontext ein deutlich akkurateres Ergebnis liefern. Die Qualität ist sehr wichtig und muss mit bestehenden Leitlinien oder Studien abgedeckt sein. Da spielt das Schadenspotential so wie die Verständlichkeit, Stichwort Personengruppen, auch eine große Rolle. Um komplett sicherzugehen wie genau die Ergebnisse der Suchmaschine sind braucht es medizinisches Fachpersonal zum Prüfen von komplexen Anfragen.

## Arbeitsaufteilung
- Niklas Kasper, 12122377:
	- Programmable Search Engine online erstellt
 	- Theoretische Fragen beantwortet
  	- Evaluierung der Testfragen gemeinsam  
- Boon-Chung Chi, 12118081:
	- Design-Mockup
 	- Prototyp mit SearchEngine von Google und auf Github bereitgestellt
  	- Evaluierung der Testfragen gemeinsam  	




[^1]: https://www.afgis.de/
[^2]: https://ub.meduniwien.ac.at/blog/?p=175
