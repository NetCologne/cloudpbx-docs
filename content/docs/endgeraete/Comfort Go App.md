---
title: "Comfort Go App"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 512
toc: true
---
Mit „Comfort Go“ wird Ihr Smartphone zum Festnetztelefon. Die App bietet Ihnen die Möglichkeit mit Ihrer Festnetznummer über das eigene Smartphone zu telefonieren, egal wo Sie sich gerade aufhalten. Mit „Comfort Go“ sind Sie im Büro, im Café oder auf Reisen über Ihre Festnetznummer erreichbar. Haben Sie doch mal einen Anruf verpasst, können Sie bequem von unterwegs Ihren NetCologne Anrufbeantworter abhören.

Ihre Vorteile im Überblick:

* nutzen Sie „Comfort Go“ um weltweit mit Ihrer Festnetznummer zu telefonieren 
* „Comfort Go“ kommuniziert verschlüsselt (TSIP / SRTP) mit unseren Servern 
* Informationen über Ihre Rufnummer sowie die Gespräche selber sind gegen Abhören geschützt 
* anwendungsgerechte Codecs wie Opus, G722, iLBC gewährleisten eine gute Sprachqualität 
* verwenden Sie die im Smartphone gespeicherten Kontakte und Favoriten direkt aus der App heraus 
* lassen Sie sich alle Anrufe im Verlauf anzeigen 
* verwenden Sie bis zu zehn Festnetznummern Ihres IP-basierten Comfort-Anschlusses 
* chatten Sie verschlüsselt mit Ihren Kontakten, die ebenfalls die „Comfort Go“ nutzen 
* hören Sie von unterwegs Ihren NetCologne Anrufbeantworter ab<br>
<br>

## Installation

### Comfort Go bei Google Play (Android)

