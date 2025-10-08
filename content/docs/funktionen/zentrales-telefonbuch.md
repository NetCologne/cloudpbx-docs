---
title: "Zentrales Telefonbuch"
date: 2023-08-02T08:54:22+00:00
menu:
  docs:
    parent: "funktionen"
weight: 495
toc: true
---

Zurzeit unterstützen ausschließlich die Endgeräte von Yealink das zentrale Telefonbuch. Dabei ist wichtig, dass die Geräte entsprechend der Anleitung unter PBX-Konfiguration eingerichtet wurden.

Im Endgerät können dann noch zwei Parameter nach Kundenwunsch angepasst werden. Dazu wird hier exemplarisch die Benutzeroberfläche des Yealink T53W dargestellt.

![Yealink_T53W_Verzeichnis-Ext_TelBuch_ein](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/9e2bfa8b-a21c-4460-b954-7d9fc5b45d6c)

Der Schalter „Suche nach eingehendem/ausgehendem…“ steuert die Anzeige des Namens im Display des Telefons. Wenn der Schalter auf „ein“ steht, wird bei einem kommenden Anruf der Name zusätzlich zur Rufnummer des Anrufers im Display angezeigt, sofern ein zugehöriger Eintrag im Telefonbuch existiert. Bleibt der Schalter auf „aus“, wird lediglich die Rufnummer des Anrufers angezeigt. Voraussetzung ist, dass der Anrufer seine Rufnummer nicht unterdrückt.<br>
Der Parameter „Update-Zeitintervall (Sekunden)“ legt fest, in welchem Abstand das Telefon das Telefonbuch mit dem Server abgleicht. Das kürzeste einstellbare Intervall sind 3600 Sekunden.

Über das Menü des Telefonbuchs am Endgerät (nur Tischtelefone) kann der Benutzer den Abgleich auch manuell initiieren. Über die Taste "Directory" wird die Liste der externen Telefonbücher aufgerufen. Standardmäßig ist das Telefonbuch der Cloud PBX enthalten. Falls mehrere Telefonbücher angezeigt werden, muss das zentrale Telefonbuch der Cloud mit den Pfeiltasten markiert werden. Dann wird über die Taste "Aktu" (aktualisieren) das aktuelle Telefonbuch in das Telefon heruntergeladen.

Das Telefonbuch in den DECT Endgeräten wird nach der eingestellten Zeit in der Basisstation automatisch aktualisiert. Eine manuelle Aktualisierung ist nur möglich, indem die Basisstation neu gestartet wird. Das empfiehlt sich nur in dringenden Fällen, da bestehende Telefongespräche, die über die Basisstation laufen, unterbrochen werden.

Einträge und Änderungen im zentralen Telefonbuch können nur vom Administrator durchgeführt werden. Es gibt zwei Möglichkeiten, die Telefonbucheinträge zu bearbeiten:<br>
1.	Einträge manuell durchführen<br>
2.	Einträge per CSV-Datei hochladen<br>

Name und Telefonnummer können manuell über die GUI der Cloud PBX eingetragen werden. Diese Methode ist für wenige Einträge bzw. Änderungen sinnvoll. Der Administrator wählt im Menü den Eintrag "PBX-Konfiguration" und dann "Telefonbuch des Kunden".

![phonebook](https://github.com/user-attachments/assets/281960d3-c94c-46bd-8cbd-b960d7231059)

In diesem Beispiel ist der Eintrag "Mustername1 Vorname" bereits vorhanden. Weitere Einträge können durch Klick "+ TELEFONBUCH HUNZUFÜGEN" vorgenommen werden.

![phonebook_manueller_Eintrag](https://github.com/user-attachments/assets/41539b7e-6a1a-4e82-aa8f-f77091e1719f)

In dem Feld für den Namen darf kein Komma verwendet werden, da es intern schon als Trennzeichen verwendet wird.

Um eine größere Anzahl von Einträgen vorzunehmen, bietet sich das Hochladen einer CSV-Datei an. Dabei ist folgendes Format zu verwenden:<br>
Name, Rufnummer

Als Trennzeichen wird das Komma verwendet. Daher darf es nicht im Namensfeld verwendet werden.<br>
Die Rufnummer muss immer im internationalen Format, beginnend mit „+“, eingetragen werden.<br>
Beispiel:<br>
Mustername1, +492214711<br>
Mustername2, +492214712<br>
Mustername3, +4922122299764<br>

Beim Hochladen muss dann die gewünschte Datei ausgewählt werden. Außerdem muss festgelegt werden, ob die vorhandenen Daten im Telefonbuch gelöscht werden sollen. In diesem Fall ist der Punkt „Vorhandenes bereinigen“ auszuwählen.

![phonebook_csv](https://github.com/user-attachments/assets/f66db0eb-a09b-4bf9-a643-2e9305442882)

Wird diese Funktion nicht aktiviert, werden die Zeilen aus der CSV-Datei zusätzlich in das Telefonbuch eingetragen. Diese Methode eignet sich sehr gut, um eine größere Anzahl zusätzlicher Rufnummern einzutragen.

Befinden sich bereits Einträge in dem Telefonbuch, so empfiehlt es sich, diese zunächst als CSV-Datei herunterzuladen und so eine Datensicherung zu erstellen. Eine Kopie dieser Datei kann dann bearbeitet und anschließend wieder hochgeladen werden.

Nebenstellen, die zur Cloud PBX gehören, werden im Telefonbuch des Endgerätes immer angezeigt. Sie können nicht entfernt werden. In der zentralen Liste werden sie nicht aufgeführt.
