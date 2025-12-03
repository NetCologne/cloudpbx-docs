---
title: "Fax"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "funktionen"
weight: 432
toc: true
---

Mit Ihrer Cloud PBX können Sie sich das klassische Faxgerät sparen. Die Faxfunktion ermöglicht den Versand von digitalen Faxen gleichermaßen wie deren Empfang. Neben einer E-Mail-Adresse brauchen Sie lediglich eine *Nebenstelle* mit Faxnummer. In unserem Beispiel lautet sie TESTNUMMER. 

![Faxeinstellungen1](https://github.com/user-attachments/assets/2e497804-d787-4b2e-8567-05c162098c09)

## 1. FAX TO MAIL UND SENDFAX

### 1.1 Faxservice einrichten

Haben Sie die *Faxeinstellungen* gewählt, klicken Sie auf +ZIELRUFNUMMER HINZUFÜGEN (1), geben die Ziel-E-Mail-Adresse (2) und den gewünschten Dateityp (3) an (hier: pdf), in dem das Fax als E-Mail gesendet werden soll. Unter Punkt (4) aktivieren Sie die E-Mail-Zustellung für ein- und ausgehende Faxe sowie für den Sendebericht. Danach bestätigen Sie mit ✓ ZIEL ERSTELLEN (5). <br>


![Faxservice einrichten2](https://github.com/user-attachments/assets/c05392ce-0e82-4c90-9b69-ce0d1a71c30a)

💡 **Wichtig:** Aktiveren Sie die Faxfunktion (rot umrandet) und beachten den nächsten Punkt [Faxempfang durch Rufumleitung](https://cloudpbx-doku.netcologne.de/docs/funktionen/fax/#faxempfang-durch-rufumleitung). <br>
<br>
 
### 1.2 Faxempfang durch Rufumleitung

Damit die Nebenstelle nun Faxe empfangen und als E-Mail weiterleiten kann, klicken Sie bitte bei *Anrufeinstellungen* auf Rufumleitung (1) und dort auf + RUFUMLEITUNG HINZUFÜGEN (2). Danach legen Sie Bedingungen fest, wann die Weiterleitung erfolgen soll. Falls dies *IMMER* der Fall sein soll, wählen Sie "Ständig" (3a) und "Wenn nicht verfügbar" (3b). Letzte Bedingung greift, falls die Nebenstelle nicht registriert ist. Eine weitere Bedingung wäre *Wenn besetzt*. Anschließend klicken Sie rechst auf die drei kleinen Punkte (4a bzw. 4b) und wählen im sich öffnenden Menü den rotumrandeten Punkt "Zu Fax2Mail weiterleiten" (5). <br>

![Fax Rufumleitung1](https://github.com/user-attachments/assets/fcc0fee2-0013-48f3-97b3-523d9a3f82ad)

Die überflüssige Zeile "Weitergeleitet zu Nummer" können Sie einfach entfernen. <br>

![Fax Rufumleitung2a](https://github.com/user-attachments/assets/593fe939-733c-4a6d-a888-8ea8727a69bc)

Danach sollte die "Fax2Mail-Rufumleitung" so aussehen: <br>

![Fax Rufumleitung2](https://github.com/user-attachments/assets/1c6413b8-e05b-4a25-891b-f3216c87d88a)


### 1.3 Faxe versenden

Auch für den Versand von Faxen ist es erforderlich, im Menüpunkt *Faxeinstellungen* die Funktion zu aktivieren (1). Klicken Sie anschließend auf das Tastatursymbol (2) und den dann erscheinenden *Sende-Fax-Button*. Im neuen Menü **Sende Fax** tragen Sie bitte die Faxnummer (3) ein und wählen für die zu übertragenden Informationen die Qualität aus (4). Wichtig ist im Feld *Seitenkopf* die Eingabe der Fax- oder Absenderkennung (5). Viele Fax-Empfänger blockieren Faxe, die überhaupt keine Absender-Kennung besitzen aus Angst vor unerwünschter Fax-Werbung.

![Fax Einstellungen3a](https://github.com/user-attachments/assets/aae6fca2-3247-4844-b349-6a3f40a8afa4)

Bei Inhalt (6) können Sie Ihre Nachricht in Textform eingeben. Darunter besteht die Möglichkeit eine Datei auszuwählen (7), die dann als Fax übertragen wird. Sind alle Angaben gemacht, klicken Sie abschließend auf SENDEN (8).

### 1.4 Konversationen

![Fax Konversationen](https://user-images.githubusercontent.com/98753538/162376562-8a9de5c1-bcb7-4dab-853a-dca5c1bfff9e.jpg)

Im Menuüpunkt Konversationen können Sie sehen, welche Faxe Sie versendet bzw. erhalten haben. Mit Filtern können Sie den Zeitraum eingrenzen. Außerdem besteht hier die Möglichkeit, die Faxe herunterladen. 


### 1.5 Fax-Konfiguration als Administrator

Wenn Sie als Administrator eingeloggt sind, können Sie jede Ihrer Nebenstellen individuell konfigurieren (ohne sich als diese anzumelden). Klicken Sie dafür im Menü *PBX-Konfiguration* den Unterpunkt Nebenstellen (1) und wählen die entsprechende aus:

![Fax NSt auswählen](https://github.com/user-attachments/assets/dfbd912c-eb21-451f-84a2-c56d76d57eb3)

Im Reiter FAX TO MAIL UND SENDFAX können Sie die gleichen Punkte konfigurieren, wie unter den *Faxeinstellungen*: +ZIELRUFNUMMER HINZUFÜGEN (1), Ziel-E-Mail-Adresse (2) eingeben und den Dateityp (3), in dem das Fax als E-Mail gesendet werden soll, auswählen. Unter Punkt (4) aktivieren Sie die E-Mail-Zustellung für ein- und ausgehende Faxe sowie für den Sendebericht. Der Abschluss erfolgt mit ✓ ZIEL ERSTELLEN (5). <br>

![Faxservice einrichten](https://github.com/user-attachments/assets/6efc3069-0aa1-425d-b666-c8dfb5f79b7d)

💡 **Wichtig:** Aktiveren Sie auch hier die Faxfunktion (rot umrandet) und beachten den Punkt [Faxempfang durch Rufumleitung](https://cloudpbx-doku.netcologne.de/docs/funktionen/fax/#faxempfang-durch-rufumleitung). <br>
<br>


## 2. Mail To Fax

Mit dieser Funktion können E-Mails als Fax versendet werden. Wenn Sie diese Funktion nutzen möchten, setzen Sie sich bitte NetCologne in Verbindung. Die Kollegen übernehmen dann die Aktivierung.

### 2.1 Konfiguration unter Faxeinstellungen

Wurde die Funktion "MAIL TO FAX" aktiviert, sind die Konfugurationen unter *Faxeinstellungen* möglich.

![Mail2Fax Einstellungen](https://github.com/user-attachments/assets/2ed19120-8d67-4fcc-8493-dee0097a7152)

Kontrollieren Sie zuerst den Schalter "Aktiv" [1]. 

Darunter aktivieren Sie einen Geiheimschlüssel (aktuell ist dieser mandatory!), hier mit eingabe von "1_2_3_4_5_6" [2] 

Falls Sie diesen zeitweilig erneuern möchten, tragen Sie die Zeitspanne (3a) ein und die Mailadresse (3b), die dazu informiert werden soll.

Unabhängig davon muss Punkt [4], die Zugriffssteuerungsliste (ACL=Access Control List), definiert werden. Klicken Sie dafür auf *+ ACL HINZUFÜGEN* und tragen folgende Berechtigungen zum Faxversandt ein: 

![acl erstellen](https://github.com/user-attachments/assets/336a6443-5919-4d6a-acf9-ec708776a9f3)


**Absender-E-Mail-Adresse** Das sind die einer oder mehreren E-Mailadressen (ihrer Mitarbeiter), die dann Faxe versenden dürfen,
**Empfangen von IP** Das ist die IP-Adresse (oder der IP-Adress-Bereich) des oder der Absender.
**Ziel** Hier werden zulässige Zielrufnummern eingetragen.
Bei beiden können Regular Expressions verwendet werden. Mit der Zeichenkombination **".*" sind beliebige Nummern** möglich. Bitte beachten Sie das Häkchen bei "RegExp verwenden".

![acl erstellt](https://github.com/user-attachments/assets/3ef8bbc9-21d6-45ec-ab3a-387e4739a833)


### 2.2 Mail als Fax versenden

Mit diesen Einstellungen kann man nun E-Mails an den Faxserver senden, der diese dann als Fax verschickt.

Mit den o. a. Einstellungen sähe dann eine E-Mail, die ein PDF Dokument über die *faxnebenstelle* an eine Zielrufnummer faxt, so aus:

![mail2fax_email3](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/cb886fcf-4b53-4061-a2b8-e8fedfb9dac2)

Vor dem Secret Key müssen Sie eine **Leerzeile** eingeben. Eine einfache Nachricht senden Sie bitte im **"Nur Text"-Format**, da **html nicht akzeptiert** wird. Sie können auch ein vorhandenes Text-Dokument faxen, wenn es im **.pdf-Format** gespeichert wurde.
