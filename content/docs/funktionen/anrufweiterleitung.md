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
*Ständig*, *Wenn nicht verfügbar (Nebenstelle ist nicht registrtiert)* oder *Wenn besetzt*:

![Rufumleitung2](https://github.com/user-attachments/assets/bdf57aaa-d3ee-49f6-a3d9-e86b31d1b340)

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

![yealink rufumleitung](https://github.com/user-attachments/assets/798b66b5-253d-4abe-8310-52c6b109505e)

>⚠️**Wichtig:** <br> 
>Die hier beschriebene Rufumleitung ist nur im Endgerät konfuguriert und auch nur hier zu aktivieren bzw. deaktivieren. Die Einstellungen Ihrer Cloud PBX bleiben davon unberührt.
