---
title: "Anrufwarteschlangen einrichten"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 205
toc: true
---

Mit einer Anrufwarteschlange stellen Sie sicher, dass keine ankommende Anrufe verloren gehen. Die Anrufe werden gehalten und Ihre Kunden durch Ansagen informiert. Auch kann die Wartezeit durch das Einspielen von Musik erleichtert werden. Hier erfahren Sie, wie Sie Ihre Anrufwarteschlangen einrichten.

![cloudpbx warteschlange](https://user-images.githubusercontent.com/98753538/158607755-632e2eed-fe5a-499c-a9b5-3796d855abb8.jpg)

Klicken Sie bitte auf den Unterpunkt “Anrufwarteschlange” (1) und hier auf "+ ANRUFWARTESCHLANGE HINZUFÜGEN". 

Wählen Sie die Gruppe oder Nebenstelle (2) aus, für die Sie die Warteschlange konfigurieren.

Mit der Warteschlangenlänge (3) bestimmen Sie die maximale Anzahl der Anrufer, die gehalten werden.

Die Nachbearbeitungszeit (4) gibt dem Angerufenen z.B. 20 Sekunden Zeit, sich abschließende Notizen zu machen, bevor ihm der nächste gehaltene Anrufer zugestellt wird.

Abschließend klicken Sie auf "ANRUFWARTESCHLANGE HINZUFÜGEN".

![cloudpbx warteschlange2](https://user-images.githubusercontent.com/98753538/158609830-57f76e3a-e0e9-4ac6-8f42-d898c48c7c34.jpg)

Beispiel: In der Warteschlange "Schäl Sick" werden bis zu 5 Anrufer gehalten. Sind alle Abfrageplätze belegt, erhalten sie standardmäßig die folgende Ansagen (Soundset):

* "Alle Leitungen sind zur Zeit belegt. Ihr Anruf wird gereiht." (pbx queue_greeting)
* "Sie befinden sich zur Zeit an Position…" (pbx queue_prefix)
* "…der Warteschlange. Bitte legen Sie nicht auf." (pbx queue_suffix)
* Anschließend hört der Anrufer Musik. (pbx queue_waiting_music)

Übersteigt die Anzahl der Anrufer die *Warteschlangenlänge* (hier 5), wird diese Ansage geschaltet:

* "Alle Leitungen sind zu Zeit belegt. Bitte versuchen Sie es später erneut." (pbx queue_full)

In Klammern stehen die Namen des jeweiligen Soundsets, die Sie mit wenigen Mausklicks auf Ihr Unternehmen bzw. für Ihre Anrufer anpassen können.
Wenn Sie im Internet mit "text to speech german kostenlos" suchen, finden Sie leicht einen (kostenlosen) Text-zu-Sprache-Generator wie z.B. ttsfree, freetts oder ttsmp3. Dort können Sie Ihren gewünschten Ansagetext eingeben, wählen die Sprache und Stimme für die Ausgabe und erzeugen so eine mp3-Datei. Um diese in der Cloud-PBX verwenden zu können, ist noch eine Wandlung ins WAV-Format erforderlich. Entsprechende Konverter sind im Internet mit "mp3 wav converter" ebenfalls
sehr leicht zu finden. Wichtig: In Mono und nach a-Law konvertieren.

Wie Sie selbst erzeugte Ansagen in Ihre Cloud-PBX hochladen und aktiveren, steht im Kapitel [Soundsets](https://cloudpbx-doku.netcologne.de/docs/pbx-konfiguration/sound-sets/).
