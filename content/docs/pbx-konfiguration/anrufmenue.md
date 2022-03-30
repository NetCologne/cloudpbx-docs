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

Zuerst klicken Sie im Menue *PBX-Konfiguration* auf den Unterpunkt **Anrufmenue [1]** . Dann wählen die Nebenstelle aus, für die Sie ein Anrufmenue zur Verfügung stellen möchten. Hier ist das *Zollstock*: 

![Anrufmenue1](https://user-images.githubusercontent.com/98753538/160846360-54337494-1f96-4b50-80b8-d2e97e1faf83.jpg)

Wenn Sie auf "+ EINTRAG HINZUFÜGEN" [2] klicken, können Sie die Ziffer (0 bis 9) auswählen, die dem Anrufer angeboten werden soll. Unter *Ziel* tragen Sie die  gewünschte Nebenstelle [3] ein und bestätigen mit "SPEICHERN" [4]. Damit ist Nebenstelle zugeordnet. Im Beispiel erreichen Sie also durch Wahl der Ziffer "1" die Nebenstelle "bruehl" und mit der "2" die Nebenstelle "chorweiler". "Kalk" erreicht man durch Wählen der "3":

![Anrufmenue2](https://user-images.githubusercontent.com/98753538/160850022-5ade644d-12c3-4450-856b-9f4c246edfa0.jpg)


### Aktivierung des Anrufmenues

