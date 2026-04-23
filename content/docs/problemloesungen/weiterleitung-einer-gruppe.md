---
title: "Weiterleitung einer Gruppe"
date: 2026-04-20T08:22:22+00:00
menu:
  docs:
    parent: "problemloesungen"
weight: 606
toc: true
---

Bei der hier beschriebenen Funktion handelt es sich um eine Sonderlösung, welche unter bestimmten Umständen sehr zweckmäßig sein kann.
Hier wird eine Lösung beschrieben, wie eine Gruppe durch einen Mitarbeiter, welcher nicht selbst Mitglied der Gruppe ist, auf eine dedizierte 
Nummer ( zB. eine Handy-Nummer ) umgeleitet werden kann. Die Aktivierung / Deaktivierung der Weiterleitung liegt jeweils auf einer Kurzwahl-Taste
mit entsprechendem Beschriftungs-Label im Telefon und kann damit per "Knopfdruck" ein- oder ausgeschaltet werden. 
Die Konfiguration kann auf 2 Wegen erfolgen ( Konfiguration via CSC-UI oder Konfiguration via Telefon-UI ) 
mit der Ausnahme der Telefon-Tasten-Beschriftung (Label), diese kann nur über die Telefon-UI erfolgen.
## 1. Konfiguration via WEB-UI 
Schritt 1 ( Darstellung der Gruppe, welche weiterleitungsfähig gemacht werden soll )
![Gruppe_Zentrale](https://github.com/user-attachments/assets/3c80029f-c2c2-431e-bfc7-27f05e394d68)
Schritt 2 ( Darstellung des Users, welcher die Weiterleitung aktivieren/deaktiviern können soll )
![Geräte_Konfig_0](https://github.com/user-attachments/assets/ad5e1627-baec-4142-af11-02a9145dadbe)
Schritt 3 ( Darstellung des Users Voreinstellung )
![Geräte_Konfig_1](https://github.com/user-attachments/assets/34a09732-1b7b-4b68-9388-adbc965b4752)
Schritt 4 ( Konfiguration der Line "Gruppe " auf Telefon des Users )
![Geräte_Konfig_2](https://github.com/user-attachments/assets/1057f995-19b4-40c6-9372-f577f46a2727)
Schritt 5 ( Konfiguration der Kurzwahl für Call Forward der Gruppe aktivieren )
![Geräte_Konfig_3](https://github.com/user-attachments/assets/e58f2545-15e7-4240-b106-6392559b8a27)
Schritt 6 ( Konfiguration der Kurzwahl für Call Forward der Gruppe deaktivieren )
![Geräte_Konfig_4](https://github.com/user-attachments/assets/2953ea6d-0df9-49bd-aac9-c69be2bd507a)

## 2. Konfiguration via Telefon-UI ( zB. Yealink T53W ) 
Schritt 1
![1_Konto_User_Registrieren](https://github.com/user-attachments/assets/e8bae4e9-7500-45d8-a54f-e2a32288cce8)
Schritt 2
![2_Konto_Gruppe_Registrieren](https://github.com/user-attachments/assets/72504092-dff8-4fb5-8c54-a497d3015cea)
Schritt 3
![3_Line_Key_Konfigurieren](https://github.com/user-attachments/assets/a27374c6-2ac9-4677-a7fb-53fabb28c5f7)
