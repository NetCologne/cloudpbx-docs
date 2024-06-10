---
title: "Verwendung von Namen für Gruppen"
date: 2024-06-10T08:22:22+00:00
menu:
  docs:
    parent: "problemloesungen"
weight: 604
toc: true
---

## Verwendung von Namen für Gruppen
Beim Anlegen einer Gruppe ist darauf zu achten, dass für den Gruppennamen nur Kleinbuchstaben verwendet werden. Leer- und Sonderzeichen sowie Ziffern führen zu unerwünschtem Fehlverhalten, das das System die Namen intern anders darstellt.

Sollten Sie bei der Namensgebung nicht auf Ziffern oder besondere Schreibweisen verzichten wollen, so sind folgende Hinweise zur internen Darstellung zu beachten:

**eingegebener Name -> wird zu**<br>
Maxmustermann -> maxmustermann<br>
MaxMustermann -> max-mustermann<br>
max mustermann -> max-mustermann<br>
mustermann2 -> mustermann-2<br>
mustermann_2 -> mustermann-2<br>

Formate, die in das gleiche interne Format umgewandelt werden, dürfen nicht gleichzeitig verwendet werden.
