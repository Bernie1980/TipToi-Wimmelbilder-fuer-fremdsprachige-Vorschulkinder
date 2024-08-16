# TipToi-Wimmelbilder-fuer-fremdsprachige-Vorschulkinder

Moin moin,
mein Projekt hat wie im Betreff geschrieben das Ziel eine Hilfe für Vorschulkinder zu sein, mit der diese deutsche Wörter und Begriffe lernen können. Unsere Familie (Partnerin, Kinder, Enkelkinder) sind alle Dual Nations und zweisprachig aufgewachsen. Deshalb sind mir die Herausforderungen an Migranten bewusst, die ihren Kindern eine Sprache nur sehr schwer vermitteln können die sie selbst kaum sprechen.
Da kam mir die Idee mit dem TipToi-Stift und dazu speziell für die Kinder gemachte Bilder. Bei den Original TipToi-Büchern ist meiner Meinung nach zu viel Text um die Vokabeln "drum herum" und kann
fremdsprachige Kinder leicht überfordern.

Etwas ähnliches gab es ja schon mal mit dem Jugendforschtprojekt "Deutschlernen mit TipToi" (https://listi.jpberlin.de/pipermail/tiptoi/2023/002942.html )

Das ganze Thema wurde für mich aktuell als kürzlich Nachrichten durch die Presse gingen, wie viele Kinder den Wechsel in die zweite Klasse nicht schaffen, nur weil es an den entsprechenden Deutschkenntnissen
schon bei der Einschulung mangelt. Da Vorschulkinder noch nicht lesen können, haben sie fast keine Chance das selbstständig z.B. per Buch oder App zu tun.
Deshalb habe ich ein paar gebrauchte TipToi-Stifte gekauft und würde diese gerne zusammen mit den im Projekt erzeugten Bildern an Kitas in der Umgebung verteilen, damit die Kids dort spielerisch deutsch lernen
können.
Dabei möchte ich bei den Objekten auf den Bildern für jedes zwei Sprachausgaben generieren:
- das Singular mit Artikel    (der Hund)
- das Plural mit Artikel      (die Hunde)
 
Zusätzlich bei bestimmten Objekten (z.B. Tiere, Fahrzeuge) noch eine dritte Tonausgabe des für das Objekt typischen Geräusches (z.B. bellen beim Hund, knattern beim Moped).

Ich habe mich im Internet umgesehen und für mein Projekt zwei unterschiedliche Themen gefunden:
1. Die Sprachtafeln des Integrationsbeauftragten in Bayern
https://integrationsbeauftragte.bayern.de/infos-und-downloads/
2. Die Wimmelbilder der Firma Kölln
https://www.koelln.de/wissen-fun/wimmelbilder/

Programmiertechnisch war ich zwar etwas eingerostet (meine Diplomarbeit 1996 habe ich noch in Assembler und Ansi C geschrieben), habe das Programm aber dann doch recht schnell hinbekommen.
Das Wimmelbild habe ich selbst vertont und es funktioniert auch ganz gut. Nur bei dunklem Hintergrund muss man den Stift manchmal 2-3 mal aufsetzen. Das Lesen hat aber erst richtig geklappt, nachdem ich in Gimp
die Ebene mit den Oid-Codes verdreifacht und Ebenen-Kopie1 um einen Pixel nach rechts und Ebenen-Kopie2 um einen Pixel nach unten verschoben habe. Dass man die Oid-Codes schon "dicker" generieren kann hatte ich erst später
gesehen und dann keine Lust mehr die ganze Arbeit mit neuen Codes in Gimp nochmal zu machen.

Ich hatte anfangs die Sprachausgaben noch selbst eingesprochen. Aber nach dem ersten Themengebiet der Sprachtafel (Essen/Trinken) aufgegeben, da der Aufwand für knapp 600 Begriffe (300 * 2  für Singular und Plural) einfach zu hoch
war. Ich habe dann im TTTool auf "TextToSpeech" umgestellt. Aber ich fand die Aussprache der Ausgabe etwas "robotisch". Das soll keine Kritik sein. Ich finde es super, dass es so was überhaupt gibt.
Aber für jemanden der die deutsche Sprache lernen soll, denke ich ist es etwas schwierig.
Hier hat mir Jens sehr geholfen. Er hatte selbst für ein größeres Projekt den Text mit einem R-script in eine Tabelle exportiert und dann in der Google cloud mit TTS 
in MP3s umgewandelt. Bei der Anzahl von Wörtern ist das noch kostenlos. Das Ergebnis war sehr gut, überhaupt kein Vergleich zu dem integrierten TTS. 
Die Files hatte er wie die Texte in der yaml benannt, dadurch funktioniert das assemblen direkt auf den MP3s, ohne das die yaml angepasst werden muss. 
Also hat er mir für die Sprachtafel die Sounddateien erzeugt.
