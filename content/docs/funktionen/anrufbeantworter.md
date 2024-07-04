---
title: "Anrufbeantworter (Voicemail)"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "funktionen"
weight: 406
toc: true
---

Um die Erreichbarkeit zu erhöhen, kann jede Nebenstelle oder Gruppe Ihrer Cloud PBX einen Anrufbeantworter (Voicemail) nutzen. Damit besteht die Möglichkeit, Anrufer im Besetztfall, außerhalb der Bürozeiten oder während der Betriebsferien mit Sprachnachrichten entsprechend zu informieren. Anschließend kann der Anrufer Ihnen eine Nachricht auf Ihren Anrufbeantworter sprechen, die Sie zu einem späteren Zeitpunkt abhören können. Diese Nachricht können Sie auch per E-Mail zugeschickt bekommen.

## 1.	Informationen zu Sprachnachrichten und Ordnern
Mit einer Sprachnachricht kann dem Anrufer zum einen mitgeteilt werden, dass sein Anruf nicht persönlich entgegengenommen wird. Zum anderen können Sie ihm weiterführende Informationen zukommen lassen, wie z. B. wann Sie wieder verfügbar sind, wie er Sie per E-Mail kontaktieren kann oder wie er zusätzliche Unterstützung erhält. Dabei wird unterschieden: <br>

### a) Nicht-verfügbar-Nachricht (Abwesenheitsansage)
Die „Nicht verfügbar-Nachricht“ ist die Standard-Begrüßung. Sie wird verwendet, wenn Sie den Anruf nicht entgegennehmen und der Anruf an Ihre Voicemail weitergeleitet wird. Wenn Sie nichts aufgezeichnet haben, spielt das Telefonsystem die gewählten Ziffern (des Anschlusses) mit dem Zusatz „ist nicht verfügbar“ ab.
Wenn Sie statt der „Nicht-verfügbar-Nachricht“ zur Begrüßung Ihren Namen, z.B. „Peter Schneider“ aufgezeichnet haben, gibt das System die Nachricht „Peter Schneider ist nicht verfügbar“ wieder. <br>

### b) Besetzt-Nachricht
Wenn Sie möchten, können Sie eine benutzerdefinierte Besetzt-Begrüßung aufzeichnen. Diese wird verwendet, wenn jemand Sie anruft und Sie gerade telefonieren. Wenn Sie nichts aufgezeichnet haben, gibt das System die gewählten Ziffern (des Anschlusses) mit dem Zusatz „ist besetzt“ wieder.
Wenn Sie statt der „Besetzt-Begrüßung“ Ihren Namen, z.B. „Petra Schmitz“ aufgezeichnet haben, spielt das System diese Nachricht ab: „Petra Schmitz ist besetzt.“ <br>

### c) Vorübergehende Begrüßung
Sie können auch eine temporäre Begrüßung aufzeichnen. Wenn diese vorhanden ist, wird sie anstelle Ihrer „Nicht-verfügbar- oder Besetzt-Begrüßung“ abgespielt. Dies kann zum Beispiel genutzt werden, wenn Sie in Urlaub fahren oder für eine Weile nicht im Büro sind und Anrufer informieren möchten, dass Sie in absehbarer Zeit nicht mit einem Rückruf rechnen können. <br>

Mit dem Voicemail-System können Sie Ihre Nachrichten speichern und in Ordnern organisieren. Die Standard-Ordnerliste umfasst:

* 0 - Neue Nachrichten
* 1 - Alte Nachrichten
* 2 - Arbeits-Nachrichten
* 3 - Familien-Nachrichten
* 4 - Freunde-Nachrichten

Wenn ein Anrufer eine Nachricht für Sie hinterlässt, legt das System die Nachricht im Ordner „Neue Nachrichten“ ab. Wenn Sie die Nachricht abhören, aber die Nachricht nicht löschen oder in einem anderen Ordner speichern, wird die Nachricht automatisch in den Ordner „Alte Nachrichten“ verschoben. <br>
Wenn Sie sich zum ersten Mal bei Ihrer Mailbox anmelden, macht das Voicemail-System den Ordner „Neue Nachrichten“ zum aktuellen Ordner, wenn Sie neue Nachrichten haben. <br>
Wenn Sie keine neuen Nachrichten haben, wird der Ordner „Alte Nachrichten“ zum aktuellen Ordner. <br>

## 2.	Individualisierung der Voicemail

Für das Customizing gibt es zwei Möglichkeiten.

