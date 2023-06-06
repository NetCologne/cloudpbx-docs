---
title: "Gruppen"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 203
toc: true
---

Sollen bei Anwahl mehrere Nebenstellen gleichzeitig oder nacheinander angesprochen werden, ist die Erstellung einer Gruppe erforderlich:

![cloudpbx gruppe2](https://user-images.githubusercontent.com/98753538/158327798-b27cc189-38a7-4fd3-95ad-5640c7ac5355.jpg)

klicken Sie bitte im Punkt “PBX-Konfiguration” auf

* Gruppen (1) und fügen <br>
* Gruppenname (2, nur Kleinbuchstaben, keine Leer- oder Sonderzeichen) und die <br>
* Durchwahl (3) hinzu. <br>
* Ist der Kunde Eigentümer einer weitereren Nummer und hat er diese bei Auftragserteilung der NetCologne mitgeteilt, kann diese unter “Alias-Nummer” (4) ausgewählt und zugewiesen werden. Die Gruppe ist dann ebenfalls unter der Alias-Nummer erreichbar. <br>
* Unter Seats (5) werden die in der Gruppe teilnehmenden Nebenstellen hinzugefügt. <br>
* Die Hunting-Regel (6) bestimmt das Verfahren, mit dem die beteiligten Nebenstellen angewählt werden. <br>

![cloudpbx gruppe hunting](https://user-images.githubusercontent.com/98753538/158193548-c0180461-ea76-41f4-9fbb-f5f091ef7c68.jpg)

* Serielles Klingeln - Bei jedem eingehenden Anruf versucht das System stets, den Anrufer an die erste Nebenstelle in der Liste zu vermitteln. Wenn diese innerhalb der *Klingeldauer, z.B. 10 Sekunden* nicht antwortet, arbeitet sich das System sequentiell durch die Liste, um eine Nebenstelle zu suchen, die den Anruf entgegen nimmt. <br>
* Zufälliges Klingeln - Das System verteilt die Anrufe an die Nebenstellen zufällig.
* Zirkuläres Klingeln - Die Nebenstellen werden zyklisch in der festegelegten Reihenfolge ausgewählt. Das System versucht einen eingehenden Anruf an die Nebenstelle zu leiten, die nach der Nebenstelle aufgeführt ist, die zuletzt einen Anruf angenommen hat. Schlägt der erste Übertragungsversuch fehl, arbeitet das System die Liste zyklisch ab. Auch hier gibt die *Klingeldauer* an, wielange die jeweilige Nebenstelle angewählt wird. <br> **Info/Tipp für die drei vorstehenden Modi:** Wenn bei der letzten Nebenstelle der Gruppe die Klingeldauer überschritten wird, wird standardmäßig ausgelöst. Bei Bedarf kann die Anrufweiterleitung *Call Forward Unavailable* zu einem beliebigen Ziel (Voicemail, benutzerdefinierte Ansage, andere Nebenstelle, Handy, ...) eingerichtet werden. <br>
Siehe hierzu [Anrufweiterleitung Gruppe](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/#b-anrufweiterleitung-gruppe) und [Besonderheit beim Call Forward in der Gruppe](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/#4-besonderheit-call-forward-in-der-pbx-gruppe)

* Paralleles Klingeln - Wenn ein Anruf eingeht, klingelt es bei allen nicht belegten Nebenstellen in der Gruppe gleichzeitig. Der Anruf wird mit dem zuerst entgegengenommenen Telefon verbunden. Der Parameter "Klingeldauer" hat in diesem Fall keine Bedeutung <br>
* Auch hier ist eine Anrufweiterleitung möglich. Dafür ist der Typ *Call Forward Timeout* auszuwählen. Der Timeout, also nach welcher Zeit die Weiterschaltung erfolgt, wird bei Konfiguration der Weiterleitung festgelegt. 
