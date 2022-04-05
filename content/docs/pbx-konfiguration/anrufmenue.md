---
title: "Anrufmenü"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 208
toc: true
---

Das Anrufmenü oder auch Interactive Voice Response (IVR) ist wie ein Wegweiser für Anrufer. Über eine Navigation verbinden sich die Anrufer eigenständig mit den zuständigen Abteilungen oder Mitarbeitern. Der Anrufer wählt dabei mit seinen Zifferntasten (DTMF) aus verschiedenen Auswahlmöglichkeiten und hört zum Beispiel "Wollen Sie einen Service-Mitarbeiter sprechen, wählen Sie bitte die 1. Möchten Sie mit der Buchhaltung verbunden werden, wählen Sie bitte die 2." Bis zu 10 Auswahlschritte können eingesetzt werden und mit Weiterleitungen belegt werden. Auch kann eine eigene Ansage im .wav- oder .ogg-Format gespielt werden.

Mit dem Cloud PBX Konto dürfen Sie so viele IVRs einrichten und zeitbasiert einsetzen, wie Sie möchten. Dann leiten unterschiedliche Sprachnachrichten zu unterschiedlichen Zeiten die Anrufer weiter, zum Beispiel zu Bürozeiten und außerhalb. Sie können an einzelne IP-Endgeräte oder an ganze Rufgruppen als Ziel verweisen oder auf Handys oder externe Nummern weiterleiten. Auch können Sie Mailboxen und Ansagen als Ziel verwenden, um so allgemeine Anfragen wie die nach den Öffnungszeiten automatisch zu beantworten. Dadurch kann sich der Anrufer eigenständig zu unterschiedlichen Themen informieren, ohne dass sich ein Mitarbeiter darum kümmern muss, auch außerhalb Ihrer Bürozeiten - ein Gewinn für Sie und Ihre Anrufer.

[Wie Sie eine IVR erstellen und einrichten, lesen Sie unter "IVR einrichten".]

Die Einrichtung eines Anrufmenues erfordert zum einen die Konfiguration der Auswahlmöglichkeiten, d.h. welche Nebenstellen werden unter welcher Auswahlziffer erreicht und zum anderen aus der Aktivierung über CallForward mit diversen Zusatz-Funktionen.

### Konfiguration der Auswahlmöglichkeiten

Zuerst klicken Sie im Menue *PBX-Konfiguration* auf den Unterpunkt *Anrufmenue [1]* . Dann wählen die Nebenstelle aus, für die Sie ein Anrufmenue zur Verfügung stellen möchten. Hier ist das *zollstock*: 

![Anrufmenue1](https://user-images.githubusercontent.com/98753538/160846360-54337494-1f96-4b50-80b8-d2e97e1faf83.jpg)

Wenn Sie auf "+ EINTRAG HINZUFÜGEN" [2] klicken, können Sie die Ziffer (0 bis 9) auswählen, die dem Anrufer angeboten werden soll. Unter *Ziel* tragen Sie die  gewünschte Nebenstelle [3] ein und bestätigen mit "SPEICHERN" [4]. Damit ist Nebenstelle zugeordnet. Im Beispiel erreichen Sie also durch Wahl der Ziffer "1" die Nebenstelle "bruehl" und mit der "2" die Nebenstelle "chorweiler". "kalk" erreicht man durch Wählen der "3":

![Anrufmenue2](https://user-images.githubusercontent.com/98753538/160850022-5ade644d-12c3-4450-856b-9f4c246edfa0.jpg)


### Aktivierung des Anrufmenues

Das Anrufmenue wird mittels *Call-Forward-Funktion* aktiviert. Klicken Sie dafür auf den Menuepunkt *Kunden-Details [1]*, dann auf *Subscriber [2]* und bei der betreffenden Nebenstelle auf *Einstellungen [3]*. Hier ist das erneut *zollstock*:

![Anrufmenue_Aktivierung1](https://user-images.githubusercontent.com/98753538/161692092-8885b079-3d9e-4b35-be48-31ad5b803f99.jpg)

Öffenen Sie nun das Menue *Call-Forwards* und entscheiden, unter welchen Bedingungen das Anrufmenue erreicht werden soll. Bei registrierter Nebenstelle sind dabei drei Fälle üblich (grün):

 * *Call Forward Unconditional* - generelle Anrufweiterleitung
 * *Call Forward Busy* - Anrufweiterleitung, wenn besetzt
 * *Call Forward Timeout* - Anrufweiterleitung nach eine bestimmten Zeitspanne
  
 ![Anrufmenue_Auswahl Call Fowards2](https://user-images.githubusercontent.com/98753538/161062432-8a60e0e0-83ac-46ff-876a-e1bb67cc1e24.jpg)

Der Sonderfall *Call Forward Unavailable* (gelb) kommt zum Tragen, falls die Nebenstelle nicht registriert und damit nicht erreichbar ist. <br>
<br>
Im Beispiel wurde *Call Forward Unconditional* also die generelle Anrufweiterleitung angeklickt. Anschließend wählen Sie unter den Destinationen den Punkt *Auto Attendant* [1] und schauen, ob das Aktivierungshäkchen bei *Enabled* [2] gesetzt ist. 

![Anrufmenue_Auswahl Call Fowards Destin2](https://user-images.githubusercontent.com/98753538/161059358-8b507405-d193-409e-8dc7-7fb08781c4b5.jpg)

Bevor Sie mit *Save* [4] speichern, können Sie mit dem Button *Advanced View* [3] weitere Funktionen/Bedingungen auswählen:

![Anrufmenue_Auswahl Call Fowards Advaced1](https://user-images.githubusercontent.com/98753538/161068276-a0d06f14-d03e-4071-bc35-bc381239c6a8.jpg)

1. during Time Set - Zeiträume, in denen das Anrufmenue aktiviert ist.
2. from Source Set - Zulässige oder verbotene A-Rufnummernbereiche.
3. to B-Number Set - Zulässige oder verbotene B-Rufnummernbereiche.
4. Destination Set - Übersicht der unterschiedlichen Call Forwards (s.o.), für die *Anrufmenues* oder *Office Hours Announcements* aktiviert sind.

Wie Sie ein solches *destination/time set* konfigurieren und das davon mehrere möglich sind, erfahren Sie unter der Funktion [Anrufweiterleitung](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/).
