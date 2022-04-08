---
title: "Fax"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "funktionen"
weight: 407
toc: true
---

Mit der Faxfunktion können Sie sich das klassische Faxgerät sparen, denn hiermit empfangen und versenden Sie digitale Faxe direkt über das Konto Ihrer Cloud PBX. Sie brauchen lediglich eine Nebenstelle/Seat (1) mit der entsprechenden Faxnummer. In unserem Beispiel ist dies die Durchwahl 22 bei der Nebenstelle Flittard (2):

![Fax Seat Flittard1](https://user-images.githubusercontent.com/98753538/162135771-5b0c0c96-13a0-4096-a0f4-2e0c1e17434c.jpg)

### Faxservice einrichten

Um Faxe empfangen und als E-Mail weitergeleitet zu bekommen, klicken Sie im Menüpunkt *Faxeinstellungen* auf +ZIELRUFNUMMER HINZUFÜGEN (1) und geben die Ziel-E-Mail-Adresse (2), den gewünschten Dateityp (3), in dem das Fax als E-Mail gesendet werden soll und aktivieren die Zustellung bzw. den Sendebericht (4). Abschließend bestätigen Sie mit ✓ ZIEL ERSTELLEN (5) und wichtig: aktiveren die Faxfunktion (6) und beachten den Punkt [Faxempfang durch Rufumleitung](https://cloudpbx-doku.netcologne.de/docs/funktionen/fax/#faxempfang-durch-rufumleitung).

![Fax Einstellungen1](https://user-images.githubusercontent.com/98753538/162148734-0797682a-2dcd-47d3-8f7d-92c813024b72.jpg)

### Faxempfang durch Rufumleitung

![Fax Rufumleitung1](https://user-images.githubusercontent.com/98753538/162376426-7f10996a-43cc-44aa-a926-91445e5db525.jpg)

![Fax Rufumleitung2](https://user-images.githubusercontent.com/98753538/162376441-df0a41c0-3568-47bb-8593-de60fff8b519.jpg)



### Faxe versenden

Auch für den Versand von Faxen ist es erforderlich im Menüpunkt *Faxeinstellungen* die Funktion zu aktivieren (1). Klicken Sie anschließend auf das Tastatursymbol (2) und den dann erscheinenden *Sende-Fax-Button*. Im neuen Menü "Sende Fax" tragen Sie bitte die Faxnummer (3) ein und wählen für die zu übertragenden Informationen die Qualität aus (4). Wichtig ist im Feld "Seitenkopf" die Eingabe der Fax- oder Absenderkennung (5). Viele Fax-Empfänger blockieren Faxe, die überhaupt keine Absender-Kennung besitzen aus Angst vor unerwünschter Fax-Werbung.

![Fax Einstellungen3](https://user-images.githubusercontent.com/98753538/162151663-768a49d4-7c83-45a3-bb03-ac65eb3ea244.jpg)

Bei "Inhalt" (6) können Sie Ihre Nachricht in Textform eingeben. Darunter besteht die Möglichkeit eine Datei auszuwählen, die dann als Fax übertragen wird. Sind alle Angaben gemacht, klicken Sie abschließend auf SENDEN (8).

### Konversationen

![Fax Konversationen](https://user-images.githubusercontent.com/98753538/162376562-8a9de5c1-bcb7-4dab-853a-dca5c1bfff9e.jpg)

Hier sehen Sie alle eingehenden und ausgehenden Faxe mit Sendeberichten. Sie können auf deren Inhalt zugreifen und sie direkt herunterladen. Ist die Funktion der E-Mail-Benachrichtigung zuvor aktiv gelassen worden, bekommen Sie zudem über jedes Fax eine Nachricht mit dem Fax-Inhalt als PDF-Dokument
Das gefaxte Dokument und den Sendebericht finden Sie nun im Fax-Journal wieder.

### Fax-Konfiguration als Administrator

![Fax Admin Kundendetails](https://user-images.githubusercontent.com/98753538/162376660-3e9aae1d-a9eb-4123-87a6-5e6725724e80.jpg)

![Fax Admin Kundendetails2](https://user-images.githubusercontent.com/98753538/162376672-7ae4aad6-9475-49c8-9f6c-164488e67070.jpg)

![Fax Admin Kundendetails3](https://user-images.githubusercontent.com/98753538/162376679-b5146278-36fb-496b-b624-8fd720e549ad.jpg)



*Der untere Teil kann nun weg, oder?

![grafik](https://user-images.githubusercontent.com/20154956/151542716-bd20b68d-2beb-4bfd-943f-4dd1c1f57e2d.png)

*Um die gewünschte Nummer als Faxnummer zu konfigurieren gehen Sie bitte unter Faxeinstellungen wie folgt vor:

*1. Aktivieren Sie die Faxfunktion
*2. Hinterlegen Sie eine E-Mail Adresse
*3. Nutzen Sie das Faxfeld um Faxe zu versenden
