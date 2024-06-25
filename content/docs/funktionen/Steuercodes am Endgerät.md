---
title: "Steuercodes am Endgerät"
date: 2024-01-31T00:10:47+00:00
menu:
  docs:
    parent: "funktionen"
weight: 402
toc: true
---

Mit Hilfe von Steuercodes können Funktionen der Telefonanlage über jedes Endgerät auch direkt angesteuert werden. Hier eine Übersicht:

### Rückrufe

 zum letzten Anrufer:      __\*74*__ <br>

 zum letzten Angerufenen:  __\*95*__ <br>


### Anrufweiterleitung in CLOUDPBX

Die einzelnen [Call Forward Typen](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/#call-forward-typen) können durch Eingabe der einzelnen Feature Codes direkt am Endgerät aktiviert werden:

*Call Forward Unconditional:* Einrichtung der Rufumleitung durch Wahl von **\*72*Zielrufnummer** (inkl. Amtsholung) – *Deaktivierung durch Wahl von #72*.

*Call Forward on Busy:* Einrichtung der Rufumleitung bei Besetzt durch Wahl von **\*90*Zielrufnummer** (inkl. Amtsholung) – *Deaktivierung durch Wahl von #90*.

*Call Forward on Timeout:* Einrichtung der Rufumleitung nach Zeit durch Wahl von **\*92*30*Zielrunfummer** (hier also nach 30 Sekunden) – *Deaktivierung durch Wahl von #92*.

*Call Forward on Not Available:* Einrichtung der Rufumleitung bei „Nicht Registriert“ durch Wahl von **\*93*Zielrufnummer** - *Deaktivierung durch Wahl von #93*.

Die **Deaktivierung aller** eingerichteten Anrufweiterschaltungen erfolgt über den Feature Code **#96**.


### Weiterleitung zur Voicebox im TELEFON:

Weiterleitung (Ständig, Besetzt, Nichtmelden) im Telefon zu: **\*56*NST** (z. B. *56*12 für die Nebenstelle mit Durchwahl 12)<br>
Abschaltung durch Deaktivieren der Weiterleitung<br>
In vielen Endgeräten (z.B. Yealink) kann auch eine Zielwahltaste mit diesem Steuercode belegt werden. Das macht die Aktivierung und Deaktivierung der Weiterleitung komfortabler, da dann jeweils nur ein Tastendruck genügt. (s. auch [Anrufbeantworter (Voicemail) - NetCologne Cloud PBX](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufbeantworter/#4-aktivierung-mittels-weiterleitung-call-forward-im-telefon).


### Sonstiges

 Rufnummernunterdrückung: **\*31*Ziel**<br>
 
 Pickup: **\*99*Ziel** (Ziel entweder Nebenstellennummer oder SIP User)<br>
 
 Parken eines Anrufes: **\*97*Slot** (Slot ist Nummer zwischen 1 und 9)<br>
 
 Wiederholen geparkten Anrufes: **\*98*Slot** (von jedem Telefon der CPBX aus möglich - also zum Beispiel zum Übergeben eines Anrufes von der App zum Tischtelefon)<br>
