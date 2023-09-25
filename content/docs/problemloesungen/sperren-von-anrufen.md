---
title: "Sperren von Anrufen"
date: 2023-09-25T00:11:33+00:00
menu:
  docs:
    parent: "problemloesungen"
weight: 601
toc: true
---

Wenn Sie wünschen, dass eine Nebenstelle von bestimmten Rufnummern nicht erreicht werden darf oder nur von bestimmten Rufnummern erreicht werden soll, können Sie entsprechende Call Blockings konfigurieren. Öffnen Sie dafür in den Kunden-Details den Punkt Einstellungen.

![Call_Blocking_1](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/c003de10-75f8-4b69-8688-51b1b30f1c40)

Unter Call Blockings können Sie den Modus (Black- oder Whitelist) einstellen und eine Liste von Rufnummern erstellen, für die der Modus gilt.

![Call_Blocking_2](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/4ecac89c-c3d8-41db-a3da-abbca5583d12)

## Call Blocking per Blacklist

Das ist die Default-Einstellung, d.h. beim Block Mode ist KEIN Häkchen (roter Pfeil) gesetzt. Die bei der Block List eingetragenen Rufnummern oder Rufnummernbereiche werden geblockt. Im Beispiel sind dies die Ortsnetze Düsseldorf (49211*) und Bonn (49228*).

![Call_Blocking_3](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/f78dd4df-11a2-4ae0-a0a5-af9252687f0c)

## Call Blocking per Whitelist

Beim Block Mode ist das Häkchen (roter Pfeil) gesetzt und es werden nur die in der Block List eingetragenen Rufnummern(bereiche) NICHT blockiert. Im Beispiel sind dies alle Rufnummern aus Deutschland (beginnend mit 49).

![Call_Blocking_4](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/9b2af1d4-7ab3-4e94-83ff-ff775a60b517)

## Call Blocking von externen Anrufen

Ist es gewünscht, dass eine bestimmte Nebenstelle (z.B. das Wartezimmer) nur von den anderen Nebenstellen der Cloud-PBX erreichbar ist, dann setzten Sie im Feld „Block Mode for inbound calls“ das Häkchen (-> Aktivierung Whitelist). Anschließend tragen Sie bei der „Block List for inbound calls“ die anderen Rufnummern Ihrer TK-Anlage ein. Das Fragezeichen steht für eine beliebige Ziffer. Die TK-Anlage im Beispiel hat also die Stammnummer 4922126152 mit zwei- und dreistelligen Durchwahlen.

![Call_Blocking_5](https://github.com/NetCologne/cloudpbx-docs/assets/98753538/de5772cf-08fd-41c7-9988-6d4461a5aebd)

Ergebnis: Die internen Anrufe (der Whitelist) werden durchgelassen und alle Calls von außerhalb werden mit SIP Cause 403 "Blocked by Callee" ausgelöst.