Für Android (ab 4.2) können Sie die App unter [Google Play](https://play.google.com/store/apps/details?id=de.netcologne.hometogo&hl=de&gl=US) herunterladen und installieren.

![App Google Play](https://user-images.githubusercontent.com/98753538/169261390-61447d26-e5b7-4297-be0a-e64ecd3b4aa5.jpg)

Anschließend werden Sie aufgefordert, den QR-Code von der zugehörigen Nebenstelle zu scannen. Diesen finden Sie im Menue ihrer Cloud-PBX am oberen Rand (roter Pfeil).

![Cloud PBX_Uebersicht2](https://user-images.githubusercontent.com/98753538/169230239-f24efc0b-9633-4713-ae8d-0196c0a560ed.jpg)

Sobald Sie auf das Symbol geklickt haben, können Sie den QR-Code einscannen.

![Cloud PBX_QR_Code1](https://user-images.githubusercontent.com/98753538/169230789-4dac34ef-d995-45ee-a15a-be3a7f933591.jpg)

Anschließend werden Sie um die üblichen Zugriffsberechtigungen (Kontakte, Microfon und Hintergrunddaten) gebeten.

![Zugriff](https://user-images.githubusercontent.com/98753538/169234986-406640bf-5dec-46e2-ae07-ae9dc6057e7b.jpg)

Sobald Sie diese gewährt haben, können Sie die App nutzen und genau wie mit Ihrer Cloud-PBX telefonieren, d.h. für abgehende Telefonaten ist die Amtsholung "0" erforderlich. Wenn Sie Ihre Kontakte direkt anrufen möchten, müssen deren Nummern mit "+49" eingetragen sein. Falls Sie angerufen werden, ist mit der Taste "Transfer" die Weiterleitung zu anderen Nebenstellen möglich.

![Funktionen](https://user-images.githubusercontent.com/98753538/169236252-fdb10320-1c51-4f78-a547-f32a13f180c1.jpg)<br>
<br>

### Comfort Go im App Store (iOS)

Für iOS (ab 13.0) finden sie die App im [App Store](https://apps.apple.com/de/app/comfort-go-ihre-sip-festnetznummer-f%C3%BCr-unterwegs/id1047120037). Nach der Installation erlauben Sie den Kamerazugriff, um den QR-Code von der zugehörigen Nebenstelle scannen zu können.

![iOS Comfort Go App](https://user-images.githubusercontent.com/98753538/169789714-43ceb944-5991-430c-a7da-a28840f6484b.jpg)

Diesen finden Sie im Menue ihrer Cloud-PBX am oberen Rand (roter Pfeil).

![Cloud PBX_Uebersicht2](https://user-images.githubusercontent.com/98753538/169230239-f24efc0b-9633-4713-ae8d-0196c0a560ed.jpg)

Sobald Sie auf das Symbol geklickt haben, können Sie den QR-Code einscannen.

![Cloud PBX_QR_Code1](https://user-images.githubusercontent.com/98753538/169230789-4dac34ef-d995-45ee-a15a-be3a7f933591.jpg)

Anschließend werden Sie um die üblichen Zugriffsberechtigungen (Kontakte, Mikrofon und Push) gebeten.

![iOS Zugriff2](https://user-images.githubusercontent.com/98753538/174999578-9c2ec802-fc65-465d-90a3-8b4bd4734b46.jpg)

Sobald Sie diese gewährt haben, können Sie die App nutzen und genau wie mit Ihrer Cloud-PBX telefonieren, d.h. für abgehende Telefonaten ist die Amtsholung "0" erforderlich. Wenn Sie Ihre Kontakte direkt anrufen möchten, müssen deren Nummern mit "+49" eingetragen sein. Falls Sie angerufen werden, ist mit der Taste "Transfer" die Weiterleitung zu anderen Nebenstellen möglich.

![iOS Funktionen](https://user-images.githubusercontent.com/98753538/169789156-eb121fa9-3bf4-4411-84ea-06d9d9bda438.jpg)

## PBX-Funktionen

Mit der Comfort-Go-App können Sie nicht nur telefonieren, sondern verfügen über weitere Cloud-PBX-Funktionen - ähnlich wie bei einer kleinen TK-Anlage.

### Weiterleiten mit Rückfrage (Comfort Go aktiv) - für IOS

Ihre Comfort-Go-App ist aktiv und Sie (B) erhalten einen Anruf von A. Drücken Sie nun die Taste "Halten":

![Weiterleitung 1](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/97ef19f8-ac8c-4055-a32c-119066590580)

Anschließend klicken Sie auf den "+ Button" (Hinzufügen). Nun können Sie das Ziel C entweder aus den Kontakten auswählen oder rechts oben zur Tastatur wechseln und die Rufnummer wählen. Im Beispiel wird der Kontakt "kalk" ausgewählt. Die zugehörge Nummer ist anschließend per Fingerdruck zu bestätigen.

![Weiterleitung 2](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/baa1910d-c303-42b0-85e8-c13b102bb075)

Anschließend klingelt es beim Ziel "kalk". Sobald der Anruf entgegengenommen wurde, können der Anrufer A und das Ziel C durch Drücken des Buttons "Transferieren" verbunden werden. 

Alternativ kann mit "Zusammenführen" eine Konferenz (A+B+C) initiiert werden. Mit dem Button "kSwap" kann zwischen A und C hin und her geschaltet werden.

![Weiterleitung 3](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/624dc7fa-ddb8-45e9-9910-0a249995c91d)

Haben Sie den Call "transferiert", ist die Verbindung für Sie beendet. Im Display erscheint:

![Bild 7](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/cd34623a-fa69-4b82-869b-328f8905025e)

### Weiterleiten mit Rückfrage (Comfort Go inaktiv) für IOS

Die Comfort-Go-App ist nicht aktiviert und Ihr Smartphone im Stand-By-Modus. Wenn Sie (B) nun einen Anruf von A erhalten, können Sie diesen durch Wischen in Pfeilrichtung annehmen. Wünschen Sie weitere Funtktionen (Weiterleitung, 3er-Konferenz), ziehen Sie den Comfort-Go-Button nach unten und entsperren den Bildschirm per Code-Eingabe.

![Weiterleitung 4](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/467f8fdc-6bdd-4258-9739-445e6fb914bb)

Auf dem Display erscheint die Tastatur, Sie wählen die Nummer des Ziels C und nach Drücken des grünen Buttons erfolgt der Gesprächsaufbau (Verbinde ...).

![Weiterleitung 5](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/eadd5f3a-86f9-456f-a79f-eaa3c70a20a2)

Sobald das Ziel den Anruf entgegengenommen hat, erhalten Sie eine "On-Hold-Meldung" und können durch Drücken der Taste "Transferieren" den Anrufer A mit dem Ziel C verbinden. Damit endet für Sie der Anruf (Aufgelegt).

![Weiterleitung 6](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/593107f5-93d8-46be-9776-2562d5ae58ec)


### Weiterleiten mit Rückfrage (Comfort Go inaktiv) für Android

Diese Funktion steht ab Version 2.2.1 zur Verfügung.

Die Comfort-Go-App ist nicht aktiviert und Ihr Smartphone im Stand-By-Modus. Wenn Sie (B) nun einen Anruf von A erhalten, können Sie diesen durch Wischen in Pfeilrichtung annehmen. Um nun eine Rückfrage einzuleiten, drücken Sie auf "Hinzufügen". Es öffnet sich ein Fenster, in dem Sie entweder die gewünschte Rufnummer eintippen oder Sie wählen aus den darüber angezeigten Favoriten das Ziel aus.

![weiterleitung_a_01](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/ff52f59d-1dc6-4f79-bf25-0e5afc0f61a3)

In diesem Beispiel wird das Ziel "kalk" aus den Favoriten ausgewählt. Dazu tippen Sie auf das Hörersymbol neben den Eintrag "kalk".

Sobald der Teilnehmer "kalk" den Anruf entgegengenommen hat, können Sie mit ihm sprechen und z.B. die Übergabe des Anrufers (A) angkündigen. Durch Tippen auf "Transferieren" übergeben Sie das Gespräch an den Teilnehmer "kalk". Für Sie endet damit der Anruf.

![weiterleitung_a_02](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/cf6995a9-12d1-46bb-b1e6-898efc7e1def)