### a.)	Administration über das Web-Interface
Klicken Sie zunächst auf den Menüpunkt Kunden-Details, dann auf Subscriber und bei der betreffenden Nebenstelle oder Gruppe auf Einstellungen. Öffnen Sie nun das Menü „Voicemail and Voicebox“:

![Voicemail and Voicebox 1](https://user-images.githubusercontent.com/98753538/193989352-c4110eb4-41b1-4817-bf1f-8af67b5287f5.jpg)

Mit Hilfe der Schaltfläche „Edit“ (in der letzten Spalte, s. Pfeil) können Sie: <br>
Den PIN ändern (1),  <br>
Ihre E-Mail-Adresse zur Benachrichtigung hinterlegen (2),  <br>
die Option zum Löschen (der Nachricht nach E-Mail-Versand) aktivieren (3) und  <br>
auswählen, dass aufgezeichnete Sprachnachrichten als WAV-Datei an die E-Mail angehängt werden (4).  <br>

Mit den Punkten 5 bis 8 konfigurieren Sie die unterschiedlichen Ansagen, die Anrufer zu hören bekommen: <br>
„Nicht-verfügbar- oder Abwesenheitsanzeige“ (5), <br>
Ansage bei „Besetzt“ (6) und  <br>
die Temporäre Ansage (7). Ist diese konfiguriert, setzt sie die anderen Ansagen außer Kraft. <br>
Außerdem können Sie Ihren Namen aufsprechen (8). Dann hören ihn Anrufer anstatt Ihrer Telefonnummer. <br>

Zur Erzeugung einer elektronischen Ansage im wav-Format gehen Sie bitte folgendermaßen vor:  <br>
Suchen Sie im Internet mit "text to speech german kostenlos". Bei den Ergebnissen finden Sie leicht einen (kostenlosen) Text-zu-Sprache-Generator wie z.B. ttsfree, freetts oder ttsmp3. Dort können Sie Ihren gewünschten Ansagetext eingeben, wählen die Sprache und Stimme für die Ausgabe und erzeugen so eine mp3-Datei. Um diese in der Cloud-PBX verwenden zu können, ist noch eine Wandlung ins WAV-Format erforderlich. Entsprechende Konverter sind im Internet mit "mp3 wav converter" ebenfalls leicht zu finden. Wichtig: In Mono und nach a-Law konvertieren. <br>
Sie können die elektronischen Ansagen im Menü „Anrufeinstellungen“ unter „Anrufbeantworter“ hochladen und wieder entfernen:  <br>

![Anrufbeantworter2](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/f085e914-42ef-4780-8565-d7fb89560ac5)


Zur Erinnerung: Wenn Sie als Administrator angemeldet sind, steht Ihnen der (zusätzliche) Menüpunkt „Kunden-Details“ zur Verfügung. Auch von hier aus gelangen Sie zu den „Subscribern“ und können dort „Einstellungen“ und den Menüpunkt „Voicemail and Voicebox“ auswählen bzw. öffen:  <br>

![Voicemail Ansagen2](https://user-images.githubusercontent.com/98753538/193989610-cfa67140-24e2-4752-a160-a337a9ff319f.jpg)

Ist die entsprechende Ansage bereits vorhanden, können Sie diese herunterladen, löschen oder mit dem Button „Edit“ eine neue laden.

### b.)	Tastatur des Endgerätes
Mit Drücken der Taste „Briefumschlag“ (bei Yealink-Telefonen) oder Tastenwahl der Ziffern 2 0 0 0 gelangen Sie in das Sprachbox-Menü der Cloud-PBX. Dieses ist folgendermaßen aufgebaut: „Drücken Sie... <br>

*	...die '1' für alte/neue Nachrichten.“ <br>
    *	„Für erweiterte Optionen" '3' drücken. <br>
        * ...die '3', um die Tonmitteilung Nachrichten zu hören.“ <br>
        * ...'*', um ins Hauptmenü zu kommen.“ <br>
    *	...die '4', um zur vorherigen Nachricht zu gelangen.“ <br>
    *	...die '5', um die aktuelle Nachricht zu wiederholen.“ <br>
    *	...die '6', um die nächste Nachricht abzuspielen.“ <br>
    *	...die '7', um die aktuelle Nachricht zu löschen.“ <br>
    *	'9', um diese Nachricht in einem Ordner zu speichern und <br>
        * '0' für Neue Nachrichten." <br>
        * '1' für Alte Nachrichten." <br>
        * '2' für Arbeits-Nachrichten." <br>
        * '3' für Familien-Nachrichten." <br>
        * '4' für Freunde-Nachrichten." <br>
        * '#', um abzubrechen. <br>
* ...die '2', wenn Sie den Ordner wechseln wollen und <br>
    *	'0' für Neue Nachrichten.“ <br>
    *	'1' für Alte Nachrichten.“ <br>
    *	'2' für Arbeits-Nachrichten.“ <br>
    *	'3' für Familien-Nachrichten.“ <br>
    *	'4' für Freunde-Nachrichten.“ <br>
    *	'#', um abzubrechen.“ <br>
*	...die '3', um zu den erweiterten Optionen zu gelangen.“ <br>
    *	'\*', um zum Hauptmenü zurückzukehren.“ <br>
*	...die '0', um zu den Mailboxoptionen zu gelangen.“ <br>
    *	'1', wenn Sie Ihre Abwesenheitsansage aufzeichnen wollen." <br>
        * '1' Akzeptieren <br>
        * '2' Hören Sie es sich an <br>
        * '3' Neu aufnehmen <br>
    * '2', um Ihre Besetztansage aufzuzeichnen." <br>
        *	'1' Akzeptieren <br>
        *	'2' Hören Sie es sich an <br>
        *	'3' Neu aufnehmen <br>
    * '3', um Ihren Namen aufzuzeichnen." <br>
        *	'1' Akzeptieren <br>
        *	'2' Hören Sie es sich an <br>
        * '3' Neu aufnehmen <br>
    * '4', wenn Sie Ihre temporäre Ansage aufnehmen wollen." <br>
        * '1' Akzeptiere es / oder nehme die Ansage neu auf, falls es bereits eine gibt. <br>
        * '2' Anhören / oder löschen, falls schon vorhanden <br>
        * '3' Neu aufnehmen <br>
    * '5', wenn Sie Ihr Passwort ändern wollen." <br>
    * ... mit der '\*'-Taste kehren Sie zurück ins Hauptmenü." <br>
* ... die '\*'-Taste, wenn Sie Hilfe wünschen.“ <br>
* ... die '#'-Taste, um das System zu verlassen.“ <br>

## 3.	Aktivierung mittels Anrufweiterleitung (Call-Forward) in der CloudPBX über das 

### a.)	Web-Interface
Klicken Sie zunächst auf den Menüpunkt Kunden-Details, dann auf Subscriber und bei der betreffenden Nebenstelle oder Gruppe auf Einstellungen. Öffnen Sie nun das Menü Call-Forwards und entscheiden, bei welcher Bedingung die Anrufweiterleitung greifen soll: <br>

•	**Call Forward Unconditional** - generelle Anrufweiterleitung. <br>
•	**Call Forward Busy** - Anrufweiterleitung, wenn besetzt <br>
•	**Call Forward Timeout** - Anrufweiterleitung nach einer bestimmten Zeitspanne <br>
•	**Call Forward Unavailable** kommt zum Tragen, falls die Nebenstelle nicht registriert/erreichbar ist. <br>

Siehe hierzu auch [Anrufweiterleitung](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/). <br>

Nachdem Sie beim gewünschten Call-Forward-Typ auf den Button „Edit“ geklickt haben, können Sie die Destination „Voicemail“ (1) auswählen, mit einem Häkchen bei Enabled (2) aktivieren und mit dem SAVE-Button (3) speichern. <br>

![Call Forward Destinations1](https://user-images.githubusercontent.com/98753538/194002770-555766ee-23b6-48c4-81be-fdba5d7bb730.jpg)

Bei (4) gelangen Sie zum [Advanced View](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/#advanced-view). <br>

### b.)	Endgerät/Telefon
Die einzelnen Call Forward Typen können durch Eingabe der einzelnen Feature Codes direkt am Endgerät aktiviert werden, wobei die Zielrufnummer in diesem Fall die Kennung der Voicemail - also die 2000 - ist. <br>
Call Forward Unconditional: Einrichtung der Rufumleitung durch Wahl von **\*72\*2000** – Deaktivierung durch Wahl von **#72**. <br>
Call Forward on Busy: Einrichtung der Rufumleitung bei Besetzt durch Wahl von **\*90\*2000** – Deaktivierung durch Wahl von **#90**. <br>
Call Forward on Timeout: Einrichtung der Rufumleitung nach Zeit durch Wahl von **\*92\*30\*2000** (hier also nach 30 Sekunden) – Deaktivierung durch Wahl von **#92**. <br>
Call Forward on Not Available: Einrichtung der Rufumleitung bei „Nicht Registriert“ durch Wahl von **\*93\*2000** - Deaktivierung durch Wahl von **#93**. <br>
Die Deaktivierung aller eingerichteten Anrufweiterschaltungen erfolgt über den Feature Code **#96**. <br>


## 4.	Aktivierung mittels Weiterleitung (Call-Forward) im Telefon

Wichtig: Das Telefon muss registriert (online) sein. Nun können Sie eine Funktionstaste mit der Weiterleitung zur Voicebox (Anrufbeantworter) belegen, die - nach Aktivierung - alle Anrufer dorthin vermittelt, im Bild ist dies die Taste 8

![Neue_Tasten 1](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/b211d3a7-aada-496f-90e6-e3169078382d)

Wählen Sie anschließend die Funktion "Weiterleitung" (entspricht Call Forward)

![Neue_Tasten 2](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/64310c8b-61bf-4d3e-8f55-de578d2d0de8)

Anschließend aktivieren Sie die Funktion "Benutzerdefinierte Nummer verwenden), tragen unter Nummer __\*56*__NST  (z.B. __\*56*10__ für die Nebenstelle mit Durchwahl 10) ein und klicken auf SPEICHERN. 

![Neue_Tasten 4b](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/693ebc04-0127-4e17-b077-0c78c558d460)

Durch Belegung der Funktionstaste mit diesem Steuercode können Sie komfortabel per Tastendruck die Weiterleitung aktivieren oder abschalten. Im Display Ihres Gerätes sehen Sie die entsprechende Belegung

![Neue_Tasten 5](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/4532c887-b053-41c2-8943-dfcb704577ca)

Außerdem wird der aktuelle Status (Weiterleitung zur Voicemail aktiv / inaktiv) angezeigt:

![Neue_Tasten 6](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/e928d301-de8a-487f-8f3b-095af0adba30)


## 5.	Information über neue Nachrichten

Hat Ihnen jemand eine/mehrere Nachricht/en hinterlassen, bekommen Sie das auf zwei Wegen mitgeteilt:

### a)	Per Message Waiting Indikator am Telefon (siehe Pfeil) 

![Message Waiting Indicator](https://user-images.githubusercontent.com/98753538/194004796-a936a162-93b4-46e6-bba2-8045073749a2.png)

### b)	Benachrichtigung per E-Mail
Falls Sie dies wünschen, tragen Sie in den Subscriber-Einstellungen Ihre E-Mail-Adresse ein:

![Edit EMail](https://user-images.githubusercontent.com/98753538/194005083-c98072cb-b209-403e-8e0a-9372faae74de.jpg)

Hinterlässt ein Anrufer eine Nachricht, erhalten sie anschließend eine solche E-Mail:

![Message Mail](https://user-images.githubusercontent.com/98753538/194005152-ad047f85-3613-4b73-9bfd-14a324d37b53.jpg)

## 6.	Abhören der Nachrichten

Zum Abhören der Nachrichten stehen Ihnen mehrere Möglichkeiten zur Verfügung:

### a) Am Telefon 
durch Wahl der 2000  oder Drücken der Message-Taste. Bei Yealink sieht diese so aus:

![Message Key](https://user-images.githubusercontent.com/98753538/194005319-d83c8153-b424-42ff-ac2e-cceb59430095.jpg)

Folgen Sie anschließend dem Menü und "Drücken Sie . . . die '1', für alte/neue Nachrichten."

### b) Per WAV-Datei aus der E-Mail. 

![Message Mail with Attachement](https://user-images.githubusercontent.com/98753538/194005654-d0bb0ba9-09c2-400a-a544-ffe0f21db838.jpg)

Voraussetzung dafür ist, dass Sie zuvor bei den Einstellungen nicht nur Ihre E-Mail-Adresse eingetragen sondern auch den Unterpunkt „Attach WAV in Email“ per Häkchen aktiviert haben (= yes):

![Edit EMail Attachement](https://user-images.githubusercontent.com/98753538/194005789-460c79bf-f655-428b-b688-45312204d5e2.jpg)

### c) In der GUI 
unter „Konversationen“ beim Punkt „Sprachnachrichten“ durch Klicken der Taste „Play“ (Pfeil): 

![Message2](https://user-images.githubusercontent.com/98753538/194005901-19b9b576-4b01-44c1-9afc-69f8fadc88b5.jpg)
