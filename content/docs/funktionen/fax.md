---
title: "Fax"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "funktionen"
weight: 432
toc: true
---

Mit Ihrer Cloud PBX können Sie sich das klassische Faxgerät sparen. Die Faxfunktion ermöglicht den Versand von digitalen Faxen gleichermaßen wie deren Empfang. Neben einer E-Mail-Adresse brauchen Sie lediglich eine *Nebenstelle (1)* mit Faxnummer. In unserem Beispiel ist dies die Durchwahl 27 bei der Nebenstelle *fax (2)*:

![Fax NSt auswählen](https://github.com/user-attachments/assets/dfbd912c-eb21-451f-84a2-c56d76d57eb3)

### Faxservice einrichten

Haben Sie die Nebenstelle ausgewählt, klicken Sie auf +ZIELRUFNUMMER HINZUFÜGEN (1), geben die Ziel-E-Mail-Adresse (2) und den gewünschten Dateityp (3) an (hier: pdf), in dem das Fax als E-Mail gesendet werden soll. Unter Punkt (4) aktivieren Sie die E-Mail-Zustellung für ein- und ausgehende Faxe sowie für den Sendebericht. Danach bestätigen Sie mit ✓ ZIEL ERSTELLEN (5). <br>

![Faxservice einrichten](https://github.com/user-attachments/assets/3f78903e-d760-434a-9796-797ad910d6e5)

Wichtig: Aktiveren Sie die Faxfunktion (6) und beachten den nächsten Punkt [Faxempfang durch Rufumleitung](https://cloudpbx-doku.netcologne.de/docs/funktionen/fax/#faxempfang-durch-rufumleitung).

Klicken Sie zunächst im Menüpunkt *Faxeinstellungen*

![Fax Einstellungen1](https://user-images.githubusercontent.com/98753538/162148734-0797682a-2dcd-47d3-8f7d-92c813024b72.jpg)

### Faxempfang durch Rufumleitung

Damit die Nebenstelle nun Faxe empfangen und als E-Mail weiterleiten kann, klicken Sie bitte bei *Anrufeinstellungen* auf Rufumleitung (1) und dort auf + RUFUMLEITUNG HINZUFÜGEN (2). Danach legen Sie Bedingungen fest, wann die Weiterleitung erfolgen soll. Falls dies *IMMER* der Fall sein soll, wählen Sie "Wenn verfügbar" (3a) und "Wenn nicht verfügbar" (3b). Letzte Bedingung greift, falls die Nebenstelle nicht registriert ist. Anschließend klicken Sie rechst auf die drei kleinen Punkte (4a bzw. 4b) und wählen im sich öffnenden Menü den Punkt "Zu Fax2Mail weiterleiten" (5). 

![Fax Rufumleitung1](https://user-images.githubusercontent.com/98753538/162376426-7f10996a-43cc-44aa-a926-91445e5db525.jpg)

Die überflüssige Zeile "Weitergeleitet zu  Nummer" können Sie einfach entfernen.

![Fax Rufumleitung2a](https://user-images.githubusercontent.com/98753538/162387302-2a4b9111-e6cf-4928-b42e-85dfdc080d65.jpg)

Aufgrund eines Fehler in der Anzeige mit der *blinkenden Punkten* in der Zeilenmitte, ist es notwendig, dass Sie die **Browseransicht aktualisieren**. Danach sollte die "Fax2Mail-Rufumleitung" so aussehen:

![Fax Rufumleitung2](https://user-images.githubusercontent.com/98753538/162376441-df0a41c0-3568-47bb-8593-de60fff8b519.jpg)

### Faxe versenden

Auch für den Versand von Faxen ist es erforderlich, im Menüpunkt *Faxeinstellungen* die Funktion zu aktivieren (1). Klicken Sie anschließend auf das Tastatursymbol (2) und den dann erscheinenden *Sende-Fax-Button*. Im neuen Menü "Sende Fax" tragen Sie bitte die Faxnummer (3) ein und wählen für die zu übertragenden Informationen die Qualität aus (4). Wichtig ist im Feld "Seitenkopf" die Eingabe der Fax- oder Absenderkennung (5). Viele Fax-Empfänger blockieren Faxe, die überhaupt keine Absender-Kennung besitzen aus Angst vor unerwünschter Fax-Werbung.

![Fax Einstellungen3](https://user-images.githubusercontent.com/98753538/162151663-768a49d4-7c83-45a3-bb03-ac65eb3ea244.jpg)

Bei "Inhalt" (6) können Sie Ihre Nachricht in Textform eingeben. Darunter besteht die Möglichkeit eine Datei auszuwählen, die dann als Fax übertragen wird. Sind alle Angaben gemacht, klicken Sie abschließend auf SENDEN (8).

### Konversationen

![Fax Konversationen](https://user-images.githubusercontent.com/98753538/162376562-8a9de5c1-bcb7-4dab-853a-dca5c1bfff9e.jpg)

Im Menuüpunkt Konversationen können Sie sehen, welche Faxe Sie versendet bzw. erhalten haben. Mit Filtern können Sie den Zeitraum eingrenzen. Außerdem besteht hier die Möglichkeit, die Faxe herunterladen. 


### Fax-Konfiguration als Administrator

Wenn Sie als Administrator eingeloggt sind, können Sie jede Ihrer Nebenstellen individuell konfigurieren (ohne sich als diese anzumelden). Zu diesen Einstellungen gelangen Sie mit dem untersten Menüpunkt *Kundendetails* (1). Hier können Sie nun die Nebenstelle konfigurieren, die als Faxgeräte betrieben werden soll. Klicken Sie dafür auf *Subscriber* (2) und dann bei der "Fax-Nebenstelle" rechts auf Einstellungen (3).

![Fax Admin Kundendetails](https://user-images.githubusercontent.com/98753538/162376660-3e9aae1d-a9eb-4123-87a6-5e6725724e80.jpg)

Unter dem Punkt "Call Forwards" können Sie bestehenden Fax2Mail-Rufumleitungen einsehen und editieren:

![Fax Admin Kundendetails2](https://user-images.githubusercontent.com/98753538/162376672-7ae4aad6-9475-49c8-9f6c-164488e67070.jpg)

Gleiches gilt für die Konfiguration der Faxeinstellungen, die Sie unter "Fax Features" finden.

![Fax Admin Kundendetails3](https://user-images.githubusercontent.com/98753538/162376679-b5146278-36fb-496b-b624-8fd720e549ad.jpg)

Auch hier können Sie die "Fax2Mail and Sendfax-Funktionen" an- und ausschalten, indem bei *Active* ein Häkchen gesetzt wird (yes) oder eben nicht (no).


### Mail2Fax

Mit dieser Funktion können E-Mails als Fax versendet werden. Zuvor muss der Administrator unter *Kundendetails* für die entsprechende Nebenstelle das Feature aktivieren und einige Einstellungen vornehmen:

![mail2fax_details2](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/e5aa3353-9e4e-4aa1-a33b-3b8f63b51104)

Die Fax2Mail- und die Mail2Fax-Funktion müssen aktiviert werden. => Setzen Sie in beiden Feldern "Active" den Wert "yes" [1]

Aktivieren Sie einen Secret Key (aktuell ist dieser mandatory!), hier "1_2_3_4_5_6" [2]

Falls Sie diesen zeitweilig erneuern möchten, tragen Sie die Zeitspanne ein und die Mailadresse, die dazu informiert werden soll [3].

Unabhängig davon muss Punkt [4], die ACL (Access Control List), definiert werden:

![edit acl](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/a84317be-6584-4bf3-98a0-d1c0e1cf4923)

Hier tragen Sie Berechtigungen zum Faxversandt ein. Neben einer oder mehreren E-Mailadressen, können die IP-Adresse (oder Bereich) des Absenders sowie zulässige Zielrufnummern eingetragen werden. Mit der Zeichenkombination ".*" sind beliebige Nummern möglich. Bitte beachten Sie das Häkchen bei "Use Regex".

Mit diesen Einstellungen kann man nun E-Mails an den Faxserver senden, der diese dann als Fax verschickt.

Mit den o. a. Einstellungen sähe dann eine E-Mail, die ein PDF Dokument über die *faxnebenstelle* an eine Zielrufnummer faxt, so aus:

![mail2fax_email3](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/cb886fcf-4b53-4061-a2b8-e8fedfb9dac2)

Vor dem Secret Key müssen Sie eine **Leerzeile** eingeben. Eine einfache Nachricht senden Sie bitte im **"Nur Text"-Format**, da **html nicht akzeptiert** wird. Sie können auch ein vorhandenes Text-Dokument faxen, wenn es im **.pdf-Format** gespeichert wurde.









