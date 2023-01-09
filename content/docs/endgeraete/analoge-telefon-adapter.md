---
title: "Analoge Telefon Adapter"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 504
toc: true
---

## Grandstream HT-814

Schließen Sie zuallererst Ihren Grandstream am Stromnetz und an Ihr Netzwerk an. Verbinden Sie dann das Gerät mit einem analogen Telefon via der Phone-Buchse.

<img src="/images/ht814.jpg" alt="HT-814"/>

#### Anschlüsse

![ATA Anschlüsse](https://user-images.githubusercontent.com/98753538/154268048-2ea154a9-ae3e-4934-960a-fa563b7d6f05.jpg)


#### Zugangsdaten und Firmeware

Das Grandstream HT-814 wird nicht automatisch provisioniert. Die Konfiguration ist daher selbst vorzunehmen.
Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse im lokalen Router ausgelesen werden kann:

![ATA_Login](https://user-images.githubusercontent.com/98472426/153013541-d360ff56-54ea-46d5-a651-2adefb915fc2.jpg)

Username und Password lauten beide "admin".

Im Menue "Grandsteam Device Configuration" überprüfen Sie bitte im Tab "Status", ob die aktuelle Firmware installiert ist.

![ATA Firmware](https://user-images.githubusercontent.com/98753538/152983105-1f5072ca-d8e5-4329-beb8-d8fb86408a5b.jpg)

https://firmware.grandstream.com/Release_Note_HT812_HT814_1.0.33.4.pdf

Weitere Informationen zum Firmwareupdate und die entsprechenden Downloads finden sich auf der Grandstream Seite: http://www.grandstream.com/support/firmware

Wechseln Sie in der Navigationsleiste auf den Reiter „Advanced Settings“ und scrollen bis zum Ende der Seite. Unter dem Punkt „Upload Firmeware“ können Sie die zuvor abgelegte Firmware auswählen und hochladen.
Mit "Export Backup Configuration" können Sie ein Backup Ihrer aktuellen Konfiguration erstellen (entfällt bei neu zu installierenden Geräten). Unter dem Punkt „Upload Configuration“ können Sie eine neue Konfiguration hochladen: Sie wählen den lokalen Pfad zu der gewünschten Konfigurations-Datei aus und klicken auf „Upload Configuration“.

#### Basic Settings

Beachten Sie die Voreinstellung von 10 Minuten beim Session Timeout.

![ATA Basic Setting](https://user-images.githubusercontent.com/98753538/152987589-de064f81-9a80-4af9-855b-2c678c5df960.jpg)

Wählen Sie die entsprechende Zeitzone und bestätigen am unteren Menueende mit "Apply". 

#### Advanced Settings

![ATA Advanced Setting 1](https://user-images.githubusercontent.com/98753538/152993085-9e822078-d8b2-4fb8-927c-45a2c5a59ae2.jpg)

![ATA Advanced Setting 2](https://user-images.githubusercontent.com/98753538/152993341-9497468f-470e-4dba-b2d0-48700a6d5cc1.jpg)

![ATA Advanced Setting 3](https://user-images.githubusercontent.com/98753538/152994356-9c31fc26-4820-4302-8472-e4911f4105d4.jpg)

###### Call Progress Tones


<table>
  <tbody>
    <tr>
      <td>Dial Tone</td>
      <td>f1=425@-10,c=0/0;</td>
    </tr>
    <tr>
      <td>Ringback Tone</td>
      <td>f1=425@-12,c=1000/4000;</td>
    </tr>
    <tr>
      <td>Busy Tone</td>
      <td>f1=425@-12,c=500/500;</td>
    </tr>
    <tr>
      <td>Reorder Tone</td>
      <td>f1=425@-12,c=220/220;</td>
    </tr>
    <tr>
      <td>Confirmation Tone</td>
      <td>f1=425@-11,f2=440@-11,c=100/100-100/100-100/100;</td>
    </tr>
    <tr>
      <td>Call Waiting Tone</td>
      <td>f1=425@-10,c=220/220-220/220-0/0;</td>
    </tr>
    <tr>
      <td>Prompt Tone</td>
      <td>f1=425@-17,f2=440@-17, c=0/0;</td>
    </tr>
    <tr>
      <td>Conference Party Hangup Tone</td>
      <td>f1=425@-15,c=600/600;</td>
    </tr>
  </tbody>
</table>

Übernehmen Sie die entsprechenden Einstellungen und bestätigen am unteren Menueende mit "Apply". 

#### Profile 1

![ATA Profile 1a](https://user-images.githubusercontent.com/98753538/152995771-2222ab95-cb9d-4a48-b043-6972b732f5a3.jpg)

![ATA Profile 1b](https://user-images.githubusercontent.com/98753538/152997833-82a5f4b8-bb80-404a-98b7-8c020d76ea02.jpg)

Bitte beachten Sie die Unterschiede bei der Einrichtung von Telefon und Faxgerät:

![ATA Profile 2a](https://user-images.githubusercontent.com/98753538/160421318-7cba8881-c80d-42d7-8da4-5686cbe3d684.jpg)

![ATA Profile 2b](https://user-images.githubusercontent.com/98753538/160421341-1a06c706-ea5f-4174-b8b7-4d3a6ce009a8.jpg)

![ATA Profile 1d](https://user-images.githubusercontent.com/98753538/152998051-436127e7-19e8-4b02-989f-059c88f43d0b.jpg)

![ATA Profile 1g](https://user-images.githubusercontent.com/98753538/211316828-46e3cd03-3dd1-450d-83f8-09a9ae8992ea.jpg)


Bitte beachten Sie die Unterschiede bei der Einrichtung von Telefon und Faxgerät:

![ATA Profile 3a](https://user-images.githubusercontent.com/98753538/160421380-55670a4f-b0df-4ebf-ad68-5dad975174ae.jpg)

![ATA Profile 3b](https://user-images.githubusercontent.com/98753538/160421400-aed4a6ec-42aa-47d6-9ac6-e8578d794c66.jpg)

Übernehmen Sie die entsprechenden Einstellungen und bestätigen am unteren Menueende mit "Apply". 

#### FXS Ports

Bei den **User Settings** achten Sie bitte darauf, ob und welche Vervollständgungegn durch Ihren Browser gemacht werden. Der Einsatz von *Google Chrome* wird empfohlen. 

![ATA FXS Ports](https://user-images.githubusercontent.com/98753538/153131122-84c31339-ff01-4c23-97e7-615006551e4b.jpg)

Ein SIP Account besteht aus einem *Benutzernamen/SIP User ID* sowie einem *SIP Passwort* und wird dazu benötigt, um sich beim SIP Anbieter anzumelden. Der Login erfolgt auf dem SIP-Server oder SIP-Proxy des Providers. Bei der Registrierung wird auch die *Authenticate ID* verlangt. Weiterhin wird unter *Name* der SIP-Display-Name eingegeben. Aus Gründen der Übersichtichkeit wird empfohlen: 

Unter *SIP User ID*, *Authenticate ID*, *Name* und *Request URI Routing ID* tragen Sie den **Sip Usernamen** der in der Cloud PBX eingerichteten Nebenstelle ein.

Das einzutragende *Passwort* ist das zugehörige **SIP Password** der Nebenstelle aus der Cloud-PBX.

Mit der *Profile ID* wählen Sie das entsprechende Profil aus. *Profile 1* könnte ein Profil für ein **analoges Telefon** sein, während *Profile 2* die Einstellungen für ein **Fax** beinhaltet. 

Zu den Unterschieden in den Profilen bzgl. Fax und analogem Telefon, beachten Sie bitte die Anmerkungen in den Abbildungen unter **Profile 1**.

Übernehmen Sie die entsprechenden Einstellungen und bestätigen am unteren Menueende mit "Apply". 

#### Besonderheit bei CLIR per Call

Auch im Bereich der IP-Telefonie sind die Funktionen "CLIP" und "CLIR" von Bedeutung. Mit Ihnen entscheiden Sie darüber, ob der angerufene Kunde die Rufnummer Ihres Unternehmens korrekt angezeigt bekommt und Sie die Rufnummer des Kunden bei einem eingehenden Anruf korrekt angezeigt bekommen.<br>
*CLIP* steht dabei für "Calling Line Identification Presentation". Das bedeutet einfach gesagt, dass die Rufnummer des anrufenden Teilnehmers zum annehmenden Teilnehmer übermittelt wird. <br>
*CLIR* stellt das Gegenteil dar "Calling Line Identification Restriction" und steht daher für Rufnummernunterdrückung. Möchte man diese **beim nächsten Anruf (CLIR per Call)** nicht anzeigen, muss bei  der Grandstream HT-814 bzw. am analogen DECT-/Telefon **\*67** vor die zu wählende Nummer gesetzt werden (abweichend vom deutschen Standard \*31).

## Grandstream HT-802

Bei diesem Analog Telefon Adapter handelt es sich um die kleinere Version des HT-814. Es besitzt im Unterschied zu diesem nur 2 analoge Phone-Buchsen.
![HT802](https://user-images.githubusercontent.com/98472426/165046529-54dd3e67-abaf-44d8-a5a9-036488a316d0.png)

Die Konfiguration des HT-802 erfolgt analog zum HT-814.
Hinweis: Die Profil-Daten der Ports werden hier direkt unter den Tab's FXS Ports konfiguriert.
