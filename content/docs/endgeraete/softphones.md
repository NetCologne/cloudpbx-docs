---
title: "Softphones"
date: 2026-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 509
toc: true
---
# Softphones
Mit einem Softphone können Sie über Ihren PC oder Ihr Smartphone Festnetzanrufe tätigen und entgegennehmen.
Für die Nutzung am PC wird ein kompatibles Headset benötigt. Gerne beraten wir Sie bei der Auswahl eines geeigneten Geräts.

# Offiziell Freigegebene Softphones
Die nachfolgend aufgeführten Softphones wurden von NetCologne für die Verwendung mit der CPBX-Telefonanlage geprüft und offiziell freigegeben.

## NetCall Desktop - Windows

Mit NetCall Desktop telefonieren Sie über Ihre Cloud PBX direkt am Windows-PC. Neben ein- und ausgehenden Anrufen unterstützt der Client mehrere Benutzerkonten und Gespräche, Halten und Vermitteln, Kontakte, Besetztlampenfelder (BLF), Gesprächsnotizen, lokale Aufnahmen, Voicemails und Rufumleitungen.

>💡**Hinweis**
>Die Nutzung des NetCall Desktop Clients für Windows erzeugt keine zusätzlichen Kosten.

### Voraussetzungen

- Ein PC mit Windows 11 und Internetverbindung.
- Eine eingerichtete CloudPBX-Nebenstelle mit Web-Benutzername und Web-Kennwort.
- Ein kompatibles Headset oder ein Mikrofon mit Lautsprechern.
- Freigegebener Mikrofonzugriff für NetCall Desktop in Windows.

### Quelle der Installationsdatei

