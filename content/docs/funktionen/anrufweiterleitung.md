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

 * *Call Forward Unconditional* - generelle Anrufweiterleitung. Bitte beachten Sie, dass sich "generell" nur auf die *registrierte Nebenstelle* bezieht. Wenn Sie für eine nicht registrierte Nebenstelle eine Anrufweiterleitung wünschen, fügen Sie einfach Call Forward Unavailable (gelb) hinzu. Oder, wenn sie ganz sicher gehen wollen, dass die Anrufweiterlieung immer greift, aktivieren sie beide Weiterleitungstypen.
 * *Call Forward Busy* - Anrufweiterleitung, wenn besetzt
 * *Call Forward Timeout* - Anrufweiterleitung nach eine bestimmten Zeitspanne
  
 ![Anrufmenue_Auswahl Call Fowards2](https://user-images.githubusercontent.com/98753538/161062432-8a60e0e0-83ac-46ff-876a-e1bb67cc1e24.jpg)

Der Sonderfall *Call Forward Unavailable* (gelb) kommt zum Tragen, falls die Nebenstelle nicht registriert und damit nicht erreichbar ist. <br>
Mit einem Klick auf den Button "Edit" (2) gelangen Sie zu den unterschiedlichen Call-Forward...

### Destinationen

![Call Forward Destinations1](https://user-images.githubusercontent.com/98753538/163390500-eaff73a8-60c1-4758-864b-69139d16c79e.jpg)

Aktuell können Sie zu sieben verschiedene Zielen/Destinationen (1) weiterleiten:

* Voicemail - Der Anrufer erhält eine Ansage und kann dem Empfänger eine Audionachricht hinterlassen.
* Conference - Wird hierhin weitergeleitet, werden die Anrufer in einer Konferenz zusammengeschaltet, um gleichzeitig mit drei, vier oder mehr Personen sprechen zu können.
* Fax2Mail - Eine Nebenstelle wird als Fax genutzt und ankommende Calls (besser: Faxe) werden dorthin geleitet und als E-Mail ausgegeben. Sehen Sie hierzu auch [FAX](https://cloudpbx-doku.netcologne.de/docs/funktionen/fax/).
* Auto Attendant - Anrufer werden zu einem Anrufmenü weitergeleitet, das die Funktion einer automatische Telefonzentrale übernimmt. Die Details stehen unter [Anrufmenü](https://cloudpbx-doku.netcologne.de/docs/pbx-konfiguration/anrufmenue/).
* Office Hours Announcement - Hier bekommen Anrufer die Geschäfts-/Öffnungszeiten mitgeteilt, d.h. es sollte immer außerhalb dieser Zeiten dorthin weitergeleitet werden.
* Custom Announcement - Hier kann auf eine individuelle kundenspezifische Ansage weitergeleitet werden.
* URI/Number - Weiterleitung zu einer konkreten Rufnummer, die so eingetragen wird, wie man sie wählen würde, d.h. mit "0", fall eine "Amtsholung" erforderlich ist.

Für die Aktivierungn ist das Häkchen bei Enabled (2) erfoderlich. Mit dem SAVE-Button (3) werden die Einstellungen gespeichert. Bei (4) gelangen Sie zum

### Advanced View

und haben folgende zusätzliche Funktionen, im Beispiel für *Call Forward Unconditional*, also eine *generelle Anrufweiterleitung*:

![Call Forward Advanced View1](https://user-images.githubusercontent.com/98753538/163390556-2808d31f-c7e3-4ecb-af22-99a27de53e6e.jpg)

#### during Time Set (1)

Hier können Sie einen oder mehrere Zeiträume eintragen und editieren, in denen die jeweilige Anrufweiterleitung gelten soll.

![Call Forward Time Sets](https://user-images.githubusercontent.com/98753538/163390616-05ac7208-cbc8-490b-bd6b-fc42886fa9ca.jpg)

#### from Source Set (2)

Sie möchten, dass Ihre Kunden im Ortsnetz Köln (0221) eine andere Ansage erhalten als die aus Bonn (0228), dann definieren Sie unterschiedliche Source Sets. Denkbar wäre auch eine Ansage in Englisch für internationale Kunden (002 bis 009). Bei jedem *Source Set* können Sie wählen, ob Sie mit einer *Whitelist (zulässige Rufnummern)* oder einer *Blacklist (verbotene Rufnummern)* arbeiten möchten.

![Call Forward Source Set](https://user-images.githubusercontent.com/98753538/163390624-de4f3337-4256-4aca-82e6-2beb4db6702a.jpg)

#### to B-Number Set (3)

Ähnlich wie bei A-Rufnummern für die Urspünge können Sie auch bei den B-Rufnummer, zu denen weitergeleitet werden soll bzw. darf, Unterschiede machen. Denkbar wäre z.B., dass Internationale Ziel nicht erlaubt sind.

![Call Forward B-Number Set](https://user-images.githubusercontent.com/98753538/163390640-8b8ce30c-7837-4d11-9e16-faafb32045fa.jpg)

#### Destination Set (4)

Hier können Sie sämtliche (Call Forward-)Destinationen verwalten oder eine neue hinzufügen.

![Call Forward Destination Sets](https://user-images.githubusercontent.com/98753538/163390656-591fcc5b-a774-449f-8fb1-b27d4001a473.jpg)

Das *Enabled-Häkchen* (5) beim [ADVANCED VIEW](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/#advanced-view) zeigt Ihnen, ob das Set aktiv ist bzw. nicht. Per Mausklick auf "Remove" (6a) löschen Sie ein Set genauso einfach, wie Sie ein neues per Klick auf "Add destination/time sets" (6b) wieder hinzufügen können. Mit dem Button "Simple View" (7) gelangen Sie zurück zur "einfachen" Ansicht. Vergessen Sie nicht die Änderungen mit SAVE (8) zu speichern.
