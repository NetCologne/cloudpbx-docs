---
title: "Anrufmenü"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 208
toc: true
---

Mit dem **Anrufmenü** werden Anrufer mit unterschiedlichen Sprachnachrichten ggf. auch zeitabhängig zu unterschiedlichen Zielen weitergeleitet, zum Beispiel innerhalb der Bürozeiten zum Sekretariat und außerhalb zu einer Ansage. Als Ziel können Sie an einzelne IP-Endgeräte, ganze Rufgruppen oder auf Handys weiterleiten. Auch können Sie Mailboxen und Ansagen als Ziel verwenden, um so allgemeine Anfragen wie die nach den Öffnungszeiten automatisch zu beantworten. Dadurch kann sich der Anrufer eigenständig zu unterschiedlichen Themen informieren, ohne dass sich ein Mitarbeiter darum kümmern muss, auch außerhalb Ihrer Bürozeiten - ein Gewinn für Sie und Ihre Anrufer.

Das **Anrufmenü** ist wie ein Wegweiser für Anrufer. Über eine Navigation verbinden sich die Anrufer eigenständig mit den zuständigen Abteilungen oder Mitarbeitern. Der Anrufer wählt dabei mit seinen Zifferntasten (DTMF) aus verschiedenen Auswahlmöglichkeiten und hört zum Beispiel: <br>
"Wollen Sie einen Service-Mitarbeiter sprechen, wählen Sie bitte die 1." <br>
"Möchten Sie mit der Buchhaltung verbunden werden, wählen Sie bitte die 2." <br>

Bis zu 10 Auswahlschritte können eingesetzt werden und mit Weiterleitungen belegt werden. <br>
Für den Fall, dass der Anrufer keine Auswahl trifft, kann ein Standardziel eingerichtet werden. <br>
Als Ziel können sowohl interne Nebenstellen als auch eine oder mehrer Ansagen im .wav- oder .ogg-Format gespielt werden. <br>
Wie Sie diese einrichten, erfahren Sie unter [Soundset](https://cloudpbx-doku.netcologne.de/docs/pbx-konfiguration/sound-sets/).

Die Einrichtung eines Anrufmenüs erfordert zum einen die Konfiguration der Auswahlmöglichkeiten, d.h. welche Nebenstellen werden unter welcher Auswahlziffer erreicht und zum anderen aus der Aktivierung über CallForward mit diversen Zusatz-Funktionen.

### Konfiguration der Auswahlmöglichkeiten

Zuerst klicken Sie im Menü *PBX-Konfiguration* auf den Unterpunkt *Anrufmenü [1]* . Dann wählen Sie die Nebenstelle aus, für die Sie ein Anrufmenü zur Verfügung stellen möchten. Hier ist das *zollstock*: 

![Anrufmenue1](https://user-images.githubusercontent.com/98753538/160846360-54337494-1f96-4b50-80b8-d2e97e1faf83.jpg)

Wenn Sie auf **+ EINTRAG HINZUFÜGEN** [2] klicken, können Sie die Ziffer (0 bis 9 und default) auswählen, die dem Anrufer angeboten werden soll. <br>
Unter **Ziel** tragen Sie die gewünschte Nebenstelle [3] (und damit den entsprechenden sip_user) ein und bestätigen mit *SPEICHERN* [4]. <br>
Damit ist die Nebenstelle bzw. der sip_user zugeordnet. Im Beispiel erreichen Sie also durch Wahl <br>
der **Ziffer 1** die Nebenstelle *bruehl*, <br> 
mit **Ziffer 2** die Nebenstelle *chorweiler* und <br>
mit **Ziffer 3** die Nebenstelle *kalk*:

![Anrufmenue2](https://user-images.githubusercontent.com/98753538/160850022-5ade644d-12c3-4450-856b-9f4c246edfa0.jpg)

Mit dem Eintrag **default** legen Sie ein Standardziel fest. Dieses wird angesteuert, wenn der Anrufer nicht innerhalb von 5 Sekunden eine Auswahl trifft.

![image](https://user-images.githubusercontent.com/99875470/208917344-e72f0fd3-9000-4b12-92e8-6c1dd92e794c.png)

### Aktivierung des Anrufmenüs

Das Anrufmenü wird mittels **Rufumleitung** aktiviert. Wählen Sie zunächst über das Menü PBX-Konfiguration -> Nebenstellen die entsprechende Nebenstelle aus (hier: Testnummer) und klicken dort auf den Reiter **RUFUMLEITUNGEN**. Nun wählen Sie + RUFUMLEITUNG HINZUFÜGEN und dann **Ständig**.

![Anrufmenue_1_update](https://github.com/user-attachments/assets/2bcabf2c-8bdd-4a65-8e68-e36c013a1f76)

Anschließend klicken Sie rechts auf die drei grünen Punkte (roter Pfeil) und wählen **Weiterleitung an das Anrufmenü** aus:

![Anrufmenue_2](https://github.com/user-attachments/assets/b7951c53-1990-4283-807a-4f624cf8160a)

Um direkt auf das Anrufmenü umzuleiten, sollten sie den mittleren Eintrag *Weitergeleitet zu 📞 Nummer* löschen. Dafür rechts auf die **drei grünen Punkte** klicken, *Entfernen* auswählen und die Frage "Ziel löschen?" mit OK bestätigen.

![Anrufmenue_3](https://github.com/user-attachments/assets/7faf776d-df34-4b17-8be1-a7054fbbef8f)

Damit haben Sie die *Rufumleitung zum Anrufmenü* erfolgreich eingerichtet.

![Anrufmenue_4](https://github.com/user-attachments/assets/2646b9aa-964c-4838-81c6-cdc1c03493d5)
 
