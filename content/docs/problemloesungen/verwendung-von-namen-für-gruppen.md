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
Beim Anlegen einer Gruppe ist darauf zu achten, dass für den Gruppennamen nur Kleinbuchstaben verwendet werden. Leer- und Sonderzeichen sowie Ziffern führen zu unerwünschtem Fehlverhalten, da das System die Namen intern anders darstellt.
Sollten Sie bei der Namensgebung nicht auf Ziffern oder besondere Schreibweisen verzichten wollen, so sind folgende Hinweise zur internen Darstellung zu beachten:

eingegebener Name -> wird zu
Maxmustermann -> maxmustermann
MaxMustermann -> max-mustermann
max mustermann -> max-mustermann
mustermann2 -> mustermann-2
mustermann_2 -> mustermann-2

Formate, die in das gleiche interne Format umgewandelt werden, dürfen nicht gleichzeitig verwendet werden.
