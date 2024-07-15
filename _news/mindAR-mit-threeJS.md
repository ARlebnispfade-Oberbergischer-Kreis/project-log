---
layout: simple
title: MindAR und threeJS
subtitle: 09.07.2024
---

Als eine möglich Alternative für AR.js und A-Frame wurde mindAR mit threeJS testweise implementiert.

Grundlegend ist mindAR mit threeJS leichtgewichtiger, jedoch ist das Tracking multipler Images komplizierter als bei A-Frame.
A-Frame kommt zudem mit sehr wenig JavaScript aus, threeJS hingehen funktioniert nur mit JavaScript.

mindAR mit threeJS funktioniert sehr gut mit Videos und Audio, bei 3D Modellen bietet sich aber AR.js und A-Frame besser an.

Welche der beiden Technologien verwendet werden soll kann über das Attribut *layout* in der markdown-Datei des Spots festgelegt werden.