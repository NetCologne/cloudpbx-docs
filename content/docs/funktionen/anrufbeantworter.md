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
Mit einer Sprachnachricht kann dem Anrufer zu einen mitgeteilt werden, dass sein Anruf nicht persönlich entgegengenommen wird. Zum anderen können Sie ihm weiterführende Informationen zukommen lassen, wie z. B. wann Sie wieder verfügbar sind, wie er Sie per E-Mail kontaktieren kann oder wie er zusätzliche Unterstützung erhält. Dabei wird unterschieden: <br>

### a) Nicht-verfügbar-Nachricht (Abwesenheitsansage)
Die „Nicht verfügbar-Nachricht“ ist die Standard-Begrüßung. Sie wird verwendet, wenn Sie den Anruf nicht entgegennehmen und der Anruf an Ihre Voicemail weitergeleitet wird. Wenn Sie nichts aufgezeichnet haben, spielt das Telefonsystem die gewählten Ziffern (des Anschlusses) mit dem Zusatz „ist nicht verfügbar“ ab.
Wenn Sie statt der „Nicht-verfügbar-Nachricht“ zur Begrüßung Ihren Namen, z.B. „Peter Schneider“ aufgezeichnet haben, gibt das System die Nachricht „Peter Schneider ist nicht verfügbar“ wieder. <br>

### b) Besetzt-Nachricht
Wenn Sie möchten, können Sie eine benutzerdefinierte Besetzt-Begrüßung aufzeichnen. Diese wird verwendet, wenn jemand Sie anruft und Sie gerade telefonieren. Wenn Sie nichts aufgezeichnet haben, gibt das System die gewählten Ziffern (des Anschlusses) mit dem Zusatz „ist besetzt“ wieder.
Wenn Sie statt der „Besetzt-Begrüßung“ Ihren Namen, z.B. „Petra Schmitz“ aufgezeichnet haben, spielt das System diese Nachricht ab: „Petra Schneider ist besetzt.“ <br>

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
Außer dem können Sie Ihren Namen aufsprechen (8). Dann hören ihn Anrufe anstatt Ihrer Telefonnummer. <br>

Zur Erzeugung einer elektronischen Ansage im wav-Format gehen Sie bitte folgendermaßen vor:  <br>
Suchen Sie im Internet mit "text to speech german kostenlos". Bei den Ergebnissen finden Sie leicht einen (kostenlosen) Text-zu-Sprache-Generator wie z.B. ttsfree, freetts oder ttsmp3. Dort können Sie Ihren gewünschten Ansagetext eingeben, wählen die Sprache und Stimme für die Ausgabe und erzeugen so eine mp3-Datei. Um diese in der Cloud-PBX verwenden zu können, ist noch eine Wandlung ins WAV-Format erforderlich. Entsprechende Konverter sind im Internet mit "mp3 wav converter" ebenfalls leicht zu finden. Wichtig: In Mono und nach a-Law konvertieren. <br>
Sie können die elektronischen Ansagen im Menü „Anrufeinstellungen“ unter „Anrufbeantworter“ hochladen und wieder zurücksetzen:  <br>

![Anrufbeantworter2](https://user-images.githubusercontent.com/98753538/193989527-bb699548-7a4c-41aa-a9b2-d5da3c99fdb2.jpg)

Zur Erinnerung: Wenn Sie als Administrator angemeldet sind, steht Ihnen der (zusätzliche) Menüpunkt „Kunden-Details“ zur Verfügung. Auch von hier aus gelangen Sie zu den „Subscribern“ und können dort „Einstellungen“ und den Menüpunkt „Voicemail and Voicebox“ auswählen bzw. öffen:  <br>

![Voicemail Ansagen2](https://user-images.githubusercontent.com/98753538/193989610-cfa67140-24e2-4752-a160-a337a9ff319f.jpg)

Ist die entsprechende Ansage bereits vorhanden, können Sie diese herunterladen, löschen oder mit dem Button „Edit“ eine neue laden.

### b.)	Tastatur des Endgerätes
Mit Drücken der Taste „Briefumschlag“ (bei Yealink-Telefonen) oder Tastenwahl der Ziffern 2 0 0 0 gelangen Sie in das Sprachbox-Menü der Cloud-PBX. Dieses ist folgendermaßen aufgebaut: „Drücken Sie . . .
*	. . . die '1', für alte/neue Nachrichten.“  <br>
  o	„Für erweiterte Optionen '3' drücken.“  <br>
 	  . . . die '3' um die Tonmitteilung Nachrichten zu hören.“  <br>
    	. . . die '*' um ins Hauptmenü zu kommen.“  <br>
  o	. . . die '4', um zur vorherigen Nachricht zu gelangen.“  <br>
  o	. . . die '5', um die aktuelle Nachricht wiederholen.“  <br>
  o	. . . die '6', um die nächste Nachricht abzuspielen.“  <br>
  o	. . . die '7', um die aktuelle Nachricht zu löschen.“  <br>
  o	'9', um diese Nachricht in einem Ordner zu speichern und   <br>
    	'0', für: Neue Nachrichten.  <br>
    	'1', für: Alte Nachrichten.  <br>
    	'2', für: Arbeits-Nachrichten.  <br>
    	'3', für: Familien-Nachrichten.  <br>
    	'4', für: Freunde-Nachrichten.  <br>
    	'#', um abzubrechen.  <br>
* . . . die '2', wenn Sie den Ordner wechseln wollen.“  <br>
  o	'0' für: Neue Nachrichten.“  <br>
  o	'1' für: Alte Nachrichten.“  <br>
  o	'2' für: Arbeits-Nachrichten.“  <br>
  o	'3' für: Familien-Nachrichten.“  <br>
  o	'4' für: Freunde-Nachrichten.“  <br>
  o	'#', um abzubrechen.“  <br>
*	. . . die '3', um zu den erweiterten Optionen zu gelangen.“  <br>
  o	'*', um zum Hauptmenü zurückzukehren.“  <br>
* . . . die '0', um zu den Mailboxoptionen zu gelangen.“  <br>
  o	'1' Zeichnen Sie Ihre Nicht-verfügbar-Nachricht auf  <br>
    	'1' akzeptieren  <br>
    	'2' Hören Sie es sich an  <br>
    	'3' Neu aufnehmen  <br>
  o	'2' Nehmen Sie Ihre Besetztnachricht auf  <br>
    	'1' akzeptieren  <br>
    	'2' Hören Sie es sich an  <br>
    	'3' Neu aufnehmen  <br>
  o	'3' Zeichnen Sie Ihren Namen auf  <br>
    	'1' akzeptieren  <br>
    	'2' Hören Sie es sich an  <br>
    	'3' Neu aufnehmen  <br>
  o	'4' Zeichnen Sie Ihre temporären Begrüßungen auf  <br>
    	'1' akzeptiere es / oder nehme die Ansage neu auf, falls es bereits eine gibt  <br>
    	'2' Anhören / oder löschen, falls schon vorhanden  <br>
    	'3' Neu aufnehmen  <br>
  o	'5' Ändern Sie Ihr Passwort  <br>
  o	'*' Um zum Hauptmenü zurückzukehren  <br>
* . . . die '*'-Taste, wenn Sie Hilfe wünschen.“  <br>
* . . . die '#'-Taste, um das System zu verlassen.“  <br>
