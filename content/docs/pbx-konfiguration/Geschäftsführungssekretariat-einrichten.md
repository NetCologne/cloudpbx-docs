---
title: "Geschäftsführungssekretariat einrichten"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 207
toc: true
---

Die Cloud-PBX-Funktion **Geschäftsführungssekretariat** bietet die Möglichkeit Anrufe zur Geschäftsführung (Chef/Chefin) gezielt zu steuern. Sämtliche Anrufe zur  Durchwahl des/der Vorgesetzten, werden zunächst zu einem Mitarbeiter (Sekretär/in) weitergeleitet und dort entgegengenommen. Je nachdem, ob Gespräche gewünscht sind, können Anrufe dann zum Vorgesetzten druchgestellt oder ggf. direkt vom Mitarbeiter (Sekretär/in) beantwortet werden.

## 1. Grundkonfig einrichten 

Im Beispiel ist *porz* der Geschäftsführer. Das *Sekretariat* hat die Rufnummer 492212615245417. In der PBX-Konfiguration den Menuepunkt **Geschäftsführungssekretariat** anklicken, dann den Manager (hier: porz) auswählen.

![GF-Sekretärin einrichten](https://user-images.githubusercontent.com/98753538/232427318-0c806532-a1e5-46ea-9d12-82b016094988.jpg)

Nun diesem die Rufnummer des Geschäftsführungssekretariat zuweisen und die Konfiguration bestätigen.

![GF-Sekretärin hinzufügen](https://user-images.githubusercontent.com/98753538/232438884-e6149b06-112e-4c77-b6b8-e1d0c56ebda6.jpg)

Damit ist die Rufnummer 492212615245417 als Geschäftsführungssekretariat "definiert".

## 2. Konfiguration durch Rufumleitung aktivieren

Damit diese Konfiguration genutzt werden kann, muss nun noch für die Nebenstelle *porz* eine *Rufumleitung zum Geschäftsführungssekretariat* eingerichtet werden. 
Dafür unter **PBX-Konfiguration** den Unterpukt **Nebenstelle** anklicken und *porz* auswählen.

![GF-Sekretärin hinzufügen](https://github.com/user-attachments/assets/48a073b7-ef58-44ee-ad9b-6d8bbdac26ee)

Nun den Punkt **Rufumleitungen** auswählen und **+ RUFUMLEITUNG HINZUFÜGEN** anklicken und im Menue *ständig* auswählen.
Im nächsten Schritt rechst neben *Ständig und Y Bedingung* auf die **drei grünen Punkte** klicken und *Weiterleiten an Geschäftsführungssekretariat* auswählen.

![GF-Sekretärin weiterleiten](https://github.com/user-attachments/assets/b54fa552-4dd0-4d28-bee6-77e2f0e36ea4)

Um direkt auf das Geschäftsführungssekretariat umzuleiten, sollten sie den mittleren Eintrag *Weitergeleitet zu ( Nummer* löschen. Dafür rechts auf die **drei grünen Punkte** klicken, *Entfernen* auswählen und die Frage "Ziel löschen?" mit OK bestätigen.

![GF-Sekretärin weiterleiten zu Nr  entfernen](https://github.com/user-attachments/assets/f0da15a8-0db1-469f-9502-1eb2d739a14e)

Damit haben Sie die *Rufumleitung zum Geschäftsführungssekretariat* erfolgreich eingerichtet.

![GF-Sekretärin Weiterleitung steht](https://github.com/user-attachments/assets/2dab0cef-5ff1-4d17-b0c7-ffa058a6bf5f)
