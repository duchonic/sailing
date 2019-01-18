# perth waszp games (worlds 2019)
[official facebook page](https://www.facebook.com/waszpgames)<br>
[entry list](https://www.revolutionise.com.au/rfbyc/eventlist/20319)<br>
[weather forecast](https://www.seabreeze.com.au/weather/wind-forecast/perth)

## 18 January (Details)
Beim Segeln muss jewils alles passen um nicht ganz hinten zu landen. So habe ich die Unterschrift auf der Auslaufliste vergessen, dann nicht mitgekriegt dass die Australier 3 min Starts (statt 5 min) haben und zu guter letzt zwei mal Amwind gekentert. Der zweite und dritte Lauf dann viel bessert. Starts waren ok (Siehe Bild unten ganz rechts). Am Schluss waren es Rang 19,17. Wenn ich einstellige Ränge segeln will muss ich Amwind mehr höhe fahren, das geht nur mit viel Luvkrängung, aber heikel bei böigem Wind. Morgen geht's erst um 16:00 auf's Wasser, da am Samstag die Australier ihre Boote ausfahren und es erst spät genügend Platz für uns hat.<br>
[results](http://www.sportspage.com.au/yacht_clubs/rfbyc/WASZPnationals/WASZP_2019_Australian_Championship_Overall.htm)<br>

![pic](photos/start.jpg)
<br><br>
![pic](photos/perth.jpg)

## 17 January
"patchy wind" heisst es auf English. Auf dem Bild vom kleinen Berg, der in Windrichtung von unserem Regattarevier steht, schön zu sehen. Auf dem Photo hat es unten Zürichseewind von 2-4 kn aus allen Richtungen, in der Mitte Walenseewind von 10-15kn und am anderen Ufer dann australische 20-25kn. In der Mitte noch eine kleine Untiefe und viele Motorboote sowie Kursschiffe. Dazu ab morgen noch ca. 60 andere Waszps.
<br>Ziel für die nächsten zwei Tage der australischen Meisterschaften heisst, mal allen Problemen aus dem Weg gehen und vor dem dritten Tag auf der Jasstafel nachschauen, ob ich die Strategie anpassen muss.
![pic](photos/patchi.JPG)

## 16 January (Scheinbarer Wind)

[scheinbarer wind](https://de.wikipedia.org/wiki/Wahrer_und_scheinbarer_Wind#Scheinbarer_Wind)<br>
[beaufortskala](https://de.wikipedia.org/wiki/Beaufortskala)<br>
[knoten]( https://engineering.mit.edu/engage/ask-an-engineer/why-is-speed-at-sea-measured-in-knots/)

Heute waren es wieder rund 90 Minuten auf dem Wasser. Bei rund 20cm Welle macht das mit den Foilern richtig Spass. Vorwind hatte ich kaum Problem, auch durch die Halse kein Problem auf den Foils zu bleiben. Anders sieht der Amwindkurs aus. Wir hatten so 15kn plus alle 2-3 Minuten Böen bis 25kn für 30 Sekunden.

Gute 5 Beafourt.

Ich habe mich auf dem Heimweg gefragt, wieso hier ohne Welle der Vorwind einfacher ist als der Amwind. Habe das kurz durchgerechnet und wenn man die Resultate kurz studiert, wird auch klar, wieso Vorwind ohne Welle (voll) easy ist.

[norweger am fliegen](https://www.facebook.com/waszpgames/videos/388457785059272/)

Wahrer Wind + Fahrtwind = Scheinbarer Wind

Bewegt man sich auf dem Wasser (gleiches gilt auch an Land), ergibt sich aus dem Fahrtwind und dem wahren Wind der scheinbare Wind.

In Zahlen heisst das mit meinem fliegendem Boot:
- Amwind (+45° zum Wind) 15 kn wahrem Wind + 11 kn Fahrtwind = scheinbarer Wind von 24 kn (in der Böe 33 kn)
  - Amwind also 5-6 Beafourt
- Vorwind (-45° zum Wind) bei 15 kn wahrem Wind + 21 kn Fahrtwind = scheinbarer Wind von 15 kn (in der Böe 18 kn)
  - Downwind also 4-5 Beafourt

Als Fazit heisst das für mich Amwind alles dicht ziehen bis zum Anschlag und Vorwind auf keinen Fall abbremsen.

```python
import numpy as np
```


```python
def calcApparent(wind, boat):
    return np.linalg.norm(wind+boat)
```


```python
def calcSpeed(vector):
    return int(np.linalg.norm(vector))
```


```python
wind = np.array([0,15]); print('wind:', calcSpeed(wind),'kn')
gust = np.array([0,10]); print('gust:', calcSpeed(gust),'kn')
upwind = np.array([8,8]); print('upwind speed:', calcSpeed(upwind),'kn')
downwind = np.array([15,-15]); print('downwind speed:', calcSpeed(downwind),'kn')
```

    wind: 15 kn
    gust: 10 kn
    upwind speed: 11 kn
    downwind speed: 21 kn



```python
print('apparent up:  ', int(calcApparent(wind, upwind)),'kn', \
      'with gust:', int(calcApparent(wind+gust, upwind)),'kn')
print('apparent down:', int(calcApparent(wind, downwind)),'kn', \
      'with gust:', int(calcApparent(wind+gust, downwind)),'kn')
```

    apparent up:   24 kn with gust: 33 kn
    apparent down: 15 kn with gust: 18 kn

## 15 January
boat is ready, already flown perfectly<br>
![pic](photos/hardwork.gif)<br>
PPC (perfect perth condition)<br>
![pic](photos/perfect.png)

## 14 January (Perth)
hello sunshine<br>
![pic](photos/helloPerth.JPG)

## 12 January (Mühlehorn)
sailing stuff plus sharkknife packed, ready for Perth...<br>
![pic](photos/packing.JPG)

<iframe id="contactMap" src="https://maps.google.com.au/maps?f=q&amp;source=s_q&amp;hl=en&amp;geocode=&amp;q=Hobbs Place, Peppermint Grove WA 6011&amp;ie=UTF8&amp;t=m&amp;z=14&amp;output=embed"></iframe>

## Training
* 15 January 2019 Boatwork
* 16 January 2019 Practice Day 1
* 17 January 2019 Practice Day 2

## National Championship	 	
* 18 January 2019 Race Day 1
* 19 January 2019 Race Day 2
* 20 January 2019	Race Day 3

## International Waszp Games	 	
* 22 January 2019 Race Day 1
* 23 January 2019 Race Day 2
* 24 January 2019 Race Day 3
* 25 January 2019 Race Day 4
* 26 January 2019 Australia Day (no racing)
* 27 January 2019 Race Day 5
* 28 January 2019 Race Day 6

# garda waszp games (euro 2018)

![pic](img/garda2018_1.jpg)
