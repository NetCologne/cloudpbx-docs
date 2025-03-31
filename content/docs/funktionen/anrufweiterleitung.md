---
title: "Rufumleitungen"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "funktionen"
weight: 470
toc: true
---

Mit der Cloud PBX können Sie Ihre Verfügbarkeit für eingehendene Anrufe automatisch erhöhen, indem sie diese an andere Ziele weiterleiten. Nutzen Sie dazu die Funktion *Rufumleitung(en)*. Diese können Sie für jede Nebenstelle/Rufnummer oder Gruppe individuell einstellen. Dies ist auf mehreren Wegen möglich:

## 1. Einrichtung in der Cloud PBX über das Web-Interface (Admin)

Um eine Rufumleitung einzurichten, wählt der **Admin** innerhalb der PBX-Konfiguration den Unterpunk *Nebenstelle [1]* oder *Gruppe [2]* und trifft dort seine Auswahl - hier *Nebenstelle kalk*. Dann klickt er auf den Reiter *Rufumleitungen* (roter Pfeil):

![Rufumleitung1](https://github.com/user-attachments/assets/9a882997-a0f4-4e7a-8f9b-8f6bcea4f4da)

## 2. Einrichtung in der Cloud PBX über das Web-Interface (Anwender)

Klicken Sie im Menü der Nebenstelle (hier Kalk) auf den Punkt *Anrufeinstellungen* und dann auf *Rufumleitung* (roter Pfeil)

![Rufumleitung8](https://github.com/user-attachments/assets/2e9be969-ce4a-4f26-a9c9-a12af3257211)


## RUFUMLEITUNG

Nun *+ RUFUMLEITUNG HINZUFÜGEN* klicken und den Status der Nebenstelle auswählen, bei dem die Rufumleitung erfolgen soll:<br>
*Wenn verfügbar*, *Wenn nicht verfügbar (Nebenstelle ist nicht registrtiert)* oder *Wenn besetzt*:

![Rufumleitung2](https://github.com/user-attachments/assets/0b69de97-6432-498a-b64e-9c05185bdec0)

Anschließend können Sie noch eine weitere Bedingung, die sich auf den Anrufer, ein Datum oder einen bestimmten Zeitraum bezieht, hinzufügen. Bei *Anruf von* können Sie entweder eine Nummernliste oder einzelne Rufnummern eingeben, für die diese Rufumleitung erfolgen soll (Whitelist-Funktion). Möchten Sie bestimmte Rufnummern ausschließen und alle anderen Anrufer sollen umgeleitet werden, verwenden Sie das Feld *Anruf nicht von*.

![Rufumleitung3](https://github.com/user-attachments/assets/9cdac053-bc3d-437d-be2e-c523739144bc)

Sie können auch eine zeitliche Bedingung wie ein Datum oder einen Zeitraum definieren, an/in dem ankommende Rufe umgeleitet werden sollen.

![Rufumleitung4](https://github.com/user-attachments/assets/44d0bc17-948e-45c1-a86e-a8fe30f8b798)

Auch *Bürozeiten* sind möglich.

![Rufumleitung5](https://github.com/user-attachments/assets/eda771fc-aada-4fbf-841b-00e626464dad)


## Ziele der Rufumleitung

Im Standardfall wird an eine einzutragende Rufnummer umgeleitet. Durch Klick auf das Drei-Punkte-Symbol (roter Pfeil) öffnet sich das Menü mit sämtlichen Möglichkeiten der Rufumleitung:

![Rufumleitung6](https://github.com/user-attachments/assets/cfe5a15d-1319-44c3-95d3-68ffac54122f)
In diesem Beispiel erfolgt die Rufumleitung, wenn die Nebenstelle "nicht verfügbar" und Samstag oder Sonntag ist.

Die angeführten Möglichkeiten sind weitgehend selbsterklärend: <br>
* **An Rufnummer weiterleiten** - Weiterleitung zu einer konkreten Rufnummer, die so eingetragen wird, wie man sie wählen würde, d.h. mit “0”, fall eine “Amtsholung” erforderlich ist. <br>
* **An Anrufbeantworter weiterleiten** - Der Anrufer erhält eine Ansage und kann dem Empfänger eine Audionachricht hinterlassen. <br>
* **Zu Konferenz weiterleiten** - Wird hierhin weitergeleitet, werden die Anrufer in einer Konferenz zusammengeschaltet, um gleichzeitig mit drei, vier oder mehr Personen sprechen zu können. <br>
* **Zu Fax2Mail weiterleiten** - Eine Nebenstelle wird als Fax genutzt und ankommende Calls (besser: Faxe) werden dorthin geleitet und als E-Mail ausgegeben. Sehen Sie hierzu auch [FAX](https://cloudpbx-doku.netcologne.de/docs/funktionen/fax/). <br>
* **Weiterleiten an Geschäftsführungssekretariat** <br>
* **Weiterleiten zur individuellen Ansage** - Hier kann auf eine individuelle kundenspezifische Ansage weitergeleitet werden. <br>
* **Weiterleitung an das Anrufmenü** (engl: Auto Attendant) - Anrufer werden zu einem Anrufmenü weitergeleitet, das die Funktion einer automatische Telefonzentrale übernimmt. Die Details stehen unter [Anrufmenü](https://cloudpbx-doku.netcologne.de/docs/pbx-konfiguration/anrufmenue/). <br>
* **Weiterleitung zur Bürostundenansage** - Hier bekommen Anrufer die Geschäfts-/Öffnungszeiten mitgeteilt, d.h. es sollte immer außerhalb dieser Zeiten dorthin weitergeleitet werden. <br>
* Weiterleitung an Calling Card <br>
* Weiterleiten zu Call Through <br>
* Weiterleitung an lokalen Teilnehmer <br>

Am Ende gibt es noch je einen Schalter zum Deaktivieren und Entfernen/Löschen der Rufumleitung. 

Beliebte Anwendungen sind die Weiterleitung zu einer (bestimmmten) **Rufnummer**, zu einem **Anrufbeantworter**, an das **Anrufmenü** oder zur **Bürostundenansage**. 
Sehr oft wird auch die Hauptnummer selbst ausgewählt und eine Umleitung zu einer weiteren Nummer eingerichtet. Dabei kann die Klingelzeit vorm Umleiten gesetzt werden.

![Rufumleitung7](https://github.com/user-attachments/assets/0a2f7d00-cd35-45ee-ae8c-3c622ad01d32)

Auch ist es möglich eine weitere Umleitung (hier zum Anrufbeantworter) hinzuzufüngen. Hat man sich “verklickt” kann man die Fehlkonfiguration mit den drei Punkten rechts (unten) entfernen.


## Rufumleitung Beispiel

Denkbar ist, dass es zu Bürozeiten erst bei einer Nebenstelle oder Gruppe kurz klingelt (hier: 5 Sekunden) und dann die Umleitung zu  einem Anrufbeantworter erfolgt, wo der Anrufer eine Nachricht hinterlassen kann. In der anderen Zeit wird (nach kurzem Klingeln) zu einer Ansage mit den Bürozeiten umgeleitet:

![Rufumleitung Beispiel](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/79753702-75f0-4b69-8e44-403b34f76e6a)

### Besonderheit: Rufumleitung in der PBX-Gruppe

Standardmäßig werden Rufumleitungen beim Anrufen einer Gruppe ignoriert. Die entsprechende Kundeneinstellung befindet sich für den **Admin** unter *PBX-Konfiguration* -> *Kundenpräferenzen*:

![Rufumleitung9](https://github.com/user-attachments/assets/f2502bd9-5ce4-4d85-a03e-258c862a3c03)

Wenn Sie dennoch eine Rufumleitung bei einer Nebenstelle/Gruppe einrichten möchten, können Sie hier die Funktion *ausklicken* (Schaltknopf nach links -> wird weiß). 

Soll die Rufumleitung aber bei einer bestimmten Nebenstelle dennoch ignoriert werden, so kann man diese auswählen und ihre *Einstellungen* anpassen.

![Rufumleitung10](https://github.com/user-attachments/assets/209f784a-280e-4f00-b37a-07a8956feeb2)

Dafür einfach bei *Anrufweiterleitung bei Anrufen . . . ignorieren* den Schiebeschalter aktivieren (nach rechts -> wird grün):

![Rufumleitung11](https://github.com/user-attachments/assets/334246ec-933d-458c-ad3b-843aae64a182)

Ist bei der Nebenstelle/Gruppe der Schalter zum *Ignorieren der Rufumleitung* deaktiviert, greift die übergeordnete Einstellung des Kunden (s.o. Kundenpräferenzen).


## 3. Einrichtung in der Cloud PBX über das Endgerät (Anwender)

Die einzelnen [Call Forward Typen](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/#call-forward-typen) können durch Eingabe der einzelnen Feature Codes direkt am Endgerät aktiviert werden:

*Call Forward Unconditional:* Einrichtung der generellen Rufumleitung durch Wahl von **\*72*Zielrufnummer** (inkl. Amtsholung) – *Deaktivierung durch Wahl von #72*.

*Call Forward on Busy:* Einrichtung der Rufumleitung bei Besetzt durch Wahl von **\*90*Zielrufnummer** (inkl. Amtsholung) – *Deaktivierung durch Wahl von #90*.

*Call Forward on Timeout:* Einrichtung der Rufumleitung nach Zeit durch Wahl von **\*92*30*Zielrunfummer** (hier also nach 30 Sekunden) – *Deaktivierung durch Wahl von #92*.

*Call Forward on Not Available:* Einrichtung der Rufumleitung bei „Nicht Registriert“ durch Wahl von **\*93*Zielrufnummer** - *Deaktivierung durch Wahl von #93*.

Die **Deaktivierung aller** eingerichteten Anrufweiterschaltungen erfolgt über den Feature Code **#96**.


## 4. Besonderheit: Einrichtung der Rufumleitung im Endgerät (Anwender)

Viele Endgeräte bieten in ihren Menüs ebenfalls die Möglichkeit eine Rufumleitung einzurichten und per Tastendruck zu aktivieren. Z.B. bei *Yeahlink* wählen Sie dafür den Menüpunkt **Leistungsmerkmale**:

![yealink hauptmenue](https://github.com/user-attachments/assets/9d434406-310d-4f17-be94-95b177106682)

Tippen Sie anschließend auf **Weiterleitung** und wälen Sie die gewünschte Art der Rufumleitung: <br>
 **Immer weiterleiten** - Eingehende Anrufe werden umgehend umgeleitet. <br>
 **Weiterleiten bei besetzt** - Eingehende Anrufe werden umgeleitet, wenn die Leitung besetzt ist. <br>
 **Bei Abwesenheit** - Eingehende Anrufe werden umgeleitet, falls sie innerhalb einer bestimmten Zeit nicht entgegengenommen werden. <br>

Geben Sie anschließend die Zielnummer ein, auf die Sie umleiten möchten und tippen im Bildschirm auf Speichern/Save, um die Änderungen zu übernehmen.

>💡**Hinweis**
> Die hier beschriebene Rufumleitung ist nur im Endgerät konfuguriert und auch nur hier zu aktivieren bzw. deaktivieren. Die Einstellungen Ihrer Cloud PBX bleiben davon unberührt.


### 5. Auslaufend: Konfiguration in der Cloud PBX unter "Kundendetails"

Darüberhinaus kann der Admin unter dem Punkt *Kunden-Details* sowohl für einzelne Teilnehmer (Subscriber) oder auch bei PBX-Gruppen Rufumleitungen einrichten:

![Rufumleitung Admin2](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/34a9798b-c80d-4464-b62c-c89c238bb781)

#### a) Anrufweiterleitung Subscriber

Klicken Sie zunächst auf den Menuepunkt *Kunden-Details [1]*, dann auf *Subscriber [2]* und bei der betreffenden Nebenstelle (hier zollstock) auf *Einstellungen [3]*. 

![Anrufmenue_Aktivierung1](https://user-images.githubusercontent.com/98753538/161692092-8885b079-3d9e-4b35-be48-31ad5b803f99.jpg)

Öffnen Sie nun das Menue *Call-Forwards* (1 im Bild unten) und entscheiden, bei welcher Bedingung die *Anrufweiterleitung* greifen soll. 

#### b) Anrufweiterleitung Gruppe

Klicken Sie zunächst auf den Menuepunkt *Kunden-Details [1]*, dann auf *PBX-Gruppen [2]* und bei der betreffenden Gruppe (hier schal-sick) auf *Einstellungen [3]*. 

![Anrufmenue_Aktivierung_Gruppe](https://user-images.githubusercontent.com/98753538/186081568-6a5c2f03-85f0-486b-8ae8-c62b62a73bbc.jpg)

Öffnen Sie nun das Menue *Call-Forwards* (1 im Bild unten) und entscheiden, bei welcher Bedingung die *Anrufweiterleitung* greifen soll. 

#### Call Forward Typen

Bei registrierter Nebenstelle sind dabei drei Fälle üblich (grün):

 * *Call Forward Unconditional* - generelle Anrufweiterleitung. Bitte beachten Sie, dass sich "generell" nur auf die *registrierte Nebenstelle* bezieht. Wenn Sie für eine nicht registrierte Nebenstelle eine Anrufweiterleitung wünschen, fügen Sie einfach Call Forward Unavailable (gelb) hinzu. Oder, wenn sie ganz sicher gehen wollen, dass die Anrufweiterleitung immer greift, aktivieren sie beide Weiterleitungstypen.
 * *Call Forward Busy* - Anrufweiterleitung, wenn besetzt
 * *Call Forward Timeout* - Anrufweiterleitung nach einer bestimmten Zeitspanne
  
 ![Anrufmenue_Auswahl Call Fowards2](https://user-images.githubusercontent.com/98753538/161062432-8a60e0e0-83ac-46ff-876a-e1bb67cc1e24.jpg)

Der Sonderfall *Call Forward Unavailable* (gelb) kommt zum Tragen, falls die Nebenstelle nicht registriert und damit nicht erreichbar ist. <br>
Mit einem Klick auf den Button "Edit" (2) gelangen Sie zu den unterschiedlichen Call-Forward...

#### Destinationen

![Call Forward Destinations1](https://user-images.githubusercontent.com/98753538/163390500-eaff73a8-60c1-4758-864b-69139d16c79e.jpg)

Aktuell können Sie zu sieben verschiedene Zielen/Destinationen (1) weiterleiten:

* Voicemail - Der Anrufer erhält eine Ansage und kann dem Empfänger eine Audionachricht hinterlassen.
* Conference - Wird hierhin weitergeleitet, werden die Anrufer in einer Konferenz zusammengeschaltet, um gleichzeitig mit drei, vier oder mehr Personen sprechen zu können.
* Fax2Mail - Eine Nebenstelle wird als Fax genutzt und ankommende Calls (besser: Faxe) werden dorthin geleitet und als E-Mail ausgegeben. Sehen Sie hierzu auch [FAX](https://cloudpbx-doku.netcologne.de/docs/funktionen/fax/).
* Auto Attendant - Anrufer werden zu einem Anrufmenü weitergeleitet, das die Funktion einer automatische Telefonzentrale übernimmt. Die Details stehen unter [Anrufmenü](https://cloudpbx-doku.netcologne.de/docs/pbx-konfiguration/anrufmenue/).
* Office Hours Announcement - Hier bekommen Anrufer die Geschäfts-/Öffnungszeiten mitgeteilt, d.h. es sollte immer außerhalb dieser Zeiten dorthin weitergeleitet werden.
* Custom Announcement - Hier kann auf eine individuelle kundenspezifische Ansage weitergeleitet werden.
* URI/Number - Weiterleitung zu einer konkreten Rufnummer, die so eingetragen wird, wie man sie wählen würde, d.h. mit "0", fall eine "Amtsholung" erforderlich ist.

Für die Aktivierung ist das Häkchen bei Enabled (2) erfoderlich. Mit dem SAVE-Button (3) werden die Einstellungen gespeichert. Bei (4) gelangen Sie zum

#### Advanced View

und haben folgende zusätzliche Funktionen, im Beispiel für *Call Forward Unconditional*, also die *generelle Anrufweiterleitung*:

![Call Forward Advanced View1](https://user-images.githubusercontent.com/98753538/163390556-2808d31f-c7e3-4ecb-af22-99a27de53e6e.jpg)

##### during Time Set (1)

Hier können Sie einen oder mehrere Zeiträume eintragen und editieren, in denen die jeweilige Anrufweiterleitung gelten soll.

![Call Forward Time Sets](https://user-images.githubusercontent.com/98753538/163390616-05ac7208-cbc8-490b-bd6b-fc42886fa9ca.jpg)

Dabei können "Von-Bis-Angaben" für die Zeiteinheiten Jahr, Monat, x. Tag im Monat, Wochentag, Stunde und Minute gemacht werden. Dabei muss man beachten, dass man für jede Periode Start- und Ende einzeln definieren muss. Im Beispiel soll die Anrufweiterleitung dienstags und mittwochs jeweils von 10:15 Uhr bis 14:00 und von 15:00 Uhr bis 15:28h erfolgen. Für diese beiden Zeitspannen sind **drei** Eingaben erforderlich:

![Call Forward Time Sets 2](https://user-images.githubusercontent.com/98753538/167443767-2a032485-6ad4-44dc-bfe0-43f95891c81d.jpg)

Bei einer minutengenauen Zeitangabe, die sich dann über mehrere Stunden erstreckt, können also **KEINE klassischen Uhrzeitangaben** gemacht werden: Die begonnene Stunde muss erst mit 59 Minuten beendet und eine neue Periode mi der nächsten vollen Stunde begonnen werden. 
Ein weiteres (einfacheres) Beispiel zeigt die Anrufweiterleitung immer freitags von 11:00 bis 14:00 Uhr:

![Call Forward Time Sets 3](https://user-images.githubusercontent.com/98753538/167446097-88a32ea3-8e87-4800-9d4e-c02aec00fb4e.jpg)

##### from Source Set (2)

Sie möchten, dass Ihre Kunden im Ortsnetz Köln (0221) eine andere Ansage erhalten als die aus Bonn (0228), dann definieren Sie unterschiedliche Source Sets. Denkbar wäre auch eine Ansage in Englisch für internationale Kunden (002 bis 009). Bei jedem *Source Set* können Sie wählen, ob Sie mit einer *Whitelist (zulässige Rufnummern)* oder einer *Blacklist (verbotene Rufnummern)* arbeiten möchten.

![Call Forward Source Set](https://user-images.githubusercontent.com/98753538/163390624-de4f3337-4256-4aca-82e6-2beb4db6702a.jpg)

##### to B-Number Set (3)

Ähnlich wie bei A-Rufnummern für die Urspünge können Sie auch bei den B-Rufnummer, zu denen weitergeleitet werden soll bzw. darf, Unterschiede machen. Denkbar wäre z.B., dass Internationale Ziel nicht erlaubt sind.

![Call Forward B-Number Set](https://user-images.githubusercontent.com/98753538/163390640-8b8ce30c-7837-4d11-9e16-faafb32045fa.jpg)

##### Destination Set (4)

Hier können Sie sämtliche (Call Forward-)Destinationen verwalten oder eine neue hinzufügen.

![Call Forward Destination Sets](https://user-images.githubusercontent.com/98753538/163390656-591fcc5b-a774-449f-8fb1-b27d4001a473.jpg)

Das *Enabled-Häkchen* (5) beim [ADVANCED VIEW](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/#advanced-view) zeigt Ihnen, ob das Set aktiv ist bzw. nicht. Per Mausklick auf "Remove" (6a) löschen Sie ein Set genauso einfach, wie Sie ein neues per Klick auf "Add destination/time sets" (6b) wieder hinzufügen können. Mit dem Button "Simple View" (7) gelangen Sie zurück zur "einfachen" Ansicht. Vergessen Sie nicht die Änderungen mit SAVE (8) zu speichern.

#### Besonderheit: Call-Forward in der PBX-Gruppe

Standardmäßig werden Rufumleitungen (Call-Forward) beim Anrufen einer Gruppe ignoriert. Die entsprechende Einstellung befindet sich unter *Kunden-Details* -> *Einstellungen* -> *Cloud PBX*

![Rufumleitung Ignore Hunting](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/60486160-9feb-439c-9c4c-43ede7e103dc)

Wenn Sie dennoch eine Rufumleitung bei einem Gruppen-Teilnehmer (Subscriber) einrichten möchten, klicken Sie auf *Edit* und entfernen das Häkchen im Feld *Value*. 

Wird dennoch gewümscht, dass die Rufumleitung (Call-Forward) bei einem bestimmten Teilnehmer (Subscriber) ignoriert wird, so kann man diesen unter *Kunden-Details* -> *Einstellungen* -> *Subscriber* auswählen und seine *Einstellungen* anpassen.

![Rufumleitung Subscriber](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/1fc78c90-5618-4500-a81f-6d56db7f9d7e)

Bei den *Einstellungen* den Unterpunkt *Cloud PBX* öffnen.

 ![Rufumleitung Subscriber Cloud PBX](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/a6afcd6f-990e-4ab9-85a7-b7ccfac78dc2)

und das entsprechende Häkchen zum Ignorieren der Rufumleitung (Call Forward) setzen:

![Rufumleitung Subscriber Ignore Hunting](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/a1141e3a-1bc1-4269-925f-f8c1458da1a0)
