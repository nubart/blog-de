---
author_name: Rosa Sala
author_bio: Dr. Rosa Sala ist CEO und Gründerin von Nubart
author_location: Berlin / Barcelona
layout: post
comments: true
published: true
title:  "Warum wir digitale Audioguides im Offline-Modus ganz ohne App anbieten können"
description: "Museen haben oft eine schlechte Netzabdeckung und können unsere digitalen Audioguides nicht streamen. Deshalb haben wir einen Offline-Modus entwickelt, der kein Herunterladen von Apps erfordert!"
slug: "digitale-audioguides-offline-ohne-netzabdeckung"
date:   2018-06-14
banner_image: audioguide-nexo-nubart2.jpg
tags: [audio tour, offline]
---

Manchmal ist ein Problem eine verkleidete Chance. Das haben wir festgestellt, als wir für Nexo Turismo y Cultura die Audioführung zu den Naturdenkmälern von El Maestrazgo (Teruel, Spanien) produzierten. Es war der Ursprung unserer digitalen Offline-Audioguides für Smartphones, die ohne Wifi und ohne Datenabdeckung funktionieren. Hier ist die Geschichte. 

<!--more-->

## Wir erstellen nicht nur Audioguides für Museen, sondern auch Führungen in Naturgebieten
   
   Unsere Audioguide-Kärtchen sind nicht nur für Museen gut. Sie können auch für Führungen durch größere Gebiete, wie Städte oder Naturräume, verwendet werden. Noelia Porrúa bemerkte dies, als sie sich in der wunderschönen Region Maestrazgo in Teruel (Spanien) niederließ und beschloss, ihre Firma [Nexo Turismo y Cultura](https://www.nexoturismocultura.com/){:target="_blank"} zu gründen.
   
   Frau Porrúa setzte sich mit uns in Verbindung, weil sie neben den Führungen, die sie für Wanderer anbietet, sie auch etwas für Alleingänger haben wollte, die die natürlichen Sehenswürdigkeiten unbegleitet, in ihrem eigenen Tempo und in ihrer eigenen Sprache entdecken möchten. 
   
   Außerdem wollte sie auch die lokale Wirtschaft ankurbeln und unsere Karten in den örtlichen Geschäften vertreiben. Die spektakuläre Schönheit der Naturlandschaft von El Maestrazgo wird immer bekannter. "Es gibt viele Websites, die Informationen liefern - sagte uns Frau Porrúa -, aber man muss jede einzelne durchstöbern. Ich wollte, dass die Besucher alle Informationen auf ihrem Handy haben können. Aber auch, dass die Geschäfte in der Umgebung diese Informationen über einem physischen Format verkaufen. Das ist mit Euren Karten möglich". 

## Das Problem der Funklöchern in den Naturgebieten
   
   Frau Porrúa hatte ein tolles Skript vorbereitet, das von unserem Team ins Englische und Französische übersetzt wurde. Wir haben das Ergebnis in diesen beiden Sprachen und auf Spanisch besprechen lassen und die Landkarten überarbeitet, um sie an den Inhalt der Audioführung anzupassen. Um das Design der Audioguide-Karte mit Frau Porrúas Fotos kümmerten wir uns auch. 
   
   ![Nubart Audio Tour durch die Naturdenkmäler von El Maestrazgo - Nexo Turismo y Cultura]({{site.baseurl}}/images/posts/audioguide-nexo-nubart2.jpg){: .center-image }

   Alles lief wunderbar, bis wir sie nach der Twitter-Integration fragten.
   
   Unsere Audioguides haben eine "Tweet about this item"-Option, die es den Nutzern ermöglicht, für die Ausstellung oder den Rundgang von ihrem eigenen sozialen Netzwerk aus zu werben. "Es mag keine gute Idee sein, diese Option auf Ihrer Route zu verwenden", sagten wir Frau Porrúa. Unser Inhalt ist zwar so bearbeitet, dass kaum Daten verbraucht werden und es sehr schnell lädt, die Twitter-App funktioniert aber langsam, wenn die Netzabdeckung mangelhaft ist. "In diesem Fall sollten wir es lieber ganz sein lassen, denn in El Maestrazgo gibt es überhaupt keine Netzabdeckung", erwiderte sie. 

Autsch... Wie bitte? *Überhaupt keine* Netzabdeckung? 

Unsere Nubart-Karten wurden zu diesem Zeitpunkt ausschließlich *gestreamt*, so dass Wifi oder Datenabdeckung, wie schlecht diese auch immer sein mag, zu ihrer Nutzung erforderlich waren. Der Inhalt für Nexo war bereits produziert, die Audio-Tour hochgeladen und die Karten gedruckt, aber ohne Daten oder Wifi waren sie nutzlos. 
Aber Frau Porrúa hatte Recht: El Maestrazgo befindet sich mitten in einem Funkloch und wir hatten nicht damit gerechnet. 
Wir standen vor einem Problem. Wir hatten alle viel Zeit und Enthusiasmus für dieses Projekt aufgewendet. Jetzt konnten wir mit den 5.000 gedruckten Karten einen hübschen Untersetzer basteln und der Kundin das Geld zurückgeben, oder nach einer technischen Lösung suchen. 
Wir entschieden uns für das Zweite. 

## Das Problem des Offline-Abrufen von Inhalten ohne dafür eine App zu installieren
   
   Wir mussten einen Weg finden, damit der gesamte inhalt des Audioguides an einem Ort mit guter Abdeckung vorgeladen werden konnte, um später offline darauf zugreifen zu können. Theoretisch ist das nur mit nativen mobilen Apps möglich. Aber bei Nubart glauben wir nicht an Apps. Der Zugang zum Inhalt musste schneller und unmittelbarer stattfinden, ohne dass die Nutzer den lästigen Prozess der Suche nach einer App im Shop, des Herunterladens, der Installation, des Öffnens und der Vergabe von Berechtigungen durchlaufen müssen. Aber wir wollten auch nicht den Handy-Speicher verbrauchen, wie es einmal installierte Apps nun mal tun. 
   Das "preload"-Attribut in html war keine brauchbare Lösung, da praktisch keiner der mobilen Browser diesem Attribut Folge leistet. 
   Wahrscheinlich würden Ihnen 95% der Softwarefirmen sagen, dass dieses Problem ohne der Entwicklung einer App nicht lösbar ist.
   
## Wie funktionieren unsere Audioguides im Offline-Modus?
   
   Unser Mitbegründer und CTO Simon Effing fand den Weg. Mit eine smarten Anwendung von Javascript der letzten Generation konnte er sicherstellen, dass der komplette Inhalt des Audioguides immer von jedem Browser vorgeladen und vorläufig im temporären Speicher des Mobiltelefons (= "Random Access Memory") gespeichert wird. Die im RAM enthaltenen Informationen verbrauchen keinen Speicher, da sie beim Schließen der Browserseite oder beim Ausschalten des Gerätes von selbst verschwinden. Aber dadurch gehen sie nicht für immer verloren: Benutzer können sie jederzeit wiederherstellen, indem sie den eindeutigen Code ihrer Nubart-Karte verwenden. All dies geschieht schnell und ohne Download von Apps.
   In diesem Video sehen Sie den gesamten Prozess in Echtzeit:
   <iframe src="https://player.vimeo.com/video/250765199" width="640" height="360" frameborder="0" webkitowowowfullscreen mozallowfullscreen allowfullscreen></iframe>{: .center-image }
   Der Zugriff auf unsere Offline-Audiotouren ist genauso einfach wie der Zugriff auf unsere Standard-Audioguides in Streaming. Man muss nur ein bisschen länger warten, bis der gesamte Inhalt vorgeladen ist.
   So hatten wir nicht nur Frau Porrúas Problem gelöst. Es war uns sofort klar, dass auch andere Kunden vom Offline-Modus profitieren konnten, wie z.B. Museen die zwar Wi-Fi im Empfangsbereich anbieten, aber keine Abdeckung in den restlichen Räumen anbieten. Auch Touristen von ausserhalb der EU können so auf das teure *Roaming* versichten, da sie einen kostenlosen Wifi-Spot zum Herunterladen der Inhalte nutzen können.
   Inzwischen haben wir diese Entwicklung erweitert und bieten nun auch eine Hybridlösung an, bei der nur die Audiospuren, die Bereichen mit schlechter Konnektivität zugeordnet sind, von uns in den Offline-Modus geschaltet werden. Dies verbessert die Ladegeschwindigkeit.



#### Bei Nubart produzieren wir innovative und kostengünstige Audioguides.

<form action="../../../../../">
    <input type="submit" value="Besuchen Sie unsere Website" />
</form>