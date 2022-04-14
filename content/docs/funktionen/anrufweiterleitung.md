---
title: "Anrufweiterleitung"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "funktionen"
weight: 402
toc: true
---

Mit der Cloud PBX können Sie Ihre Verfügbarkeit für eingehendene Anrufe automatisch erhöhen, indem sie diese an andere Ziele weiterleiten. Nutzen Sie dazu die Funktion *Anrufweiterleitung / Call-Forward*. Diese können Sie für jede Nebenstelle/Rufnummer individuell einstellen.

Klicken Sie zunächst auf den Menuepunkt *Kunden-Details [1]*, dann auf *Subscriber [2]* und bei der betreffenden Nebenstelle (hier zollstock) auf *Einstellungen [3]*. 

![Anrufmenue_Aktivierung1](https://user-images.githubusercontent.com/98753538/161692092-8885b079-3d9e-4b35-be48-31ad5b803f99.jpg)

Öffenen Sie nun das Menue *Call-Forwards* (1 im Bild unten) und entscheiden, bei welcher Bedingung die *Anrufweiterleitung* greifen soll. 

### Call Forward Typen

Bei registrierter Nebenstelle sind dabei drei Fälle üblich (grün):

 * *Call Forward Unconditional* - generelle Anrufweiterleitung. Bitte beachten Sie, dass sich "generell" nur auf die *registrierte Nebenstelle* bezieht. Wenn Sie auch für diesen Fall eine Anrufweiterleitung wünschen, fügen Sie einfach *Call Forward Unavailable* (gelb) hinzu.
 * *Call Forward Busy* - Anrufweiterleitung, wenn besetzt
 * *Call Forward Timeout* - Anrufweiterleitung nach eine bestimmten Zeitspanne
  
 ![Anrufmenue_Auswahl Call Fowards2](https://user-images.githubusercontent.com/98753538/161062432-8a60e0e0-83ac-46ff-876a-e1bb67cc1e24.jpg)

Der Sonderfall *Call Forward Unavailable* (gelb) kommt zum Tragen, falls die Nebenstelle nicht registriert und damit nicht erreichbar ist. <br>
Mit einem Klick auf den Button "Edit" (2) gelangen Sie zu den unterschiedlichen Call-Forward...

### Destinationen

![Call Forward Destinations1](https://user-images.githubusercontent.com/98753538/163186900-64c4af17-b174-4d58-8dc9-36734d01591f.jpg)

Aktuell können Sie zu sieben verschiedene Zielen/Destinationen (1) weiterleiten:

* Voicemail - Der Anrufer erhält eine Ansage und kann dem Empfänger eine Audionachricht hinterlassen.
* Conference - Wird hierhin weitergeleitet, werden die Anrufer in einer Konferenz zusammengeschaltet, um gleichzeitig mit drei, vier oder mehr Personen sprechen zu können.
* Fax2Mail - Eine Nebenstelle wird als Fax genutzt und ankommende Calls (besser: Faxe) werden dorthin geleitet und als E-Mail ausgegeben. Sehen Sie hierzu auch [FAX](https://cloudpbx-doku.netcologne.de/docs/funktionen/fax/).
* Auto Attendant - Anrufer werden zu einem Anrufmenü weitergeleitet, das die Funktion einer automatische Telefonzentrale übernimmt. Die Details stehen unter [Anrufmenü](https://cloudpbx-doku.netcologne.de/docs/pbx-konfiguration/anrufmenue/).
* Office Hours Announcement - Hier bekommen Anrufer die Geschäfts-/Öffnungszeiten mitgeteilt, d.h. es sollte immer außerhalb dieser Zeiten dorthin weitergeleitet werden.
* Custom Announcement - Hier kann auf eine individuelle kundenspezifische Ansage weitergeleitet werden.
* URI/Number - Weiterleitung zu einer konkreten Rufnummer, die so eingetragen wird, wie man wählen würde, d.h. mit "0", fall eine "Amtsholung" erforderlich ist.

Für die Aktivierungn ist das Häkchen bei Enabled (2) erfoderlich. Mit dem SAVE-Button (3) werden die Einstellungen gespeichert. Der ADVANCED VIEW (4) bietet Ihnen zusätzliche Funktionen:



