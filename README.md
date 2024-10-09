# TipToi-Wimmelbilder-fuer-fremdsprachige-Vorschulkinder

Hallo,
mein Projekt hat wie im Betreff geschrieben das Ziel eine Hilfe für Vorschulkinder zu sein, mit der diese deutsche Wörter und Begriffe lernen können. Unsere Familie (Partnerin, Kinder, Enkelkinder) sind alle Dual Nations und zweisprachig aufgewachsen. Deshalb sind mir die Herausforderungen an Migranten bewusst, die ihren Kindern eine Sprache nur sehr schwer vermitteln können die sie selbst kaum sprechen.
Da kam mir die Idee mit dem TipToi-Stift und dazu speziell für die Kinder gemachte Bilder. Bei den Original TipToi-Büchern ist meiner Meinung nach zu viel Text um die Vokabeln "drum herum" und kann fremdsprachige Kinder leicht überfordern.

Das ganze Thema wurde für mich aktuell als kürzlich Nachrichten durch die Presse gingen, wie viele Kinder den Wechsel in die zweite Klasse nicht schaffen, nur weil es an den entsprechenden Deutschkenntnissen schon bei der Einschulung mangelt. Da Vorschulkinder noch nicht lesen können, haben sie fast keine Chance das selbstständig z.B. per Buch oder App zu tun.

Im Internet fand ich zu dem Thema TipToi die Seite (https://tttool.entropia.de/) von Joachim Breitner, der das TTTool entwickelt hat um individuelle Projekte für den TipToi-Stift erstellen zu können. Dort sah ich auch, dass etwas ähnliches bereits mit dem Jugendforschtprojekt "Deutschlernen mit TipToi" (https://listi.jpberlin.de/pipermail/tiptoi/2023/002942.html) gemacht wurde. Mit diesen Informationen beschloss ich mein eigenes Projekt zu starten.
Also habe ich ein paar gebrauchte TipToi-Stifte mit dem Ziel gekauft, diese zusammen mit den im Projekt erzeugten Bildern an Kitas in der Umgebung zu verteilen, damit die Kids dort spielerisch deutsch lernen können.

Für die Sprachausgabe möchte ich bei den Objekten (Substantive) auf den Bildern für jedes zwei Sprachausgaben generieren:
- das Singular mit Artikel    (der Hund)
- das Plural mit Artikel      (die Hunde)
Zusätzlich bei bestimmten Objekten (z.B. Tiere, Fahrzeuge) noch eine dritte Tonausgabe des für das Objekt typischen Geräusches (z.B. bellen beim Hund, knattern beim Moped).
Adejktive und andere Wortgruppen werden einfach mit einem Begriff ausgegeben.

Ich habe mich im Internet umgesehen und für mein Projekt zwei unterschiedliche Themen als Basis für die Bilder gefunden:
1. Die Sprachtafeln des Integrationsbeauftragten in Bayern
https://integrationsbeauftragte.bayern.de/infos-und-downloads/
2. Die Wimmelbilder der Firma Kölln
https://www.koelln.de/wissen-fun/wimmelbilder/

Das erste Wimmelbild (Im Zoo) habe ich selbst vertont und es funktioniert auch ganz gut. Nur bei dunklem Hintergrund muss man den Stift teilweise 2-3 mal aufsetzen. Das Lesen der Codes mit dem Stift hat aber erst richtig geklappt, nachdem ich in Gimp die Ebene mit den Oid-Codes verdreifacht und die Ebenen-Kopie 1 um einen Pixel nach rechts und die Ebenen-Kopie 2 um einen Pixel nach unten verschoben habe. Dass man die Oid-Codes schon "dicker" generieren kann hatte ich erst hinterher gesehen. 
Das nachträglich zu ändern hätte eine komplette Neugestaltung der Bilder erfordert, weshalb ich die beschriebene Alternative in Gimp benutzt habe.

Auh für das Bild "Sprachtafel" hatte ich anfangs die Audio-Dateien für die Sprachausgaben noch selbst eingesprochen. Aber nach dem ersten Themengebiet der Sprachtafel (Essen/Trinken) aufgegeben, da der Aufwand für knapp 600 Begriffe (300 * 2  für Singular und Plural) einfach zu hoch war. Ich habe dann im TTTool auf "TextToSpeech" umgestellt um die Audiodateien automatisch zu erzeugen. Aber ich fand die Aussprache der Ausgabe etwas "robotisch". Das soll keine Kritik sein. Ich finde es super, dass es so was überhaupt gibt. Aber für jemanden der die deutsche Sprache lernen soll, denke ich, ist es etwas schwierig zu verstehen. Vor allem wenn kleine Kinder die gesprochenen Wörter so wiedergeben wie sie diese gelernt haben.
Hier hat mir Jens sehr geholfen. Nach einem Aufruf in der Mailingliste zu TipToi (https://listi.jpberlin.de/mailman/listinfo/tiptoi) hat er mir seine Hilfe zur Erzeugung der Audio-Dateien angeboten. Er hatte selbst für ein größeres TipToi-Projekt den Text mit einem R-script in eine Tabelle exportiert und dann in der Google cloud mit TTS 
in MP3s umgewandelt. Bei der Anzahl von Wörtern ist das noch kostenlos. Das Ergebnis war sehr gut, überhaupt kein Vergleich zu dem integrierten TTS. 
Also hat er mir für die Sprachtafel die Sounddateien erzeugt.