Installieren Sie NetCall Desktop über den [Microsoft Store](https://apps.microsoft.com/detail/9pnhd6vg67v9?hl=de-DE&gl=DE). Öffnen Sie die Produktseite, wählen Sie die Installation aus und starten Sie anschließend die Anwendung.

<img alt="NC-Desktop" src="https://github.com/user-attachments/assets/ea1185e2-04c4-479f-9ef1-ad0a18448580" />

### Erste Anmeldung

Beim ersten Start erscheint die Anmeldung für Ihre Cloud PBX.

1. Tragen Sie unter **Benutzername** den vollständigen **Web-Benutzernamen einschließlich Anmeldedomäne** ein.
2. Tragen Sie unter **Passwort** das zugehörige **Web-Kennwort** ein.
3. Klicken Sie auf **Anmelden**. Der Client lädt die Telefoniekonfiguration automatisch.
4. Prüfen Sie die Statusanzeige oben rechts. Sobald dort **Registriert** steht, ist die Nebenstelle für die Telefonie angemeldet.

<img alt="netphone-anmeldung" src="https://github.com/user-attachments/assets/1139d96d-3892-4939-88b0-649d74c9bce6" />

>💡**Hinweis**
>Den Web-Benutzernamen finden Sie im Admin-Portal unter **PBX-Konfiguration > Nebenstellen > gewünschte Nebenstelle > Web-Benutzername**. Ergänzen Sie bei der Anmeldung die Anmeldedomäne, sofern sie noch nicht enthalten ist. Aus `Mustermann` und `@muster.cloudpbx.netcologne.de` wird beispielsweise `Mustermann@muster.cloudpbx.netcologne.de`.

Web-Zugangsdaten und SIP-Zugangsdaten können sich unterscheiden. Verwenden Sie zur Anmeldung die Web-Zugangsdaten; SIP-Benutzername, SIP-Kennwort und SIP-Domäne werden automatisch eingerichtet. Kennwörter speichert die Desktop-Anwendung im geschützten Anmeldedatenspeicher des Betriebssystems.

### Oberfläche und Benutzerkonten

Über die Symbole am unteren Fensterrand wechseln Sie zwischen den Bereichen:

| Bereich | Funktion |
|---|---|
| **Wähltastatur** | Rufnummern eingeben, Anrufe starten und zuletzt geführte Anrufe aufrufen. |
| **BLF / Favoriten** | Häufig benötigte Kontakte und Kurzwahlen anzeigen und interne Nebenstellen überwachen. |
| **Kontakte** | Telefonbuch durchsuchen, Kontakte verwalten und importieren. |
| **Anrufstapel** | Zwischen laufenden, gehaltenen und eingehenden Gesprächen wechseln. |
| **Voicemails** | Nachrichten der CloudPBX-Voicemailbox abhören und Ansagen verwalten. |
| **Weiterleitungen** | Rufumleitungen der ausgewählten Nebenstelle verwalten. |
| **Einstellungen** | Benutzerkonten, Audiogeräte und weitere Funktionen einrichten. |

Die **Anrufliste** öffnen Sie über **Liste** auf der Wähltastatur. **Statistiken & Reporting** erreichen Sie über die Einstellungen.

#### Mehrere Benutzerkonten verwenden

Unter **Einstellungen > Benutzerkonten > Neues Konto hinzufügen** können Sie weitere Konten einrichten. Vergeben Sie einen **Kontonamen**, tragen Sie **Portal-Benutzername** und **Portal-Passwort** ein, wählen Sie eine Kontofarbe und klicken Sie auf **Speichern**. Der Kontoname dient nur der Übersicht im Client und ändert weder den Namen noch die Durchwahl der Nebenstelle in der Telefonanlage.

Mit einem Klick auf die Kontoanzeige oben rechts wählen Sie das gewünschte aktivierte Konto aus. Diese Auswahl bestimmt das Konto für neue Anrufe über die Wähltastatur sowie die angezeigten CloudPBX-Kontakte, Voicemails und Weiterleitungen. Rückrufe aus einem vorhandenen Anrufeintrag und bereits laufende Gespräche behalten ihr zugehöriges Konto.

Aktivierte Telefoniekonten können gleichzeitig angemeldet sein und Anrufe empfangen. Unter **Benutzerkonten** lassen sich Konten bearbeiten, deaktivieren oder löschen. Wenn Sie das ausgewählte Konto deaktivieren oder entfernen, wählen Sie anschließend ausdrücklich ein anderes Konto aus.

### Audiogeräte und Headset einrichten

Öffnen Sie **Einstellungen > Audiogeräte** und wählen Sie die Geräte für folgende Aufgaben aus:

- **Eingang Mikrofon:** das Mikrofon Ihres Headsets oder ein anderes Aufnahmegerät.
- **Ausgabe Lautsprecher:** das Gerät, über das Sie Ihren Gesprächspartner hören.
- **Ausgabe Klingelton:** das Gerät, über das eingehende Anrufe hörbar sein sollen. Dies kann beispielsweise der PC-Lautsprecher sein, während das Gespräch über das Headset läuft.

Prüfen Sie die Auswahl mit **Mikrofon testen** und **Klingelton testen**. Beim Mikrofontest zeigt der Pegelbalken an, ob Sprache erkannt wird. Über **Datei wählen** können Sie einen eigenen Klingelton hinterlegen; **Standard** stellt den voreingestellten Klingelton wieder her.

Unter **Headset-Anrufsteuerung (HID)** wählen Sie ein unterstütztes USB-Headset aus und aktivieren die Steuerung mit **Verbinden**. Je nach Gerät stehen Annehmen, Auflegen und Stummschalten über die Headsettasten zur Verfügung. Die Anrufsteuerung wird getrennt von der Auswahl der Audiogeräte eingerichtet.

Unter **Einstellungen > Audioverarbeitung** finden Sie Echounterdrückung, Rauschunterdrückung und automatische Verstärkung des Mikrofons.

### Telefonieren

#### Ausgehenden Anruf starten

1. Wählen Sie bei mehreren Konten oben rechts das gewünschte Telefoniekonto aus.
2. Geben Sie auf der **Wähltastatur** eine Rufnummer oder interne Durchwahl ein. Sie können die PC-Tastatur verwenden oder eine Nummer einfügen. Bei einer Namenssuche wählen Sie den passenden Kontakt aus den Vorschlägen aus.
3. Klicken Sie auf **Anruf** oder drücken Sie im Eingabefeld **Enter**.

Interne Durchwahlen werden anhand des geladenen Nebenstellenverzeichnisses des zugehörigen Kontos aufgelöst. Alternativ starten Sie einen Anruf über das Hörersymbol in den Kontakten, über einen Favoriten oder aus der Anrufliste.

Über **Anonym** schalten Sie die Rufnummernunterdrückung für das ausgewählte Konto ein oder aus. Die Einstellung bleibt bis zum erneuten Ausschalten bestehen. **Lautlos** schaltet Klingel- und Anklopftöne im Client stumm; eingehende Anrufe werden weiterhin angezeigt.

#### Eingehenden Anruf annehmen oder ablehnen

Bei einem eingehenden Anruf werden der Anrufer und das zugehörige Konto angezeigt. Klicken Sie auf den grünen Hörer zum **Annehmen** oder auf den roten Hörer zum **Ablehnen**. Bei mehreren eingehenden Anrufen können Sie zwischen den angezeigten Anrufen wechseln.

Mit aktivierten **Desktop-Pop-ups** können Sie Anrufe auch über die Benachrichtigung annehmen oder ablehnen. Diese Funktion finden Sie in den Schnelleinstellungen. Windows muss Benachrichtigungen für die Anwendung zulassen.

#### Funktionen während eines Gesprächs

| Bedienelement | Funktion |
|---|---|
| **Halten / Fortsetzen** | Gespräch halten und anschließend wieder aufnehmen. |
| **Stumm** | Eigenes Mikrofon aus- oder einschalten. Sie hören den Gesprächspartner weiterhin. |
| **Weiterleiten** | Gespräch direkt oder nach Rückfrage an einen anderen Teilnehmer übergeben. |
| **Tastatur** | Ziffern und Sonderzeichen als DTMF senden, beispielsweise zur Bedienung einer Voicemailbox oder eines Sprachmenüs. |
| **Aufnehmen** | Lokale Gesprächsaufnahme starten oder stoppen. |
| **+ Kontakt** | Die Gegenstelle als Kontakt übernehmen. |
| **Lautstärkeregler** | Wiedergabelautstärke der Gegenstelle anpassen. |
| **Roter Hörer** | Gespräch beenden. |

Wenn Sie während eines Gesprächs in einen anderen Bereich wechseln, gelangen Sie über die eingeblendete Gesprächsleiste und **Zurück** wieder zur Gesprächsansicht.

#### Mehrere Gespräche und Anklopfen

Über den **Anrufstapel** sehen Sie Ihre laufenden und gehaltenen Gespräche. Wählen Sie dort das Gespräch aus, zu dem Sie wechseln möchten. Ein gehaltenes Gespräch nehmen Sie mit **Fortsetzen** wieder auf.

Unter **Einstellungen > Anrufverhalten** legen Sie fest, ob Gespräche beim Leitungswechsel automatisch gehalten oder fortgesetzt werden und ob der Client nach Gesprächsende zu einem vorherigen gehaltenen Gespräch zurückkehrt. Ist **Auto-Hold bei Leitungswechsel** ausgeschaltet, halten Sie das aktuelle Gespräch vor einem Wechsel manuell.

Mit **Anklopfen** lassen Sie weitere eingehende Anrufe während eines Gesprächs zu. Bei ausgeschaltetem Anklopfen weist der Client weitere Anrufe mit Besetzt ab. **Benutzerkonto bei Anrufannahme wechseln** bestimmt, ob beim Annehmen automatisch das Konto des eingehenden Anrufs ausgewählt wird.

### Gespräche verbinden

#### Verbinden ohne Rückfrage

1. Klicken Sie im laufenden Gespräch auf **Weiterleiten**.
2. Geben Sie die Zielrufnummer oder interne Durchwahl ein oder wählen Sie einen Kontakt aus den Vorschlägen.
3. Klicken Sie auf **Direkt**. Das Gespräch wird ohne vorherige Rücksprache an das Ziel übergeben.

Während der Übergabe zeigt der Client **Wird weitergeleitet…** an. Nach erfolgreicher Übergabe endet Ihre Beteiligung am Gespräch.

#### Verbinden mit Rückfrage

1. Klicken Sie im laufenden Gespräch auf **Weiterleiten** und wählen Sie das gewünschte Ziel.
2. Klicken Sie auf **Mit Rückfrage**. Das ursprüngliche Gespräch wird gehalten und das Ziel angerufen.
3. Sobald der Zielteilnehmer angenommen hat, können Sie das Gespräch ankündigen.
4. Klicken Sie auf **Übergeben**, um beide Teilnehmer zu verbinden.

Mit **Zurück** brechen Sie die Rückfrage ab und kehren zum ursprünglichen Gespräch zurück. War dieses bereits vor der Rückfrage gehalten, können Sie es mit **Fortsetzen** wieder aufnehmen.

### Kontakte und Telefonbuch

Unter **Kontakte** sehen Sie lokale Kontakte, CloudPBX-Telefonbucheinträge und die geladenen internen Nebenstellen des ausgewählten Kontos. Suchen Sie nach Name oder Nummer und starten Sie einen Anruf über das Hörersymbol. **Synchronisieren** lädt die Verzeichnisse erneut von der Telefonanlage.

#### Kontakt hinzufügen oder bearbeiten

Klicken Sie auf **Hinzufügen**, tragen Sie **Name** und **Nummer** ein und wählen Sie den Speicherort:

- **Lokal:** Der Kontakt wird nur auf diesem Gerät gespeichert.
- **CloudPBX - Persönlich:** Der Kontakt wird im persönlichen CloudPBX-Telefonbuch gespeichert.
- **CloudPBX - Firmenweit geteilt:** Der Kontakt wird als geteilter CloudPBX-Kontakt gespeichert.

Bestätigen Sie mit **Speichern**. Die Cloud-Speicherorte setzen ein verfügbares Konto mit gültigen Web-Zugangsdaten voraus. Bearbeitbare Kontakte ändern Sie über das Stiftsymbol und entfernen sie über den Papierkorb. PBX-Nebenstellen und zentral bereitgestellte Firmenkontakte lassen sich in dieser Ansicht nicht direkt bearbeiten oder löschen.

#### Kontakte importieren und exportieren

1. Klicken Sie auf **Kontakte importieren**.
2. Wählen Sie eine CSV- oder vCard-Datei aus oder ziehen Sie sie in das Importfenster. Unterstützt werden unter anderem Outlook-CSV, Google-Kontaktexporte und `.vcf`-Dateien. Eine Datei darf höchstens **10 MiB** groß sein und **10.000 Kontakte** enthalten.
3. Prüfen Sie die Vorschau und wählen Sie die zu importierenden Kontakte aus.
4. Wählen Sie den Speicherort und legen Sie fest, ob Duplikate anhand der Rufnummer übersprungen werden sollen.
5. Klicken Sie auf **Importieren** und prüfen Sie das angezeigte Ergebnis.

Die zusätzliche Option **Vorhandene CloudPBX-Kontakte vor dem Import löschen** entfernt vor dem Import die vorhandenen persönlichen und geteilten Telefonbucheinträge dieses Kontos. Aktivieren Sie sie nur, wenn Sie diesen Bestand ersetzen möchten.

Über **Kontakte als CSV exportieren** speichern Sie lokale Kontakte und CloudPBX-Telefonbucheinträge des ausgewählten Kontos in einer Datei.

### Favoriten, BLF und Pick-up

Klicken Sie in den **Kontakten** auf den **Stern**, um einen Eintrag als Favorit zu übernehmen. Ein erneuter Klick entfernt ihn aus den Favoriten. Bei internen PBX-Nebenstellen wird die BLF-Überwachung automatisch eingerichtet; externe Kontakte dienen als Kurzwahl.

Öffnen Sie **BLF / Favoriten**, um die Kacheln anzuzeigen. Interne Nebenstellen zeigen den von der Telefonanlage gemeldeten Zustand:

| Anzeige | Bedeutung |
|---|---|
| **Verfügbar** (grün) | Die überwachte Nebenstelle ist frei. |
| **Klingelt** (orange) | An der Nebenstelle wird ein eingehender Anruf signalisiert. |
| **Besetzt** (rot) | Die Nebenstelle führt ein Gespräch oder baut einen ausgehenden Anruf auf. |
| **Offline** (grau) | Es steht derzeit kein nutzbarer BLF-Status zur Verfügung. |

Wird bei einer klingelnden Nebenstelle **Abholen** eingeblendet, können Sie den Anruf damit auf Ihrem Client übernehmen (Pick-up). Die Funktion setzt die entsprechende Freigabe in Ihrer Telefonanlage voraus. Über **BLF-Pop-ups** in den Schnelleinstellungen lassen sich zusätzliche Hinweise zu klingelnden überwachten Nebenstellen ein- und ausschalten.

Über **Kurzwahl** legen Sie eine manuelle Kachel mit Name und Rufnummer an. Manuelle Kurzwahlen besitzen keine BLF-Statusanzeige. Über das Drei-Punkte-Menü passen Sie Favoriten an; durch Ziehen ändern Sie ihre Reihenfolge. Mit **Als Fenster öffnen** zeigen Sie die Favoriten in einem separaten Fenster an.

### Anrufliste, Notizen und Aufnahmen

#### Anrufliste

Öffnen Sie **Liste** auf der Wähltastatur. Die lokale Anrufliste enthält ein- und ausgehende Anrufe einschließlich verpasster Anrufe. Sie können die Liste filtern und nach **Name, Nummer oder Notiz** durchsuchen. Bei mehreren aktivierten Konten können Sie zwischen **Aktives Konto** und **Alle Konten** umschalten.

Ein Klick auf einen Eintrag öffnet den Gesprächsverlauf mit dieser Gegenstelle. Dort finden Sie Datum, Status, Dauer, Notizen und zugehörige Aufnahmen. Über das Hörersymbol starten Sie einen Rückruf mit dem Konto des Anrufeintrags.

#### Gesprächsnotizen

Tragen Sie während eines Gesprächs Ihre Notiz in **Notiz zum Gespräch** ein. Änderungen werden automatisch lokal gespeichert; die Anzeige **Lokal gespeichert** bestätigt das Speichern. Nachträglich öffnen Sie den Gesprächsverlauf in der Anrufliste und wählen **Notiz hinzufügen** oder **Notiz bearbeiten** am gewünschten Anruf.

#### Gesprächsaufnahmen

Mit **Aufnehmen** starten Sie im verbundenen Gespräch eine lokale Aufnahme. Ein weiterer Klick stoppt sie; beim Gesprächsende wird sie ebenfalls beendet. Unter **Einstellungen > Anrufverhalten > Automatisch aufnehmen** können Sie die automatische Aufnahme angenommener Gespräche einschalten.

Aufnahmen finden Sie beim zugehörigen Anruf im Gesprächsverlauf. Dort können Sie sie **Abspielen** oder **Herunterladen**. Die Aufnahmen liegen lokal auf diesem Gerät und werden nicht in die Cloud PBX hochgeladen. Der Client bewahrt bis zu **100 abgeschlossene Aufnahmen** auf; bei weiteren Aufnahmen werden ältere Aufnahmen oberhalb dieser Grenze automatisch entfernt. Laden Sie Aufnahmen, die Sie dauerhaft benötigen, als Datei herunter.

Meldet der Client, dass eine Aufnahme nur vorübergehend im Speicher liegt, laden Sie diese vor dem Beenden der Anwendung herunter.

### Voicemailbox und Ansagen

Unter **Voicemails** sehen Sie die Nachrichten für das ausgewählte Konto. Über die Symbole an einer Nachricht können Sie diese **Abspielen**, **Herunterladen**, den Anrufer **Zurückrufen** oder die Nachricht **Löschen**. Sofern die Telefonanlage ein Transkript bereitstellt, können Sie es über **Transkript anzeigen** einblenden. Beim Abspielen wird die Nachricht als gelesen markiert.

Mit **Aktualisieren** laden Sie die Nachrichten erneut. Die Schaltfläche **Voicemailbox** ruft die konfigurierte Abfragenummer an; voreingestellt ist **2000**. Zur Bedienung des Sprachmenüs öffnen Sie während des Anrufs **Tastatur**.

Über **Ansage** verwalten Sie Ihre persönlichen Voicemail-Ansagen:

1. Wählen Sie **Temporär**, **Besetzt** oder **Nicht erreichbar**. Eine vorhandene temporäre Ansage hat Vorrang vor den anderen Ansagen.
2. Wählen Sie mit **WAV wählen** eine Audiodatei aus oder sprechen Sie mit **Aufsprechen** eine Ansage ein. Beenden Sie die Aufnahme mit **Stopp**.
3. Klicken Sie auf **Hochladen**, um die Ansage in der Telefonanlage zu speichern.
4. Prüfen Sie die gespeicherte Ansage mit **Abspielen**.

Mit **Löschen** entfernen Sie die eigene Ansage des gewählten Typs. Entfernen Sie eine temporäre Ansage, wenn wieder die situationsabhängigen Ansagen verwendet werden sollen.

### Rufumleitungen einrichten

Unter **Weiterleitungen** verwalten Sie die Rufumleitungen der ausgewählten Nebenstelle direkt in der Cloud PBX. Gespeicherte Regeln gelten auch dann, wenn NetCall Desktop beendet ist.

Folgende Arten stehen zur Verfügung:

| Art | Wirkung |
|---|---|
| **Ständig** | Anrufe sofort weiterleiten, ohne vorheriges Klingeln. |
| **Nach Zeit** | Weiterleiten, wenn innerhalb der eingestellten Klingeldauer niemand annimmt. |
| **Wenn besetzt** | Weiterleiten, wenn die Nebenstelle besetzt ist. |
| **Nicht erreichbar** | Weiterleiten, wenn kein Endgerät der Nebenstelle erreichbar ist. |

1. Klicken Sie auf **Hinzufügen**.
2. Wählen Sie die Art der Weiterleitung.
3. Wählen Sie als Ziel eine **Rufnummer / Nebenstelle**, die **Voicemailbox** oder eine verfügbare **Ansage** aus. Tragen Sie bei einem Rufnummernziel die Nummer oder interne Durchwahl ein.
4. Legen Sie, falls erforderlich, die Klingeldauer fest und klicken Sie auf **Rufumleitung speichern**.

In der Übersicht schalten Sie Regeln zwischen **Aktiv** und **Inaktiv** um, bearbeiten Ziele über das Stiftsymbol oder löschen Regeln über den Papierkorb. Bei **Nach Zeit** bestimmt **Timeout nach dem Klingeln** die Klingeldauer am eigenen Gerät.

Über **Bedingung** können Sie Regeln auf Bürozeiten, Wochentage, Datumsbereiche oder bestimmte anrufende beziehungsweise angerufene Rufnummern begrenzen. Über **Ziel hinzufügen** ergänzen Sie weitere Ziele in einer Weiterleitungskette. Voicemail und Ansage bilden das Ende einer solchen Kette.

Falls die Übersicht auf weitere, hier nicht bearbeitbare Weiterleitungstypen hinweist, verwalten Sie diese im PBX-Portal.

### Statistiken und Reporting

Öffnen Sie **Einstellungen > Statistiken & Reporting > Statistiken & Reporting öffnen** und wählen Sie einen Zeitraum, beispielsweise **Heute**, **Letzte 7 Tage** oder **Dieser Monat**.

Die Ansicht lädt Anrufdaten aus der Telefonanlage und zeigt unter anderem Anrufvolumen, Erreichbarkeit, Gesprächsdauer, Annahmezeit und häufige Gesprächspartner. Angaben zur Sprachqualität erscheinen, sofern entsprechende Messdaten vorliegen. Die detaillierte Anrufliste können Sie durchsuchen und nach Richtung sowie Status filtern. Über **Exportieren** speichern Sie die geladenen Anrufdaten als CSV-Datei.

Die Statistiken stammen aus der Telefonanlage. Die Anrufliste mit Gesprächsnotizen und Aufnahmen speichert der Client dagegen lokal; beide Ansichten können deshalb unterschiedliche Einträge enthalten.

### Weitere Einstellungen und Integrationen

- **Schnelleinstellungen:** Autostart, Dunkelmodus, Desktop-Pop-ups und BLF-Pop-ups ein- oder ausschalten.
- **Agentenstatus:** Über die Statusanzeige unten wählen Sie **Verfügbar**, **Beschäftigt**, **Nicht stören (DND)** oder **Offline**. **Beschäftigt** weist eingehende Anrufe im Client mit Besetzt ab. **Nicht stören (DND)** wird an die Telefonanlage übermittelt. **Offline** meldet das betreffende Telefoniekonto von der Telefonie ab; mit **Verfügbar** melden Sie es wieder an.
- **PBX-Funktionen:** Anrufwarteschlange und Warteschleifenmusik für die ausgewählte Nebenstelle verwalten.
- **Wählhilfe:** Rufnummern aus `tel:`- und `callto:`-Links sowie aus Programmen mit unterstützter Windows-Wählhilfe übernehmen. Ordnen Sie die Rufnummernlinks unter **Windows-Einstellungen > Apps > Standard-Apps** dem Client zu. Mit **Direkt anrufen (Auto-Dial)** startet ein übernommener Anruf sofort; andernfalls wird die Nummer zunächst ins Wählfeld eingetragen.
- **CRM-Integration:** Eine Kontaktseite im Browser öffnen oder Anrufereignisse per Webhook übertragen. Wählen Sie den Auslöser **Klingeln / Wählen**, **Annehmen** oder **Beenden**, hinterlegen Sie die URL und prüfen Sie die Einrichtung mit **Testen** beziehungsweise **Test-Webhook**.
- **Daten löschen:** Verwaiste Aufnahmedateien bereinigen, die lokale Anrufliste samt Aufnahmen leeren oder lokale Kontakte löschen. **Lokale Daten löschen** entfernt sämtliche lokalen Daten einschließlich Favoriten, App-Einstellungen und eingerichteter Konten. Diese Aktionen ändern keine Daten in der Cloud PBX.

#### Comfort Go per QR-Code anmelden

Unter **Einstellungen > Mobile App** finden Sie die Store-Links für Comfort Go. Wählen Sie oben rechts das gewünschte Telefoniekonto aus und klicken Sie auf **Anmelde-QR-Code generieren**. Öffnen Sie Comfort Go auf dem Smartphone und scannen Sie den Code im Anmeldebildschirm. Beachten Sie die angezeigte Restgültigkeit; nach Ablauf generieren Sie einen neuen Code.

#### CloudPBX-Verwaltung

Wird Ihr Zugang bei der Anmeldung als Verwaltungskonto erkannt, öffnet der Client die **CloudPBX-Verwaltung**. Dort stehen je nach Berechtigung beispielsweise Nebenstellen, Gruppen, Geräte und weitere Verwaltungsbereiche bereit. Zum Telefonieren wählen Sie ein eingerichtetes Telefoniekonto aus.

### Anwendung im Hintergrund und beenden

Das Schließen des Hauptfensters über **X** blendet die Anwendung aus. Sie läuft im Infobereich von Windows weiter und kann weiterhin Anrufe empfangen. Über das Anwendungssymbol und **NetCall Desktop anzeigen** öffnen Sie das Fenster erneut. Mit **Beenden** schließen Sie den Client vollständig.

Aktivieren Sie **Autostart** in den Schnelleinstellungen, wenn NetCall Desktop bei der Windows-Anmeldung starten soll. Falls Windows den Autostart blockiert, prüfen Sie **Einstellungen > Apps > Autostart**.

### Hilfe bei häufigen Problemen

| Problem | Prüfschritte |
|---|---|
| **Anmeldung fehlgeschlagen** | Vollständigen Web-Benutzernamen mit Anmeldedomäne und das Web-Kennwort prüfen. |
| **Nicht registriert / Registrierung fehlgeschlagen** | Internetverbindung, aktiviertes Benutzerkonto und Agentenstatus prüfen. Bei **Offline** wieder **Verfügbar** wählen. |
| **Web-Anmeldung erforderlich** | Über **Webpasswort aktualisieren** die gültigen Web-Zugangsdaten erneut eingeben. |
| **Kein Mikrofonton** | Unter **Audiogeräte** das richtige Mikrofon wählen und testen. In Windows unter **Datenschutz und Sicherheit > Mikrofon** den Zugriff für die Anwendung beziehungsweise Desktop-Apps erlauben. |
| **Kein Klingelton** | **Lautlos**, das gewählte Klingeltongerät und die Windows-Lautstärke prüfen; **Klingelton testen** verwenden. |
| **Kein BLF-Status oder kein Pick-up** | Eine interne Nebenstelle aus den Kontakten als Favorit übernehmen und die Freigaben der Telefonanlage prüfen. **Abholen** erscheint nur bei einem übernehmbaren eingehenden Anruf. |

## NetCall Pro - Mac OS
Mit dem SIP Client „NetCall Pro“ stellt NetCologne eine Anwendung für MacOS bereit, die optimal für die Verwendung mit dem Produkt Cloud PBX geeignet ist. Der Vorteil liegt darin, dass die grundlegenden Parameter bereits voreingestellt sind und bei der Installation lediglich die Benutzerdaten für die gewünschte Nebenstelle angegeben werden müssen, um sofort telefonieren zu können.

>💡**Hinweis**
>Durch die Installation von NetCall Pro für Mac OS und dessen Verwendung mit einer Nebenstelle in der Cloud PBX fallen monatliche Gebühren an. Diese entnehmen Sie bitte der aktuellen Preisliste.

### Quelle der Installationsdatei

Die Installationsdatei für die aktuelle Version 5.6.12.1 finden Sie unter folgendem Link:<br>
[NetCall Pro 5.6.12.1 für Mac OS](https://shop.zoiper.com/download.php?id=NZ7SOOQEJYKGYMU)


### Installation der Anwendung
Führen Sie den .exe Installer für Windows bzw. die .pkg Datei für MAC OS aus. Navigieren Sie sich durch den Installer per Button "Next". <br>
Die vorgeschlagenen Einstellungen des Installers müssen nicht angepasst werden, fahren Sie mit den bereits empfohlenen Optionen durch.

<img alt="image" src="https://github.com/user-attachments/assets/b87f83df-6a35-4cc4-8e4b-875bfb9c8f1a" />
<img alt="image" src="https://github.com/user-attachments/assets/4a037638-ad12-4ad7-a3ee-13acabb62cd5" />
<img alt="image" src="https://github.com/user-attachments/assets/d272f0fa-f59f-407f-9637-b625d840c5dc" />
<img alt="image" src="https://github.com/user-attachments/assets/9e7ca044-f9c5-41f4-83cf-f3794068625f" />
<img alt="image" src="https://github.com/user-attachments/assets/50a0f101-e7db-4d76-83d1-a790f4d7acba" />
<img alt="image" src="https://github.com/user-attachments/assets/3352dba4-cb4c-4193-aeba-8695e674d5c0" />
<img alt="image" src="https://github.com/user-attachments/assets/2bb31cdf-f52f-4692-8103-6974540edf9e" />
<img alt="image" src="https://github.com/user-attachments/assets/66a9cd1b-f6a0-4369-a4cb-74068b9d05fd" />

### Konfiguration eines Benutzers

Nach der Installation erfolgt die Konfiguration des gewünschten Benutzers. Dazu benötigen Sie den **WEB-Benutzer** mit der **vollständigen Domain** und das zugehörige **WEB-Passwort**. Hierbei ist darauf zu achten, dass sich die Namen für SIP-Benutzer und WEB-Benutzer unterscheiden können.

>💡**Hinweis** 
>Bitte beachten Sie, dass NetCall Pro nur einen SIP Benutzer der Cloud PBX unterstützt. Zusätzliche manuell angelegte SIP Konten stehen nach einem Neustart der Anwendung nicht mehr zur Verfügung.

Für die folgenden Beispiele wird der WEB-Benutzer softphone@firmaid.cloudpbx.netcologne.de mit dem zugehörigen SIP-Benutzer softphone-sip@firmaid.cloudpbx.netcologne.de verwendet.

Starten Sie NetCall Pro.

Jetzt geben Sie den WEB-Benutzer mit der vollständigen **Domain** und das **WEB-Passwort** ein. Die Häkchen sollten gesetzt werden. Damit merkt sich NetCall Pro die Anmeldedaten und meldet den Benutzer automatisch beim Starten an der Cloud PBX an.
<img alt="image" src="https://github.com/user-attachments/assets/2ff1d85a-3003-4960-bddf-ad0a8657c967" />

Anschließend werden ein paar Tests durchlaufen, bei denen die Verfügbarkeit von Lautsprechern, Mikrofon und einer Videokamera geprüft werden. Um NetCall Pro nutzen zu können, ist der Zugriff auf mindestens den Lautsprecher und das Mikrofon erforderlich. Sofern vorhanden, kann an dieser Stelle auch ein Headset ausgewählt werden.

Außerdem wird geprüft, ob in der Windows Defender Firewall Anpassungen erforderlich sind. Um NetCall Pro verwenden zu können, müssen Sie die Änderungen zulassen.
<img alt="image" src="https://github.com/user-attachments/assets/eb60dcc4-350a-4fef-b4e5-f7145d82f1ce" />

Damit ist NetCall Pro für die grundlegende Telefonie eingerichtet.

### Telefonbuch, Busy Lamp Field und Pick-up

Im Telefonbuch können Sie Ihre individuellen Kontakte speichern. Zur Verwendung der „Busy Field Lamp“ (BLF) und von Pick-up ist dies zwingend notwendig. Das bedeutet, dass Sie die Nebenstellen Ihrer Cloud PBX, deren Status Sie angezeigt bekommen möchten, im Telefonbuch eintragen müssen. Gleiches gilt, wenn Sie ankommende Rufe von anderen Nebenstellen heranholen wollen (Pick-up).

#### Telefonbuch (Eintrag manuell erstellen)

Ein neuer Eintrag wird ins Telefonbuch aufgenommen, indem Sie auf das Plus-Zeichen neben den Reitern klicken und dann „Kontakt hinzufügen“ wählen.
<img alt="image" src="https://github.com/user-attachments/assets/e224f6f0-cedd-4def-b288-6f809c72b35d" />

In dem sich öffnenden Fenster können die Stammdaten wie Vorname, Name, Firma etc. eingetragen werden. Um nun auch die Telefonnummer eintragen zu können, muss ein zusätzliches Feld hinzugefügt werden.
Hier wird als Feldtyp „Telefon“ gewählt und mit hinzufügen bestätigt. Bei internen Teilnehmern wird unter Telefon der SIP-Benutzer eingetragen. Als Beispiel wird hier „tims“ verwendet. 
<img alt="image" src="https://github.com/user-attachments/assets/95f4aa1a-ad14-47af-8335-aac8b5126059" />

Als „Wählkonto“ wird der eigene SIP-Benutzer gewählt. Sofern es sich bei dem Telefonbucheintrag um eine Nebenstelle der eigenen Cloud PBX handelt, können Sie den Status dieser Nebenstelle als „Besetztlampenfeld (BLF)“ anzeigen lassen, indem Sie bei „Anwesenheitskonto“ ebenfalls den eigenen SIP-Benutzer auswählen. Diese Funktion wird im Kapitel „Busy Lamp Field“ genauer beschrieben.
<img alt="image" src="https://github.com/user-attachments/assets/5d7ae9b9-adf9-496d-bb97-e3d57d5bf06f" />

Beim Verlassen des Fensters müssen die Änderungen gespeichert werden.
<img alt="image" src="https://github.com/user-attachments/assets/703f54a5-b8a0-4213-969d-3912b8678abb" />

#### Telefonbuch (Kontakte importieren)

Für eine größere Anzahl an Kontakten empfiehlt es sich, diese als CSV-Datei zu importieren. Dazu klicken Sie auf das Plus-Zeichen neben den Reitern und wählen „Kontakte importieren“ aus.
<img alt="image" src="https://github.com/user-attachments/assets/ec8ff004-d6ec-4d65-a31f-7871c08beb92" />

Wählen Sie nun die gewünschte CSV-Datei mit zugehöriger Codierung und Separator aus und bestätigen Sie die Auswahl durch Klick auf „Datei analysieren“.
<img alt="image" src="https://github.com/user-attachments/assets/11dd01f5-af3a-45cf-9519-d4fc79b0df7e" />

Im folgenden Fenster werden die Spalten der CSV-Datei den Feldern im Telefonbuch zugeordnet. Im gezeigten Beispiel besteht die CSV-Datei aus drei Spalten: Vorname, Nachname, Festnetz

Max,Mustermann,+4912345678<br>
Petra,Musterfrau,+4987654321<br>

<img alt="image" src="https://github.com/user-attachments/assets/4142c338-ce6b-413f-a32f-114ea99c66cd" />

Im letzten Schritt können Sie aus der CSV-Datei die zu importierenden Kontakte auswählen. Dabei gilt, dass die Kontakte grundsätzlich im Telefonbuch angelegt werden. Vorhandene Kontakte werden nicht überschrieben.
<img alt="image" src="https://github.com/user-attachments/assets/14e94ed1-11d9-46aa-8e06-d39728637207" />

Nach dem Import erscheinen die neuen Kontakte sofort im Telefonbuch.
<img alt="image" src="https://github.com/user-attachments/assets/b04c8b0b-7e78-4035-a672-f5f19d9df5e2" />

#### Busy Lamp Field

Voraussetzung für die Verwendung der Funktion „Busy Lamp Field“ ist der entsprechende Eintrag der Nebenstelle im Telefonbuch. Als Beispiel wird hier der Eintrag „tims“ verwendet. Siehe hierzu auch Kapitel Telefonbuch.
Außerdem muss in dem SIP Konto unter Einstellungen „BLF benutzen“ aktiviert sein.
<img alt="image" src="https://github.com/user-attachments/assets/e04c5373-0c83-494e-8343-5b88d7dc1f30" />

Wird die Nebenstelle „tims“ angerufen, so wird das im Telefonbuch durch ein rotes Glockensymbol angezeigt.

<img alt="image" src="https://github.com/user-attachments/assets/d86b520f-7122-4217-a3c3-1dc86b548406" />

Sobald das Gespräch angenommen wurde, wird das durch einen blauen Kreis mit Telefonhörer angezeigt.

<img alt="image" src="https://github.com/user-attachments/assets/92fd4498-0020-41a5-b990-97f885072a2d" />

#### Pick-up

Zur Verwendung von Pick-up muss der entsprechende Eintrag im Telefonbuch ergänzt werden, d.h. es muss ein benutzerdefiniertes Feld hinzugefügt werden. Das Feld kann individuell benannt werden. Entsprechend der Funktion wird hier „pick-up“ eingetragen.
<img alt="image" src="https://github.com/user-attachments/assets/963f275b-edd9-4e04-a31f-82a6ebc2c99b" />

Der Wählcode für Pick-up ist *99*tims. Als Wählkonto wird das eigene Konto ausgewählt. Das Anwesenheitskonto wird auf „Nicht verwenden“ gesetzt.
<img alt="image" src="https://github.com/user-attachments/assets/80ad6bae-126f-438b-901b-5f78b11e000c" />

Wird der Teilnehmer „tims“ angerufen, wird dies im Telefonbuch wie im Kapitel Busy Lamp Field beschrieben angezeigt. Zum Heranholen des Gesprächs klicken Sie zuerst auf den Hörer und anschließend auf „Pick-up“ in dem sich öffnenden Fenster.
<img alt="image" src="https://github.com/user-attachments/assets/baedc814-f485-4cd6-8249-211d900e911b" />

Wenn die Verbindung hergestellt ist, wird das folgende Fenster angezeigt und Sie können das Gespräch führen und weitere Funktionen, wie z.B. Stummschalten, Halten etc. verwenden.
<img alt="image" src="https://github.com/user-attachments/assets/b434af74-a011-4a21-88dd-2ad5e2bd7d81" />

### Verbinden
Mit der Funktion **Verbinden** können Sie ein laufendes Gespräch an einen anderen Teilnehmer übergeben.
Für die Gesprächsübergabe stehen Ihnen folgende Möglichkeiten zur Verfügung:

- **Verbinden ohne Rückfrage**  
  Das Gespräch wird direkt an den gewünschten Teilnehmer übergeben, ohne vorherige Rücksprache.

- **Verbinden mit Rückfrage**  
  Vor der Übergabe können Sie den Zielteilnehmer kontaktieren und das Gespräch ankündigen. Anschließend entscheiden Sie, ob die Übergabe erfolgen soll.

- **Verbinden in der Rufphase**  
  Eingehende Anrufe können direkt an einen anderen Teilnehmer weitergeleitet werden, ohne dass Sie das Gespräch zuvor annehmen müssen.


#### Verbinden ohne Rückfrage

Sie führen ein Telefongespräch und möchten dieses nun zu einem anderen Anschluss ohne Rückfrage verbinden. Dazu klicken Sie zuerst auf den Knopf „Übergabe“.
<img alt="image" src="https://github.com/user-attachments/assets/88f708a9-bfb9-4117-b0f9-68ed1ab0e710" />

Die gewünschte Rufnummer geben Sie oben links in das Feld ein. Hier soll als Beispiel an die Nebenstelle „19“ verbunden werden. Anschließend klicken Sie auf den kleinen Pfeil neben dem Feld.
<img alt="image" src="https://github.com/user-attachments/assets/8e7a2cf4-b2a3-46c0-9792-9ddd7cb69f8c" />

Das Gespräch wird an die Nebenstelle „19“ übergeben. Für Sie ist das Gespräch damit beendet.

#### Verbinden mit Rückfrage

Sie führen ein Telefongespräch und möchten dieses nun zu einem anderen Anschluss mit Rückfrage verbinden.
Dazu müssen Sie das aktive Gespräch „halten“.
<img alt="image" src="https://github.com/user-attachments/assets/ad4a4f7f-4086-4e55-a834-70c6ddca94c5" />

Geben Sie dann in dem Feld links oben die Rufnummer ein, an die das Gespräch übergeben werden soll und klicken auf den kleinen Telefonhörer darunter. In diesem Beispiel wird die Nebenstelle „19“ angerufen.
<img alt="image" src="https://github.com/user-attachments/assets/36d7e6d8-3b6f-4bf9-acfa-4b4d416a7464" />

Sobald der Gesprächspartner das Gespräch entgegen nimmt können Sie die Übergabe absprechen. Anschließend wechseln Sie zu dem ursprünglichen Anrufer „mulheim“, indem Sie auf den Teilnehmer unter „Anrufe“ klicken.
<img alt="image" src="https://github.com/user-attachments/assets/c8df01ca-973e-4c04-873c-47394e13da0e" />

Nun leiten Sie die Übergabe ein. Dazu klicken Sie zuerst auf „Übergabe“ und wählen anschließend das Ziel unter „Anrufe“ aus. Damit ist das Gespräch für Sie beendet und die Übergabe ist abgeschlossen.
<img alt="image" src="https://github.com/user-attachments/assets/ef8e5aa1-7829-4962-a5f0-4cd0e1593d21" />

#### Verbinden in der Rufphase

Bei dieser Funktion geht es darum, dass ein kommendes Gespräch weiterverbunden werden kann, ohne es zuvor anzunehmen.

Wenn ein Gespräch im NetCall Pro signalisiert wird, klicken Sie ohne das Gespräch anzunehmen direkt auf „Übergabe“. Nun geben Sie in dem Feld oben links die Rufnummer ein, zu der Sie weiterverbinden möchten, und klicken anschließend auf den kleinen Pfeil. Damit haben Sie das Gespräch an die gewählte Nummer verbunden.
<img alt="image" src="https://github.com/user-attachments/assets/db8b2068-ba18-4421-bc1e-478efb99ec96" />

## Comfort Go App - iOS & Android 

<img alt="comfort-go" src="https://github.com/user-attachments/assets/1a995f0b-3ca5-41e1-b060-32eb64655ae8" /><br>
Für Apple und Android Geräte steht die Comfort Go App im Apple App Store bzw. Google Play Store zur Verfügung.<br>
Ausführliche Informationen zur Installation, Einrichtung und Nutzung finden Sie in unserem Wiki-Eintrag zur Comfort Go App:
[Wiki Eintrag Comfort Go App](https://cloudpbx-doku.netcologne.de/docs/endgeraete/comfort-go-app/)

>💡**Hinweis** 
>Die Comfort Go App ist primär für die mobile Erreichbarkeit unterwegs konzipiert. Sie stellt eine sinnvolle Ergänzung zur Telefonie dar, ersetzt jedoch keinen festen Arbeitsplatz mit Hardware-Telefon oder PC-Softphone.
Insbesondere bei einem hohen Anrufaufkommen empfehlen wir die Nutzung eines Hardware-Telefons oder eines PC-Softphones mit geeignetem Headset. Nur diese Lösungen bieten dauerhaft die bestmögliche Sprachqualität, Stabilität und Benutzerfreundlichkeit im Büroalltag.

# Third Party Softphones - Nicht offiziell freigegeben
Die nachfolgend aufgeführten Softphones können für die Telefonie mit der CPBX-Telefonanlage verwendet werden. Bitte beachten Sie, dass je nach eingesetzter Software nicht alle Funktionen und Komfortmerkmale unterstützt werden.

>💡**Hinweis** 
>Diese Anwendungen wurden von NetCologne weder geprüft noch offiziell freigegeben. Die Nutzung erfolgt daher auf eigene Verantwortung. Für Einschränkungen, Fehlfunktionen oder Inkompatibilitäten kann kein Support oder keine Haftung durch NetCologne übernommen werden.

## PhonerLite

Installation des Softclients unter http://phonerlite.de/download_de.htm. 

### Konfiguration

Zur Konfiguration wird im Reiter "Server" in den Feldern Proxy/Registrar und Domain/Realm der Servername eingetragen. Für die Registrieung ist ein Häkchen zu setzen - 3.600 Sekunden sind ein plausibler Wert. Das Häkchen beim message-waiting indicator (MWI) ist optional:
![PhoneLite Konfiguration Server](https://user-images.githubusercontent.com/98753538/153848572-20e621de-3bd6-49a9-8b27-91cfaa74f07c.jpg)
<br>
<br>  
Im Reiter "Benutzer" werden Benutzername, Angezeigter Name, Authentifizierungsname und zur Bestätigung das SIP-Kennwort eingetragen:
![PhoneLite Konfiguration Benutzer](https://user-images.githubusercontent.com/98753538/153848487-ffd54614-be89-4a5e-a1bb-7d88b315be46.jpg)
<br>
<br>  
Um die Inhalte zu schützen bzw. sicher zu verschlüsseln, wird im Reiter "Netzwerk" TLS als bevorzugte Verbindungsart ausgewählt. Der Lokale Port lautet 5061:
![PhoneLite Konfiguration Netzwerk](https://user-images.githubusercontent.com/98753538/153848648-7e632f41-637a-4e9e-9981-62e29ab2c0cd.jpg)
<br>
<br>  
Im Reiter "Codecs" muss der Codec "G.711 A-Law" ausgewählt werden. Weitere Codecs sind optional. Wichtig auch die Häkchen bei SRTP und SAVP:
![PhoneLite Konfiguration Codecs](https://user-images.githubusercontent.com/98753538/153848681-538cc078-55c7-4d99-a235-6ea1dedfa2ad.jpg)
<br>
<br>  
Abschließend speichert man das Profil mit Angabe eines Namens
![PhoneLite Konfiguration Speichern](https://user-images.githubusercontent.com/98753538/153848898-3573ac86-51c3-46d6-8db3-87855a3fd115.jpg)
<br>
<br>  
und erhält in der unteren Statusleiste eine Bestätigung der Registrierung:
![PhoneLite Konfiguration Registrierung](https://user-images.githubusercontent.com/98753538/153848918-f7d61a80-3fb9-4fdf-a09f-fc252ebfb171.jpg)
<br>
<br>  
### Telefonbuch

PhonerLite bietet die Möglichkeit ein Telefonbuch anzulegen:
![PhoneLite Konfiguration Telefonbuch](https://user-images.githubusercontent.com/98753538/153849003-47444112-b522-4fb7-8d51-908cb3d2ed61.jpg)
<br>
<br>  
Im Menue "Optionen" können die Kurzwahltasten angewählt werden:
![PhoneLite Konfiguration Kurzwahl](https://user-images.githubusercontent.com/98753538/153849019-0e5857be-3c33-44a8-92c6-b6fffb33f279.jpg)
<br>
<br>  
Zur Belegung zieht man den gewünschten Telefonbuch-Eintrag einfach auf das Kurzwahl-Feld:
![PhoneLite Konfiguration Kurz Kollege](https://user-images.githubusercontent.com/98753538/153849040-d45cd9ec-cdd1-4644-aba0-667edcf25be6.jpg)


## Zoiper

Für die Verwendung mit der Cloud PBX ist die kostenpflichtige Version erforderlich, da nur diese die notwendige Verschlüsselung mit TLS und SRTP unterstützt.

Die aktuelle Version laden Sie am besten direkt vom Hersteller herunter: https://www.zoiper.com/en/voip-softphone/download/current
Zur Installation des Clients folgen Sie der Anleitung des Herstellers.

### Konfiguration

Die folgende Beschreibung führt Sie durch die grundlegende Konfiguration für die Cloud PBX. Nach dem Start des Clients erscheint zunächst ein Fenster mit leeren Feldern für die Anmeldedaten. Dort werden die Anmeldedaten für den Subscriber eingetragen. Exemplarisch wird hier der Subscriber "mulheim" in der Domäne xxx.cloudpbx.netcologne.de verwendet.

<img alt="02_Cloud-PBX_Start" src="https://user-images.githubusercontent.com/99875470/214311476-0834c659-fe79-4994-a26c-159af36de675.png">

Username/Login: mulheim

Passwort: Hier wird das Passwort des SIP-Benutzers eingetragen. Klicken Sie dann auf "Login".

Im folgenden Fenster wird als Hostname die URL der Cloud PBX eingetragen: xxx.cloudpbx.netcologne.de

<img alt="03_Cloud-PBX_Hostname_a" src="https://github.com/NetCologne/cloudpbx-docs/assets/99875470/fa0c64a2-b437-42a6-adfc-77026e718ec7">

Auf der nächsten Seite muss das Häkchen für optionale Angaben gesetzt werden und Angaben zur Authentifizierung und zum outbound proxy eingetragen werden.

Authentication username: mulheim@xxx.cloudpbx.netcologne.de

Outbound proxy: xxx.cloudpbx.netcologne.de

<img alt="05_Cloud-PBX_Authentication_Out-Proxy_a" src="https://github.com/NetCologne/cloudpbx-docs/assets/99875470/d430b022-1778-4fb9-a6f4-94ed6bcc83b7">

Im nächsten Schritt erkennt der SIP Client automatisch die Verschlüsselung über TLS.

<img alt="06_Cloud-PBX_SIP-TLS" src="https://user-images.githubusercontent.com/99875470/214319317-e9cf571f-9ce4-4377-b64d-852fb9049076.png">

Diese Seite muss mit klicken auf "Next" bestätigt werden.

Die Grundeinstellungen wurden nun vorgenommen. Allerdings müssen noch ein paar Details angepasst werden.

Durch Auswahl des neu angelegten Accounts erreichen Sie die Seite für die Einstellungen.

<img alt="08_Cloud-PBX_Feinheiten_nachjustieren_a" src="https://github.com/NetCologne/cloudpbx-docs/assets/99875470/6d796ad7-1cc9-4cef-8958-1decf7565af4">

Oben rechts schalten Sie mit "advanced" die erweiterten Einstellungen frei.

<img alt="09_Cloud-PBX_Advanced_a" src="https://github.com/NetCologne/cloudpbx-docs/assets/99875470/04dae346-fa60-4820-a812-f14a6fb99edd">

Im Abschnitt "Features" werden die gewünschten Leitungsmerkmale angehakt.

<img alt="10_Cloud-PBX_Features" src="https://user-images.githubusercontent.com/99875470/214569579-c4e7f8f4-1db0-4610-9b38-fa8987aed09e.png">

"Register on startup" sorgt dafür, dass sich der Client sofort beim Starten an der Cloud PBX registriert. Erst mit der Registrierung sind Gespräche möglich.

"Subscribe presence" muss aktiviert werden, wenn Sie den Status anderer Teilnehmer der Cloud PBX in Ihrem Client angezeigt bekommen wollen. Voraussetzung dafür ist, dass die anderen Teilnehmer ihren Status veröffentlichen (publish presence). Der Status der anderen Teilnehmer wird im Telefonbuch angezeigt (siehe Abschnitt "Telefonbuch").

"Publish presence" muss aktiviert werden, wenn Sie Ihren Status in der Cloud PBX bekannt geben wollen.

"Use BLF" muss aktiviert sein, damit der Status eines Teilnehmers in der Cloud in Ihrem Telefonbuch angezeigt wird (siehe auch Abschnitt "Telefonbuch").

Unter "Number Rewriting" sorgt der Haken bei "Strip dial chars" dafür, dass die aufgeführten Sonderzeichen vor dem Wählen der Rufnummer entfernt werden. Das ist u.a. wichtig, wenn Sie im Telefonbuch diese Sonderzeichen im Rufnummernfeld verwenden.

<img alt="11_Cloud-PBX_number_rewriting" src="https://user-images.githubusercontent.com/99875470/214571826-35e7cba6-9fbb-4039-83cc-1f9309b76589.png">

In den Einstellungen für "Pre-configured Extensions" wird im Feld "Check voicemail" 2000 eingetragen. Damit wird das Brief-Symbol in der Benutzeroberfläche so eingestellt, dass mit einem Klick darauf der interne Anrufbeantworter abgefragt werden kann.

Bei den "Compatibility modes" werden vornehmlich die Einstellungen für DTMF vorgenommen.

"DTMF mode": Use DTMF RFC-2833

"Send KPML (Cisco Unified Communications Manager)" muss aktiviert sein, damit bei der Abfrage des interenen Anrufbeantworters die Ziffern (DTMF) richtig übertragen werden. Andernfalls ist eine Navigation im Anrufbeantworter nicht möglich.

<img alt="12_Cloud-PBX_pre-conf-ext_compat-modes" src="https://user-images.githubusercontent.com/99875470/214579241-84d6f555-0399-4017-a4b9-c76e428a0fb9.png">

In dem nun folgenden Abschnitt "Network related" können die Einstellungen übernommen werden. Zur Sicherheit sollten Sie aber die Parameter mit dem Bild vergleichen.

<img alt="13_Cloud-PBX_network-related" src="https://user-images.githubusercontent.com/99875470/214589492-22a247a6-5b62-48ce-aff8-d31c6fc2109f.png">

Bei den "Audio codecs" sollten nur die wirklich notwendigen ausgewählt werden. Das Bild zeigt die empfohlene Auswahl.

<img alt="14_Cloud-PBX_audio-codecs" src="https://user-images.githubusercontent.com/99875470/214590112-73a39f02-df4b-4627-a3a1-253c48c88e64.png">

Für die Verschlüsselung ist kein Zertifikat erforderlich. Bei "SRTP key negotiation" muss "SDES" ausgewählt werden.

<img alt="15_Cloud-PBX_encryption" src="https://user-images.githubusercontent.com/99875470/214590988-f4fe286a-bd6e-48ab-a0b8-b5b2fb0108c1.png">

Damit ist die Grundkonfiguration abgeschlossen.


### Telefonbuch

An dieser Stelle werden nur die Einstellungen erläutert, die für die Statusanzeige erforderlich sind. Die allgemeine Bedienung des Telefonbuchs kann der Dokumentation des Herstellers entnommen werden.

Wie oben bereits erwähnt, erfolgt die Statusanzeige (Busylamp Field) im Zusammenhang mit Einträgen im Telefonbuch. Das bedeutet, dass die Nebenstelle der Cloud PBX, deren Status der Teilnehmer sehen möchte, im Telefonbuch eingetragen sein muss.

Am Beispiel des Teilnehmers "chorweiler" wird hier die Konfiguration dargestellt.

<img alt="18_Cloud-PBX_contact" src="https://user-images.githubusercontent.com/99875470/214605449-f091ac25-87ba-44fd-8787-627720d985c6.png">

Die ersten fünf Einträge enthalten Angaben zum Kontakt. Als Beispiel ist hier nur das Feld "First name" belegt. Grundsätzlich können die Felder nach Belieben ausgefüllt werden, da sie nur für die Anzeige in der Benutzeroberfläche relevant sind.

Um die Rufnummer bzw. den Benutzernamen des Kontaktes einzutragen, klicken Sie auf "Add an additional field", wählen als "Field type" Phone aus und bestätigen mit "add".

<img alt="19_Cloud-PBX_add_phone" src="https://user-images.githubusercontent.com/99875470/214609391-255fecb9-6aa4-4f8e-8203-7a69d3cfd4af.png">

In dem Kontakt erscheinen dann die weiteren Felder "Phone", "Dial account" und "Presence account".

"Phone": Hier wird der Benutzername der gewünschten Nebenstelle eingetragen (auf die richtige Schreibweise achten).

"Dial account": Das ist der Account, der für abgehende Gespräche verwendet werden soll. Wenn in dem Zoiper Client nur ein Account eingerichtet ist, kann die Einstellung auf "Default account" bleiben. Andernfalls wählen Sie einen anderen Account aus dem Aufklappmenü aus.

"Presence account": Hier wird "Contact service account" ausgewählt.

Beim Verlassen des Kontakt-Fensters das Speichern der Daten bestätigen.

In der Benutzeroberfläche steht unter "Contacts" jetzt mindestens der Eintrag "chorweiler". Sobald die Nebenstelle "chorweiler" angerufen wird, wird das in der Benutzeroberfläche durch ein Glockensymbol an dem Kontakt dargestellt.

<img alt="16_Cloud-PBX_BLF-ringing_a" src="https://github.com/NetCologne/cloudpbx-docs/assets/99875470/01f03270-2675-453b-bf4c-bd38eaae24e2">

Ein bestehendes Gespräch ist an dem Hörer-Symbol neben dem Kontakt erkennbar.

<img alt="17_Cloud-PBX_BLF-speaking_a" src="https://github.com/NetCologne/cloudpbx-docs/assets/99875470/ef73b3c4-abc8-48f7-963e-f581f9f1a690">

### Pick-up

Um Pick-up zu ermöglichen, muss im entsprechenden Telefonbucheintrag ein zusätzliches Feld erstellt werden. Klicken Sie auf "add an additional field". Im nun geöffneten Fenster wählen Sie als Field type "Custom" aus und tragen in Custom type z.B. "pick-up" ein.

<img alt="Cloud-PBX_add_pick-up_1" src="https://github.com/NetCologne/cloudpbx-docs/assets/99875470/5c365fd7-f606-4725-abb8-b23d4270eff9">

Klicken Sie auf Add um das Fenster zu schließen.

Nun tragen Sie als Ziel \*99\*chorweiler ein.

<img alt="Cloud-PBX_add_pick-up_2b" src="https://github.com/NetCologne/cloudpbx-docs/assets/99875470/0bdf373e-e58d-45f0-a88b-ede80b284c04">

Beim Verlassen des Kontakt-Fensters das Speichern der Daten bestätigen. 

### Ninja Pro

Für die Verwendung mit der Cloud PBX ist die kostenpflichtige Version erforderlich, da nur diese die notwendige Verschlüsselung mit TLS und SRTP unterstützt. Ein positiver Nebeneffekt ist, dass der Client ein Plugin für Outlook enthält, welches bei der Installation automatisch installiert wird.

Die aktuelle Version laden Sie am besten direkt vom Hersteller herunter: https://www.globaliptel.com/Contents/Products/Software/Ninja-Pro-(CTI).html
Zur Installation des Clients folgen Sie der Anleitung des Herstellers.

### Konfiguration

Die folgende Beschreibung führt Sie durch die grundlegende Konfiguration für die Cloud PBX. Dazu starten Sie zuerst den Ninja Client.

<img alt="05_Konfig_GUI_mit_Pfeil" src="https://user-images.githubusercontent.com/99875470/215804545-3f80961a-91f8-49a0-bd63-1256e8d05d6b.png">

Mit einem Klick auf das kleine Zahnrad (siehe Bild) öffnen Sie die Einstellungen.

Wir beginnen mit dem Reiter "Proxy". Hier müssen die Angaben für den Proxy Server und die Anmeldedaten für den Subscriber eingetragen werden. Als Muster wird hier der Subscriber "mulheim" in der Domain "firmaid.cloudpbx.netcologne.de" verwendet.

**Proxy Server**

Aktiv: ja (Damit wird festgelegt, dass dieser Account aktiv sein soll und der sich der subscriber in der Cloud PBX registriert.)

Proxy Bezeichnung: Hier können Sie nach Belieben eine Bezeichnung wählen. Sie dient lediglich der Verwaltung der Zugangsdaten.

Domain/Realm: die für Ihre Cloud PBX festgelegte Domain, hier als Beispiel: firmaid.cloudpbx.netcologne.de

Proxy Server: gleich der Domain, hier: firmaid.cloudpbx.netcologne.de

SIP Port: 5061

Reregistrierung: 300

Outbound Proxy: gleich der Domain, hier: firmaid.cloudpbx.netcologne.de

Outbound Proxy Port: 5061


**Anmeldedaten**

Angezeigter Name: Hier können Sie nach Belieben einen Namen wählen. Sinnvoll ist z.B. den Namen des Benutzers zu verwenden: mulheim

Benutzername: Hier muss der Name eingetragen werden, mit dem der subscriber in der Cloud PBX angelegt wurde: mulheim

Kennwort: das zum oben eingerichteten Benutzer vergebene Passwort

Auth User: der vollständige Benutzer, bestehend aus dem oben eingerichteten Benutzernamen und der Domain: mulheim@firmaid.cloudpbx.netcologne.de

Anonym: Diese Einstellung entscheidet darüber, ob der Teilnehmer immer anonym (mit unterdrückter Rufnummer) telefonieren soll.

<img alt="06_Konfig_Proxy" src="https://user-images.githubusercontent.com/99875470/215814488-b64d98f3-54db-4234-bda4-c13a0929e176.png">


**Anrufbeantworter**

Wenn Sie den Anrufbeantworter des Ninja Clients verwenden wollen, informieren Sie sich über die Bedienung bitte in der online bei Global IP verfügbaren Anleitung.

Wenn Sie den internen Anrufbeantworter der Cloud PBX verwenden, erfolgt die Aktivierung durch Feature Codes. Die Beschreibung dazu finden Sie im Kapitel "Anrufbeantworter (Voicemail)" https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufbeantworter/.

Um die Abfrage des internen Anrufbeantworters der Cloud PBX zu erleichtern, kann in diesem Reiter die Rufnummer zur Abfrage voreingestellt werden. In der Cloud PBX ist das die 2000.

<img alt="07_Konfig_Anrufbeantworter" src="https://user-images.githubusercontent.com/99875470/216052862-472cbcba-483c-4ff3-ba07-93e055f71d24.png">


**Presence**

Der Ninja Client kann innerhalb der Cloud PBX seinen Zustand anzeigen (Presence). Damit kann an anderen Nebenstellen z.B. angezeigt werden, ob die Nebenstelle gerade besetzt ist (Busy Lamp Field). In umgekehrter Richtung kann der Client auch den Zustand anderer Nebenstellen anzeigen, wenn diese ihren Zustand kundtun.

Presence: Der Client teilt den eigenen Status mit, wenn "ja" ausgewählt wird.

Besetztlampenfeld (BLF): "Ja" einstellen, um den Status anderer Nebenstellen anzuzeigen (siehe auch Abschnitt "Schnellwahl")

Gültigkeitsspanne: 300

<img alt="08_Konfig_Presence" src="https://user-images.githubusercontent.com/99875470/216058173-cbaa7d2b-30c6-479f-892a-660be6a26a35.png">


**Wählregeln**

Im Reiter Wählregeln wird das Präfix für "Gespräch heranholen" (pickup) eingetragen. Damit können Anrufe, die zu einem Teilnehmer, der in der Schnellwahl (siehe unten) eingetragen ist, per doppeltem Mausklick herangeholt werden. Details zur Bedienung finden Sie in der Hilfe des Ninja Clients.

PickUp Präfix: \*99\*

<img alt="09_Konfig_Waehlregeln" src="https://user-images.githubusercontent.com/99875470/222443929-08320d6d-5dcd-4265-8e5c-274bc25650ee.png">


**Sicherheit**

In diesem Reiter wird die Verschlüsselung für SIP und SRTP eingestellt.

Verschlüsselung/Sicherheit: SRTP/TLS

Verschlüsselung aktiviert: ja

TLS Port: 5061

SAVP: ja

<img alt="10_Konfig_Sicherheit" src="https://user-images.githubusercontent.com/99875470/216073341-4c3f30a0-f0d0-4327-9969-b897fbdf21cf.png">

Wenn alle Einstellungen vorgenommen wurden und der Client den TLS-Handshake durchlaufen hat, wird auch das Zertifikat im entsprechenden Feld angezeigt.

<img alt="10a_Konfig_Sicherheit" src="https://user-images.githubusercontent.com/99875470/216074133-b83ee4fc-e165-459e-a9a7-b917fdb33930.png">


**Erweitert**

Unter "Erweitert" werden nur Anpassungen bei den Audio Codecs und bei DTMF vorgenommen. Alle anderen Einstellungen bleiben auf ihren voreingestellten Werten.

Audio Codecs: G711a, G711u, GSM, G729a, iLBC (nur die hier aufgeführten Codecx auswählen und in der dargestellten Reihenfolge anordnen)

DTMF: Auto (erforderlich, damit im internen Anrufbeantworter der Cloud PBX navigiert werden kann)

<img alt="11_Konfig_Erweitert" src="https://user-images.githubusercontent.com/99875470/216076028-4e52a38a-a98b-4a49-a950-1e7b46dffa71.png">

Damit sind die Einstellungen für den SIP Proxy und den Benutzer, d.h. die Nebenstelle der Cloud PBX, abgeschlossen.

Vor Verwendung der "Busy Lamp Field" (BLF) sind noch Einstellungen im Menü "Schnellwahl" erforderlich.

<img alt="15_Konfig_Schnellwahl_mit Markierung" src="https://user-images.githubusercontent.com/99875470/216563700-271c51ac-4282-4dcf-844d-e4cd3f10c7b9.png">

Fensterposition: Wählen Sie aus dem Menü die für Sie passende Position des Schnellwahlfensters auf dem Monitor.

Immer Anzeigen: Wählen Sie "ja", wenn das Schnellwahlfenster immer angezeigt werden soll. Alternativ können Sie das Fenster auch manuell mit der Funktionstaste F9 ein- und ausblenden.

Bei Transfers anzeigen: Auch hier wählen Sie die für Sie angenehmste Einstellung aus.

Immer im Vordergrund: Wenn Sie "ja" auswählen, bleibt das Fenster immer im Vordergrund und überdeckt ggf. andere Fenster. Wählen Sie die für Sie günstigste Einstellung aus.

Im folgenden Beispiel ist der Teilnehmer "chorweiler" in der Schnellwahl aufgeführt.

<img alt="Ninja_Schnellwahlfeld" src="https://user-images.githubusercontent.com/99875470/216581414-28243395-dcd6-4f1a-8e59-2c584a8d97e1.png">

Sobald dieser Teilnehmer angerufen wird, erscheint in der Liste ein orangenes Feld. Daneben wird die Nummer des Anrufers angezeigt.

<img alt="16_Schnellwahl_ringing_geschwaerzt" src="https://user-images.githubusercontent.com/99875470/216582503-2dc99b8b-e885-47e8-9418-433b5556a1b3.png">

Wenn der Teilnehmer das Gespräch annimmt, wechselt die Anzeige von orange zu rot und die Rufnummer des Anrufers verschwindet.

<img alt="17_Schnellwahl_speaking" src="https://user-images.githubusercontent.com/99875470/216583054-60bb5f5e-9488-4592-b3fa-7e05903bcc5b.png">

## Baresip+
<img alt="baresip-einrichtung-1-4" src="https://github.com/user-attachments/assets/18521647-5a4c-4e43-8ac0-c360cb8eeb63" />
<img alt="baresip-einrichtung-5-7" src="https://github.com/user-attachments/assets/555163a3-3746-4d63-a401-0e439a2a2163" />

## WaveLite
<img alt="wavelite-einrichtung-1-4" src="https://github.com/user-attachments/assets/ac1727e8-6ed0-4548-81d1-5a2423425e99" />
<img alt="wavelite-einrichtung-5-7" src="https://github.com/user-attachments/assets/9f079ce6-7ae5-4215-8ecd-18143abb690a" />


# Übersicht der Softphones und ihrer Leistungsmerkmale

<img alt="table" src="https://github.com/user-attachments/assets/e5c6fc22-6c04-4d7e-9fe0-1d79b88fb695" />
