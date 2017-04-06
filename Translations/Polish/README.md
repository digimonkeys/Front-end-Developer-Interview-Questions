#Pytania kwalifikacyjne na stanowisko front-end web developera

@version 2.0.0

To repozytorium zawiera wiele pytań weryfikujących wiedzę potencjalnych kandydatów na stanowisko front-end web developera. Nie zaleca się zadawania wszystkich pytań jednej osobie (zajęłoby to godziny). Wybranie pojedynczych pozycji z listy pomoże w sprawdzeniu wymaganych umiejętności.

[Rebecca Murphey](http://rmurphey.com/) opracowała [Podstawowe wymagania dla Front-End web developerów](http://rmurphey.com/blog/2012/04/12/a-baseline-for-front-end-developers/), które są warte przeczytania zanim udamy się na rozmowę o pracę.

**Uwaga:** Pamiętaj, że wiele pytań jest otwartych, co prowadzi do ciekawych dyskusji, które powiedzą Ci więcej o możliwościach danej osoby, niż w przypadku prostej odpowiedzi.

#### Pierwotni autorzy

Większość pytań zaczerpnięto z wątku [oksoclap](http://oksoclap.com/) stworzonego pierwotnie przez [Paula Irisha](http://paulirish.com) ([@paul_irish](http://twitter.com/paul_irish)) i rozwijanego przez następujące osoby:

* [@bentruyman](http://twitter.com/bentruyman) - http://bentruyman.com
* [@cowboy](http://twitter.com/cowboy) - http://benalman.com
* [@ajpiano](http://ajpiano) - http://ajpiano.com
* [@SlexAxton](http://twitter.com/slexaxton) - http://alexsexton.com
* [@boazsender](http://twitter.com/boazsender) - http://boazsender.com
* [@miketaylr](http://twitter.com/miketaylr) - http://miketaylr.com
* [@vladikoff](http://twitter.com/vladikoff) - http://vladfilippov.com
* [@gf3](http://twitter.com/gf3) - http://gf3.ca
* [@jon_neal](http://twitter.com/jon_neal) - http://twitter.com/jon_neal
* [@wookiehangover](http://twitter.com/wookiehangover) - http://wookiehangover.com
* [@darcy_clarke](http://twitter.com/darcy) - http://darcyclarke.me
* [@iansym](http://twitter.com)

### Pytania ogólne:

* Czego nauczyłeś się wczoraj/w tym tygodniu?
 React Higher Order Components
 Sequelize ORM dla NodeJS

* Co pobudza lub interesuje cię w programowaniu?

Tworzenie rzeczy. Od dziecka uwielbiałem tworzyć coś nowego i rozwiązywac łamigłówki. Uwielbiam stale się rozwijać, uczyć się nowych rzeczy i codziennie stawiać czoła nowym wyzwaniom.

* Jakie wyzwanie technologiczne stanęło przed toba ostatnio i jak je rozwiązałeś?
Pracowałem nad projektem wykorzystującym boilerplate bundlujący się przez starą wersję webpacka. Kiedy chciałem dodać do niego kilka niezbędnych rozszerzeń, wszystko okazało się niekompatybilne i rozsypało w drzazgi. Musiałem napisac cały skrypt webpacka od nowa.

* Jak planujesz budowę UI, utrzymanie bezpieczeństwa, wysoką wydajność, SEO, łatwość w utrzymaniu kodu i jakie wykorzystujesz technologie kiedy zaczynasz budować aplikację webową lub stronę internetową?

UI - zazwyczaj zaczynam od narysowania interfejsu na kartce papieru, która później służy mi jako generalny wyznacznik tego, co chcę osiągnąć na koniec pracy. Zawsze przykładam wagę do czytelności i prostoty interfejsu dla użytkowników.

Bezpieczeństwo - ponieważ po stronie klienta z kodem może stać się wszystko, trzymam wszystkie wrażliwe dane po stronie serwera.

Wydajność - skupiam się na pisaniu przejrzystego, zrozumiałego kodu, a gdy któraś funkcjonalność okazuje się zbyt wolna pracuje nad poprawieniem jej wydajności. Czasem jeśli jakiś problem wydaje mi się 'ciężki' dla aplikacji i moge go rozwiązać na kilka sposobów, od razu wykonuje pomiar czasów wykonania przy różnych rozwiązaniach.

SEO - nie zajmuję się optymalizacją SEO (nie bywało to moim zadaniem)

Utrzymanie kodu - stosuję ogólne dobre praktyki, takie jak proste i czytelne nazywanie funkcji i zmiennych, dzielenie kodu na małe, proste moduły. Zawsze kładę wielki nacisk na przystosowanie mojego kodu do zwyczajów panujących w zatrudniającej mnie firmie.

Technologie - ostatnio preferuję React i redux w połączeniu z webpackiem, ale używałem również angulara 1 z gulpem itd itp

* Jakie jest Twoje preferowane środowisko programistyczne? (system operacyjny, edytor, przeglądarki, narzędzia itd.)  
Używam sublime 3 z jego dodatkowymi pluginami i świetnymi funcjonalnościami pomagającymi w edycji tekstu. Preferuję pracę na chromie i jego dev toolsach, ale używam też firebuga. Mam pewną wiedzę na temat linuksa, ale obecnie pracuję na win10. Korzystam też z gulpa, webpacka, managerów okien linterów itp.  

* Z jakimi systemami kontroli wersji pracowałeś / jesteś zapoznany?  
Z gitem, pracowałem na githubie i gitlabie. Próbowałem używać interfejsów graficznych gita, ale jednak wolę pracować w command line.  

* Opisz kolejne zadania podczas tworzenia strony internetowej? 
Najpierw zbieranie wymagań klienta, funkcjonalnych i niefunkcjonalnych.
Tworzenie środowiska - skrypty służące do budowania w środowisku developerskim i produkcyjnym - webpack, gulp.
Szkielet strony i semantyka, wypełnienie kontentem + poprawa semantyki, stylowanie, animacje, dodawanie interaktywności.  

* Opisz różnicę między stopniowym ulepszaniem (progressive enhancement) i wdzięczną degradacją (graceful degradation)?
  * Dodatkowe punkty za opisanie wykrywania obsługi cech (feature detection)  
  
* Wyjaśnij, co kryje się za terminem "semantyczny HTML".  
Semantyczny HTML - jest to używanie znaczników / tagów HTML zgodnie z ich przeznaczeniem i znaczeniem semantycznym, a nie tylko do prezentowania danych. Znaczniki nadają sens i w różnym kontekście mogną oznaczać do innego. Np <i> i <em> <b> i <strong>, section, aside, nav. Jest to ważne dla robotów indeksujących google, dla czytników przeznaczonych dla osób niepełnosprawnych etc.  

* Jak optymalizowałbyś zasoby strony internetowej?  
Optymalizacja obrazków, łączenie plików, Zmniejszenie rozmiaru plików przy użyciu uglifyjs, stosowanie minifikacji, używanie SVG i css sprites (jeden obrazek, używany wiele razy), Zasoby CDN - mogą być serwowane w zależności od odległości od użytkoniwka, response time etc, cachowanie, nie ładować dużych bibliotek jeśli potrzebujemy z nich tylko jednej funkcji  

* Dlaczego serwowanie zasobów strony przez wiele domen jest lepsze?  
Ponieważ pozwala na użycie lżejszego serwera, który nie będzie musiał ładować modułów wymaganych do serwowania dynamicznych treści przy każdym requeście o zasoby statyczne. Dodanie domeny oznacza, że zwięszymy liczbę możliwych równoległych pobrań dla przeglądarki. Można równiez wykorzystać brak potrzeby wysyłania plikow cookie przy przesyłaniu statycznych treści (css, obrazków, plików js) co zmniejszy obciażenie sieci.
http://webmasters.stackexchange.com/a/26757
http://webmasters.stackexchange.com/a/25091 

* Ile zasobów pobiera przeglądarka z danej domeny w jednej chwili?  
Starsze przeglądarki jak IE6 - 2, nowsze 6 / 8.  

* Podaj 3 sposoby na zmniejszenie czasu ładowania strony. (postrzeganego lub rzeczywistego czasu ładowania)
* Jeśli dołączasz do projektu, w którym używa się tabulacji, a ty używasz spacji, co wtedy zrobisz?
  * Sugerowanie użycia narzędzi w stylu EditorConfig (http://editorconfig.org)
  * Zgodnie z konwencjami (pozostań konsekwentny)
  * `issue :retab! command`
  Dostosuję się. Wystarczy przecież zmienić ustawienia edytora.

* Napisz prosty pokaz slajdów
  * Dodatkowe punkty, jeśli nie używasz JS.
Można to zrobić za pomocą CSS3 wykorzystując unordered list i input type = radio. Najistotniejsze elementy kodu:

```
<li>
    <input type="radio" id="slide1" name="slide" checked>
    <label for="slide1"></label>
    <img>
</li>
.your-ul-class img {
    opacity: 0;
    visibility: hidden;
}
.ul-class li input:checked ~ img {
    opacity: 1;
    visibility: visible;
    z-index: 10;
}
```

Pełny tutorial: http://joshnh.com/weblog/making-a-pure-css-featured-image-slider/

* Jakich narzędzi używasz do sprawdzenia wydajności swojego kodu?
  * Profiler, JSPerf, Dromaeo  
Chrome Timeline - dostępne w devTools, nagrywa i pozwala na analizę wszystkich aktywności aplikacji podczas jej działania 
JSPerf - jsPerf umożliwia łatwe tworzenie i udostepnianie testów wydajności, porównując wydajność snippetów JS przez testy benchmarkowe
 Dromaeo - zetaw testów wydajności dla JS od Mozilli, obecnie nadal w fazie rozwoju  
https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/timeline-tool  
https://jsperf.com/  
https://wiki.mozilla.org/Dromaeo  

* Gdybyś mógł opanować jedną technologię w tym roku, jaka byłaby to technologia?
* FOUC? Jak unikasz FOUC?
* Wyjaśnij znaczenie standardów sieciowych i ich twórców.  

Standardy są bardzo istotne ponieważ aplikacje pisane w danym języku są kompilowane przez różne przeglądarki. Pozwala to uniknąć sytuacji, w której kod działa w połowie przeglądarek, lub działa tylko w tej ulubionej kodera. Gdy opracowany jest standard przeglądarki wiedzą czego się spodziewać i każdy piszący w zgodzie ze standardem może zakładać, że wszystko będzie działać. Twórcami standardów są w3c, iso, ansi, unicode consortium, ietf oraz ecma.  

* Czym jest FOUC? Jak unikasz FOUC?  

Flash of unstyled content jest to wyświetlenie użytkownikowi nieostylowanej strony (jej zawartości) podczas ładowania strony. Pojawia się gdy CSS jest wolno ładowany lub gdy JS powoduje wielokrotne renderowanie strony.
Aby uniknąć FOUC należy serwować użytkownikowi jak najbardziej zoptymalizowany CSS (zminifikowany, w jednym pliku), oraz używać jak najmniej javascriptu powodującego fazę render przeglądarki. Używanie Critical CSS (czyli wrzucanie najważniejszych reguł css inline w znaczniku head).
Używanie media queries i serwowanie CSS zoptymalizowanego dla urządzeń o mniejszej rozdzielczości. Można też ukryć całą stronę do czasu załadowania wszystkich styli.  
https://en.wikipedia.org/wiki/Flash_of_unstyled_content  
http://www.techrepublic.com/blog/web-designer/how-to-prevent-flash-of-unstyled-content-on-your-websites/  
* Co to jest ARIA, screenreader i jak stworzyć stronę z ułatwieniami dostępu?
ARIA to zestaw wytycznych opracowanych przez WAI(Web Accessibility Initiative) aby umożliwić korzystanie z aplikacji ludziom z dysfunkcjami(np. niewidomi), którzy posługują się technologiami wspierającymi.

Screenreadery to programy służące do odczytywania treści i dostępnych akcji, które podejmuje się na komputerze.

3 kroki tworzenia aplikacji z ułatwieniami dostępu: używaj natywnych tagów HTML kiedy tylko się da; elementy interaktywne twórz z możliwością obsługi przez klawiaturę; zapewnij dodatkowe znaczniki specjalnie dla AT (accessibility technology). 
https://www.w3.org/WAI/intro/aria
http://gingertech.net/2012/02/14/a-systematic-approach-to-making-web-applications-accessible/

* Opowiedz o wadach i zaletach animacji w css i w JS.   
Minusy CSS w stosunku do JS:  
- skalowanie, rotacja, pozycja zostały wepchnięte do jednej właściwości transform, co uniemożliwia kontrolowanie skomplikowanych animacji  
- CSS chwali się za używanie pamięci GPU zamiast CPU do obsługi animacji, jednak używa jej tylko do transform i opacity a w JS można osiągnąć to samo za pomocą charakterystyk 3D  
- CSS teoretycznie korzysta z wielu wątków procesora, ale w rzeczywistości tylko dla elementów nie wpływających na flow dokumentu (transform, opacity - znikomy procent)  
- niemal w każdym środowisku animacje tworzone w JS (z wykorzystaniem GASP) są szybsze od tych tworzonych przez CSS  
- brak kontroli nad flow animacji - nie można przejść do jej konkretnego punktu, cofnąć jej, zmienić prędkości lub dodać callbacków w konkretnych punktach  
- przeglądarki starsze niż IE9 nie obsługują animacji CSS  

Plusy animacji CSS w stosunku do JS:  
- są szybsze od animacji jQuery  
- bardzo dobre do prostych przejść, np proste slidery, ofc również do efektów hover  

https://developers.google.com/web/fundamentals/design-and-ui/animations/css-vs-javascript  
https://css-tricks.com/myth-busting-css-animations-vs-javascript/  

### Pytania HTML:

* Co robi `doctype` i jakie znasz przykłady?  
służy do deklaracji typu dokumentu, i powinien być umieszczony jako pierwszy element w dokumencie HTML, w szczególności przed znacznikiem <html>. Ten znacznik informuje przeglądarkę której wersji HTML lub XHTML używa wczytywana właśnie strona. Przykłady:  

```
html 5: <!DOCTYPE html>
HTML 4.01 Strict <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
XHTML 1.0 Strict <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

* Jaka jest różnica między trybem full standards, almost standards a trybem dziwactw (quirks mode)?  
Quirks mode to renderowanie strony przez przeglądarkę w wersji dla navigatora 4 i IE 5, zaś full standards mode to renderowanie zgodne ze współczesnymi standardami html i css. Tryb almost standards posiada zaimplementowaną pewną niewielką ilość dziwactw navigatora i IE.  
https://developer.mozilla.org/pl/docs/Quirks_Mode_and_Standards_Mode  

* Jaka jest różnica między html a xhtml?  
XHTML to HTML napisany jako XML. Są niemal identyczne. Główne różnice to to, że xhtml jest bardziej restrykcyjny i dzięki temu obsługiwany przez wszystkie główne przeglądarki. Doctype jest obowiązkowy, podobnie atrybut xmlns w znaczniku html oraz znaczniki <html>, <head>, <title> i <body>. Elementy xhtmla musza być poprawnie zagnieżdżone, zawsze zamknięte, napisane małymi literami; zawsze muszą mieć jeden root element.  
https://www.w3schools.com/html/html_xhtml.asp  

* Jakie są ograniczenia w serwowaniu stron XHTML?  
Wbrew pozorom i założeniom największym problemem jest wsparcie przeglądarek. Większość z nich przekształca xhtml na zwykły html. Kod xhtml też niekoniecznie jest 'czystszy' od kodu html. Do tego trzeba pamiętać o następujących ograniczeniach:  
- wszystkie elementy muszą mieć początkowy znacznik  
- elementy non-void ze znacznikiem początkowym muszą mieć też znacznik końcowy  
- każdy element może sam się zamknąć przez '/>'  
- tagi i atrybuty są case sensitive  
- atrybuty musza być w cudzysłowiu  
- puste atrybuty są zabronione, więc checked zmienia się w checked="true"  
- znaki specjalne muszą być escapowane  

http://www.webdevout.net/articles/beware-of-xhtml#myths  

* Czy istnieją problemy z serwowaniem stron jako `application/xhtml+xml`?  
Kiedy browser dostaje xml, używa xml parsera. Niestety przeglądarki do IE8 włącznie nie obługują tego typu plików. Wiele plików xhtml jest więc serwowanych jako text/html. Wymusza to na deweloperach rozważanie pewnych różnic między tymi formatami podczas pisania kodu.
W ie8 dla tak serwowanej strony otwiera się dialog pobierania. Serwery proxy keszujące przy zapytaniu z takim content-type mogą zwrócić kod xml przeglądarce nie obsługującej tego typu. Przeglądarki wyświetlą błędy xml (jeśli jakieś będą) na stronie. 

http://stackoverflow.com/a/351908  
https://www.w3.org/International/articles/serving-xhtml/   

* Jak serwujesz stronę z treścią w wielu językach?  
Zawsze należy używać atrybutu language na tagu html do określenia domyślnego języka strony. Zawartość w innym języku należy otoczyć jakimś elementem do którego dodamy równiez atrybut language. Dla stron html należy używać atrybutu lang, zaś dla xhtml xml:lang. W html 1.x i w html 5 obu. 
https://www.w3.org/International/questions/qa-html-language-declarations  

* O czym trzeba pamiętać tworząc strony wielojęzykowe?
Należy rozważyć jak userzy będą przekierowywani na odpowiednią wersję językową strony. Należy również pamiętać o sprawach takich jak: tekst w obrazkach się nie przetłumaczy ani nie przeskaluje, kolory mogą być inaczej postrzegane przez ludzi z innych kultur, nie powinno się wpisywać w ogóle tekstu do szablonów strony (tekst powinien być dynamicznie renderowany), formaty dat mogą się różnić, należy pamiętać o stylowaniu czcionek przez selector css :lang, słowa w różnych językach będą miały różną długość.  
https://www.quora.com/What-kind-of-things-one-should-be-wary-of-when-designing-or-developing-for-multilingual-sites  

* Jaka jest przydatność atrybutów `data-`
* Rozpatrujemy HTML5 jako otwartą platformę internetową. Jakie składniki tworzą HTML5?  
Główne składniki takiej platformy internetowej to html 5, css3, js i svg. Html 5 służy do definiowania kształtu dokumentu (tytułów, nagłówków, tabel itp), css do nadawania mu stylu, js do tworzenia skryptów i svg do tworzenia skalowalnych grafik wektorowych.  
http://yucianga.info/?p=655  

* Opisz różnice między cookies, sessionStorage i localStorage.  
cookie:
maksymalny rozmiar to 4093B, może mieć datę ważności, wysyłane przy każdym requeście  
sessionStorage:
maksymalny rozmiar 2,5MB+ w zależności od przeglądarki, przechowywanie danych w przeglądarce bez wysyłania ich przy requestach, przy zamknięciu karty lub przeglądarki session storage jest czyszczony  
localStorage: tak jak sessionStorage ale jest zachowywane nawet po zamknięciu przeglądarki  
http://stackoverflow.com/a/19869560  

* Opisz różnice między `<script>`, `<script async>` i `<script defer>`.  
Zachowanie przeglądarki napotykającej:  
- script tag: Zatrzymuje parsowanie dokumentu. Wykonuje request po plik skryptu. Wykonuje skrypt po ściągnięciu go. Kontynuuje parsowanie dokumentu.  
- script tag z async: Wykonuje równoległe requesty po każdy napotkany skrypt. Kontynuuje parsowanie dokumentu jakby nic nie przerwało tego procesu. Kiedy którykolwiek skrypt zostanie ściągnięty, wykonuje go.  
- script tag z defer: Wykonuje równoległe requesty po każdy napotkany skrypt. Kontynuuje parsowanie dokumentu jakby nic nie przerwało tego procesu. Parsuje dokument do końca, nawet jeśli jakiś skrypt się ściągnął. Następnie wykonuje skrypty w kolejności, w jakiej zostały napotkane w dokumencie.  
http://javascript.tutorialhorizon.com/2015/08/11/script-async-defer-attribute/  

* Dlaczego dobrą praktyką jest umieszczanie cssów (<link>) w headerze i skryptów JS (<script>) tuż przed znacznikiem </body>? Czy znasz jakieś wyjątki?
Umieszczanie cssów w headerze pozwala uniknąć FOUC. Umieszczanie script tagów pod koniec body ma sens dla starych przeglądarek, które ładując skrypty przestawały renderować stronę. Dla dużych stron był to jednak problem, ponieważ ściąganie skryptów nie mogło się rozpocząć dopóki wszystkie pozostałe elementy nie zostały załadowane.  
Obecnie przeglądarki obsługują script tagi defer i async, istnieje również speculative parsing, więc współczesnym podejściem jest po prostu zasotowanie atrybutu defer na tagu script.  
http://stackoverflow.com/a/24070373  

* Czym jest renderowanie progresywne?  
Są to techniki renderowania treści do wyświetlenia tak szybko, jak to możliwe. Przykład: opóźnione ładowanie obrazków, gdzie skrypt js ładuje obrazek dopiero gdy znajdzie się w viewporcie przeglądarki, zamiast ładować wszystkie - również niewidoczne - obrazki podczas startu strony.  
http://stackoverflow.com/a/33651444  

* Czy używałeś różnych HTML templating languages?  
Nie, ale jestem zaznajomiony z: Jade, EJS, HandlebarsJs, Underscore Templates, Mustache  

### Pytania JS:

* Wyjaśnij delegację zdarzeń.
    Delegacja zdarzeń / eventów polega na przypięciu obsługi zdarzenia (event handler) do elementu nadrzędnego, zamiast do elementu który chcemy obsłużyć. Po kliknięciu na element wewnętrzny, event bubbles up (bąbluje do góry) dochodząc do elementu z przypisanym handlerem. Następnie za pomocą event.target możemy sprawdzić gdzie zdarzył się event i wykonać go na odpowiednim elemencie.
    Dzięki temu możemy obsłużyć zdarzenia występujące na wielu elementach, za pomocą jednego handlera.

    http://www.crimsteam.site90.net/crimsteam/dom/dom_zdarzenia_delegacja.html
    https://davidwalsh.name/event-delegate
    
* Wyjaśnij jak działa `this` w JavaScripcie.
  `this` wskazuje na jakiś obiekt w zależności od kontekstu,
  w jakim została użyta funkcja, w której go zdefiniowaliśmy.
  Kontekstu czyli sposobu i miejsca wywołania.

  Kontekst globalny:
  console.log(this === window); // true
  this.a = 37;
  console.log(window.a); // 37
  Jako metoda obiektu:
  var o = {  prop: 37, f: function() { return this.prop; }};
  console.log(o.f()); // logs 37

  https://developer.mozilla.org/pl/docs/Web/JavaScript/Referencje/Operatory/this
  http://stackoverflow.com/questions/3127429/how-does-the-this-keyword-work

* Wyjaśnij jak działa dziedziczenie prototypowe.
* Jak radzisz sobie z testowaniem swojego kodu JavaScript?
* AMD kontra CommonJS?

Obie specyfikacje opisują format i sposób w jaki moduły i ich zależności powinnybyć definiowane;
Głowną rożnicą pomiędzy AMD(Asynchronous Module Definition) a CommonJS est asynchroniczne ładowanie modułow w AMD.

AMD:
 - używane jest w przeglądarkach, umożliwia asynchroniczne ładowanie modułów
 - define('module', [dependencies], function module() { return contents });
CommonJS:
 - na backendzie - dawniej często używana w NodeJS, obecnie się od niej odchodzi.
 - exports / module.exports | require

 https://auth0.com/blog/javascript-module-systems-showdown/
 
* Jakie znasz patterny w javascripcie? 

- Strażnik (Guard Pattern)

W programowaniu strażnik jest wyrażeniem typu boolean, które musi zwrócić true jeśli program ma kontynuować swoje wykonanie. Bez względu na język programowania, kod ochrony lub klauzula ochronna jest sprawdzeniem warunków, które pozwolą uniknięcia błędów podczas dalszego wykonywania programu.


- Konstruktor
Konstruktory obiektów używane są do tworzenia określonych typów obiektów - przygotowują obiekty do użycia oraz przyjmują argumenty, które konstruktor może wykorzystać do ustawiania wartości właściwości i metod obiektu, kiedy ten tworzony jest po raz pierwszy.

- Moduł
W JavaScript wzorzec modułu używany jest do głębszej emulacji klas, w taki sposób, że możemy tworzyć zarówno publiczne jak i prywatne metody i zmienne wewnątrz obiektu, jednocześnie ukrywając poszczególne jego części przed global scope. Wynikiem tego jest mniejsze ryzyko konfliktu nazw funkcji stworzonych w module z funkcjami stworzonymi przez inne skrypty w aplikacji.

- Singleton
Wzorzec singletonu ma w założeniu zapewnić tylko jedną instancję danej klasy. Oznacza to, że próba utworzenia obiektu danej klasy po raz drugi powinna zwrócić dokładnie ten sam obiekt, który został zwrócony za pierwszym razem. Jako, że w JS nie istnieją klasy, możemy mówić tylkoo instancjach obiektów. W JS istnieje kilka sposobów uzyskania singletonu:

  - Wykorzystanie zmiennej globalnej do zapamitania instancji.
  - Wykorzystanie właściwości statycznej konstruktora. Funkcje w jzyku JavaScript są obiektami, więc mają właściwości. Można utowrzyć właściwość "Object".instance i to w niej przechowywać obiekt.
  - Zamknicie instancji w domkniciu. W ten sposób instancja staje si elementem prywatnym i nie może zostać zmieniona z zewnątrz.

- Obserwator
Wzorzec obserwatora jest niezwykle czsto wykorzystywany w programowaniu po stronie klienta w jzyku JavaScript.
Głównym celem użwania wzorca jest promowanie luźnego powiązania elementów. Zamiast sytuacji, w której jeden obiekt wywołuje metod drugiego, mamy sytuacj, w której drugi z obiektów zgłasza chęć otrzymywania powiadomień o zmianie w pierwszym obiekcie. Subskrybenta
nazywa si czsto obserwatorem, a obiekt obserwowany obiektem publikującym lub źródłem. Obiekt publikujący wywołuje subskrybentów po zajściu istotnego zdarzenia i bardzo często przekazuje informację o nim w postaci obiektu zdarzenia.

  Uczestnicy

  - Subject:
    - zarząda lista observerów
    - implementuje interfejs pozwalający observerom subskrybować i usuwać subskrypcję dla danego zdarzenia
    - wysyła powiadomienie do swoich subskrybentów, gdy jego stan się zmieni
  - Observers - posiadają sygnaturę funkcji, która może zostać wykonana, gdy zmieni się Subject

- Strategia
Wzorzec strategii umożliwa wybór odpowiedniego algorytmu na etapie działania aplikacji. Użytkownicy kodu mogą stosować ten sam interfejs zewntrzny, ale wybierać spośród kilku dostpnych algorytmów, by lepiej dopasować implementacj do aktualnego kontekstu.

  Uczestnicy: 

  - Context:
    - przechowuje referencję do obecnego obiektu Strategii
    - posiada interfejs dzięki któremu klienci mogą zarządać wykonania konkretnej strategii
    - pozwala klientowi na zmianę strategii
  - Strategy - implementuje algorytmy używając interfejsu Strategii

DotFactory patterns![DotFactory patterns](http://www.dofactory.com/javascript/design-patterns)
JavaScript Design Patterns![JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/)

* Czym jest tablica mieszająca (hashtable)?
* Co oznaczają komunikaty `undefined` i `undeclared` dla zmiennych?
* Co oznaczają komunikaty `null`, `undefined` i `undeclared` dla zmiennych?
  - Undeclared jest to zmienna, która nie została stworzona za pomocą var/let/const, a więc została stworzona na obiekcie globalnym window/global.
  - Undefined jest to zmienna, która została zadeklarowana, ale nie została do niej przypisana żadna wartość
  - Null jest to typ, który ma przypisaną tylko jedną wartość null, zmienna została zadeklrowana i przypisny do niej obiekt typu Null
  - Undefined jest typem, null jest obiektem
  * Jak byś sprawdził te stany zmiennych?
    - typeof undefined === 'undefined'
    - typeof null === 'object';
  https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof

* Czym jest promise?

Promise (natywnie dodany w ES6) jest obiektem używanym w operacjach asynchronicznych. Jest to obiekt, który reprezentuje wartość, która może być dostępna teraz, w przyszłości, lub nie być dostępna wcale.
Promise ma trzy stany: pending (rozpoczęte), fullfiled (zakończone pozytywnie), rejected (zakończone niepowodzeniem - błędem). Gdy Promise osiągnie stan fullfiled lub rejected uruchamiane są handlery poprzez .then (.catch jest aliasem do .then(undefined, function()))

Promise![Promise](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Promise)

* Czym są domknięcia, jak i po co są używane?
    Closure - domknięcie - pozwala na dostęp do wewnętrznego scope funkcji, nawet po jej wykonaniu.
    Osiąga się to poprzez zwrócenie funkcji po wywołaniu funkcji nadrzędnej.
    Pozwala to na symulowanie zmiennych publicznych i prywatnych.
  * Ulubiony wzorzec używany do ich tworzenia?
    - Module pattern
  http://blog.nebula.us/13-javascript-closures-czyli-zrozumiec-i-wykorzystac-domkniecia

* Jakie znasz typowe użycie funkcji anonimowych?
  - Callbacks
  - IIFE's
  - Closures

* Wyjaśnij pojęcie "Moduł JavaScript" i kiedy jest warte stosowania.
  * Dodatkowe punkty za wzmiankę na temat czystości przestrzeni nazw.
  * Co jeśli Twój kod nie używa przestrzeni nazw?
* Jak organizujesz swój kod? (moduły, klasyczne dziedziczenie?)
  Np. Używam module pattern, IIFE, Atomic design

* Jaka jest różnica między obiektami typu `host` i `native`?
  Host objects są to obiekty dostarczane przez środowisko hosta. Mogą się one różnić pomędzy środowiskami, przykłady:
  - window, document, location
  Native objects są to obiecty opisane i w pełni zdefiniowane w specyfikacji ECMAScript, przykłady:
  - Date, Math, parseInt.
  http://stackoverflow.com/questions/7614317/what-is-the-difference-between-native-objects-and-host-objects

* Różnica między:
```javascript
function Person(){}, var person = Person(), var person = new Person()
```
  - Jest to deklaracja funkcji, przypisuje nazwę do funkcji bez konieczności przypisywania jej do zmiennej
  - Przypisuje do zmiennej person wartość zwracaną przez funkcję person, w tym przypadku undefined
  - Przypisuje do zmiennej person obiekt/konstruktor typu Person, z this przypisanym do obiektu Person
  https://javascriptweblog.wordpress.com/2010/07/06/function-declarations-vs-function-expressions/

* Jaka jest różnica między `.call` i `.apply`?
  Za pomocą `.call` i `.apply` można przypisać inny obiekt podczas wywoływania istniejącą funkcji.
  `this` odnosi się do bieżącego obiektu, obiektu wywołującego.
  Dzięki czemu można napisać metodę raz, a następnie dziedziczyć ją w innym obiekcie, bez konieczności przepisywania metody dla nowego obiektu.
  Call przymuje wartość `this` i pojednyńcze argumenty, natomiast apply w postaci tablicy.
  theFunction.apply(valueForThis, arrayOfArgs)
  theFunction.call(valueForThis, arg1, arg2, ...)
  http://stackoverflow.com/questions/1986896/what-is-the-difference-between-call-and-apply
  https://developer.mozilla.org/pl/docs/Web/JavaScript/Referencje/Obiekty/Function/apply
  https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Function/call

* Wyjaśnij `Function.prototype.bind`?
    Bind tworzy nową funkcję pozwalającą przypisać `this` do kontekstu jaki chcemy, ponieważ w funkcji zwrotnej
    wartość obiektu bieżącego `this` może nie być tym, czego się spodziewamy.
    Pozwala on także przypisać domyślne argumenty dla zwracanej funkcji:
      var Person = function (name) { this.name = name; };
      Person.prototype.speak = function (volume) {return this.name +  volume };
      var person = new Person("John");
      var f = person.speak.bind(person, "loudly");
      // "John loudly"
      http://www.kurshtml.edu.pl/js/bind,function-prototype.html

* Czym jest callback?
Callback jest to funckcja przekazywana do innej funkcji poprzez argument. Funkcja, która przyjmuje callback jako argument może w swoim ciele wywołać przekazaną funkcję. Wywołanie to może nastąpić natychmiast (synchronicznie), albo późniejszym czasie (asynchronicznie).

Callback![Callback](https://en.wikipedia.org/wiki/Callback_(computer_programming))

* Kiedy optymalizujesz swój kod?

* Czy w jsie mamy metody prywatne?

Tak, w JS można tworzyć zmienne i metody jako prywatne. Aby stworzyć metodę prywatną należy utworzyć definicję funkcji w konstruktorze obiektu (bez przypisania jej do this). W takim wypadku funkcja / metoda będzie dostępna tylko wewnątz obiektu i tylko dla funkcji prytwatnych.

Private members![Crockford on private members](http://javascript.crockford.com/private.html)

* Wyjaśnij działanie dziedziczenia w JavaScript?
* Co to jest function declaration a co function expression i czym sie roznia?

Function declaration jest to stworzenie obiektu typu Function i przypisanie mu nazwy oraz parametrów używanych przez funkcję.
Function expression jest niemal identyczne, natomiast pozwala na ominięcie nazwy funkcji (co tworzy tzw. funkcję anonimową). Function expression może być także używane jako IIFE. Function expression, w przeciwieństwie do function declaration nie są hoistowane.

Function delcaration![Function delcaration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)
Function expression![Function expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/function)
Function declaration vs function expression![Function declaration vs function expression](https://www.sitepoint.com/function-expressions-vs-declarations/)

* Kiedy użyłbyś `document.write()`?
    Document.write() jest zawsze dostępny, jest dobrym wyborem dla dostawcow skryptow zewnetrznych aby mogli dodać oni swoj kod.
    Wiele generowanych reklam używa `document.write()` choć nie jest to mile widziane.

* Jakie są różnice między wykrywaniem obsługi funkcji, wnioskowaniem obsługi funkcji i używaniem ciągu UA?
    Feauture detection(wykrywaniem obsługi funkcji) jest to wykrywanie, czy dany feature / właściwość / funkcjonalność /  jest dostępny w środowisku wykonywalnym
    np: return !!document.createElement('canvas').getContext; // return true or false

    Feauture inference (wnioskowanie obsługi funkcji) polega na założeniu, że jeśli dana funkcjonalność jest dostępna w danej wersji przeglądarki, to cała reszta funkcjonalności także. Używa się ich wtedy bez sprawdzania czy istnieją, co może prowadzić do błędów.

    UA string czyli User Agent string domyślnie zwraca wersję przeglądarki jaka wykonuje zapytanie, jaka uruchamia danych skrypt js. UA string może być zmieniany przez klienta.

    http://lucybain.com/blog/2014/feature-detection-vs-inference/

* Co to sa falsy values?

Falsy values są to wartości, które podczas konwersji na boolean dają wartość false. Są to:

- 0
- "" - pusty string
- null
- undefined
- NaN
- false 

Falsy values![MDN falsy values](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)

* Omów AJAX jak najbardziej szczegółowo.
* Podaj wady i zalety żywania technologii AJAX
  Zalety:
    - Ciągłe i niewidoczne dla użytkownika uaktualnianie danych
    - Brak konieczności odświeżania całej strony

  Wady:
    - Nie działa, gdy wyłączona jest obsługa JavaScript w przeglądarce
    - Strona nie jest odświeżana a więc nie można cofnąć lub powtórzyć kroków za pomocą przycisków w przeglądarce
    - Opóźnienia, gdy serwer jest mocno obciążony
    - Dane są ładowane dynamicznie a więc nie są częścią strony WWW. Wyszukiwarki internetowe nie indeksują treści ładowanych dynamicznie

* Wyjaśnij działanie JSONP (i dlaczego nie jest właściwie AJAX).
    JavaScript Object Notation with Padding - zdalny AJAX spoza domeny.
    Pozwala na pobieranie danych z serwerów znajdujących się w innej domenie,
    niż domena w której uruchamiany jest skrypt.js. Pomaga ominąć Same-origin policy.
    JSONP umożliwa pobieranie danych JSON poprzez opakowanie danych w funkcję JS,
    co umożliwia uruchomienie zewnętrznego skryptu js poprzez dodanie go za pomocą tagu script.
    W celu uruchomienia funkcji zwracającej JSON musimy w urlu podać callback taki sam jak funkcja opakowująca JSON.
    - `http://www.example.net/sample.aspx?callback=mycallback`
    - można używać tylko z zapytaniami GET

    http://stackoverflow.com/questions/2067472/what-is-jsonp-all-about

* Typy zmiennych w jsie?
 
W JS rozróżniamy dwa typy danych: typy proste i typy złożone.

Do typów prostych należą:
- String
- Number
- Boolean
- null
- undefined
- Symbol (od ES6)

Typem złożonym jest Object jak np:
- Array
- Date
- Function
- Map, WeakMap
- Set, WeakSet

Typy proste przekazywane są przez wartość, natomiast typy złożone przez referencję.
 
Javascript Types![Javascript Data Types](https://developer.mozilla.org/pl/docs/Web/JavaScript/Data_structures)

* Czy kiedykolwiek używałeś szablonów w JavaScript?
  * Jeśli tak, jakie to były biblioteki? (Mustache.js, Handlebars itd.)
    Używałem jedynie Handlebars do prostych skryptów wymagających wypełniania dużej ilości danych w pętli.
    Popularne szablony:
    - Mustache
    - Underscore
    - Embedded JS

* Co robi drugi parametr object.create?

Drugi parametr Object.create pozwala na dodanie właściwości do nowo powstałego obiektu. Format w jakim podajemy te właściwości jest taki sam jak w drugim argumencie Object.defineProperties().

Object.create![Object.create](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Object/create)

* Wyjaśnij pojęcie "hoisting".
* Zasieg zmiennych w jsie?

 W JS, do wersji ES6 występowały tylko dwa rodzaje zasięgu zmiennych, tj. globalny (global scope) i zasięg lokalny - w obrębie funkcji (function scope).
 Od ES6 i pojawienia się zmiennych deklarowanych jako let i const pojawił się także zasięg blokowy (tj. wewnątrz { }).

var![var](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var)
let![let](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Statements/let)
const![const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)
Other scopes![other scopes](http://stackoverflow.com/a/500459)

* Opisz bąbelkowanie zdarzeń.
    Bubbling jest to wynoszenie / przechodzenie eventu do góry drzewa DOM.
    Jeśli mamy jakiś event w wewnętrznym elemencie i oba mają zarejestrowany event,
    bąbelkowanie najpierw wykona się w najbardziej zagnieżdonym miejscu. Następnie
    będzie przenosić się wyżej i uruchamiać kolejne eventy.

    http://stackoverflow.com/questions/4616694/what-is-event-bubbling-and-capturing

* Jak jest różnica między "atrybutem" i "właściwością"?
    Atrybut jest to wartość w samym HTML, która jest zawsze stringiem
    Property jest przypisana do obiektu w drzewie DOM, może mieć różne typy jak String czy boolean

    http://lucybain.com/blog/2014/attribute-vs-property/

* W jaki sposob mozemy realizowac dziedziczenie w javascripcie (new + Object.create)?

- Używając konstruktora

W JS konstruktor jest po prostu dowolną funkcją, którą jest wykonywana za pomocą operatora new.
W konstruktorach, nowo stworzona funkcja dziedziczy bezpośrednio z prototypu konstruktora.
Przy wykonaniu new Funcition(), zadeklarowane właściwości / funkcje wewnątrz konstruktora nie tworzą prototypu.

- Używając Object.create

Object.create zostało dodane w ECMAScript 5. Object.create tworzy nowy obiekt, który dziedziczy bezpośrednio z obiektu podanego jako pierwszy argument wywołania funkcji. Object.create nie uruchamia konstruktora.

- Za pomocą class

W ECMAScript 2015 przedstawiono nowe słowa kluczowe implementujące klasy. Mogą one wyglądać identycznie do konstrukcji znanych z języków implementujących klasyczny model dziedziczenia, jednak nie są one tym samym. Dziedziczenie w JavaScript nadal pozostało prototypowe. Klasy są tak naprawdę tylko "lukrem składniowym" na tworzenie obiektu za pomocą konstruktora i new.

Difference new vs Object.create![Difference new vs Object.create](http://stackoverflow.com/questions/4166616/understanding-the-difference-between-object-create-and-new-somefunction)

* Czemu rozszerzanie obiektów wbudowanych w JavaScript jest złym pomysłem?
    Ponieważ obiekty te zostały stworzone według pewnej dobrze udokumentowanej i przemyślanej specyfikacji
    Jeśli dodamy swoje metody do wbudowanego obiektu, mogą one zostać nadpisane
    przez nieświadomego developera używającego naszego kodu,
    twórcy przeglądarki mogą zaimplementować metodę o takiej samej nazwie,
    użytkownik nie będzie wiedział której używa itp.

* Czy rozszerzanie obiektów wbudowanych ma dobre strony?
    Można wykorzystać możliwości normalnie niedostępne dla danej metody.
    Np. odwrocenie stringa z wykorzystaniem metody `reverse` z Array.
    String.prototype.reverse = function() {
      return Array.prototype.reverse.apply(this.split('')).join('');
    };
    https://code.tutsplus.com/tutorials/quick-tip-how-to-extend-built-in-objects-in-javascript--net-9168
    
* Jak jest różnicą między zdarzeniami `document load` i `DOMContentLoaded` dla strony internetowej?
    Event DOMContentLoaded jest uruchamiany, gdy HTML został załadowany i drzewo DOM zbudowane
    natomiast event load, gdy cała strona, włącznie z css, grafiką zostały załadowane.
    http://stackoverflow.com/questions/2414750/difference-between-domcontentloaded-and-load-events

* Jaka jest różnica między `==` i `===`?
    `==` porównuje wartości, dokonując koercji jeśli typy zmiennych nie są jednakowe
    `===` porównuje wartości jak i typy zmiennych, nie dokonując koercji

* Wyjaśnij ewentualny sposób pobrania parametrów z adresu URL w oknie przeglądarki.
* Wyjaśnij politykę `same-origin` w odniesieniu do JavaScript.
    Jest to fundamentalny mechanizm bezpieczeństwa przeglądarki. Mechanizm ten zapobiega dostępowi
    skryptów js do drzew DOM różnego pochodzenia.
    Same origin zachodzi wtedy, gdy zgodne są protokół port i host stron, z których wywoływane są skrypty.

* Opisz wzorce dziedziczenia w JavaScript.
  - Pseudoclassical pattern - instancje konstruktora/klas tworzone są przez `new`,
    dziedziczące wszystkie metody i właściwości rodzica. Tworząc instancję poprzez `new`
    bindujemy ją do `this`. Metody klasy odnoszą się do `this` instancji.
  - Functional pattern - zawiera wszyskie metody i właściwości wewnątrz funkcji konstruktora.
  - Prototypal pattern - rozszerza klasę/konstruktor o kolejne subklasy dziedziczące wszystkie metody i właściwości rodzica.

  http://wes.is/2014/12/14/why-i-prefer-the-pseudoclassical-pattern-for-creating-classes-in-javascript-and-why-you-should-too/

* Czy funkcje sa hoistowane?
    W JS funcje można deklarować na dwa sposoby: poprzez function definition oraz function expression.
    Function definition są hoistowane, natomiast function expressions nie.
    Function hoisting![Function hoisting](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)

* Napisz działający kod:
```javascript
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```

```javascript
function duplicate(arr) {
  return arr.concat(arr);
}
```
Odniesienie: [Array.prototype.concat](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/concat)

* Opisz strategię zapamiętywania (unikanie powtarzalnych obliczeń) w JavaScript.
* Dlaczego mówimy wyrażenie trójkowe, co dokładnie oznacza słowo "trójkowy"?

Mówimy wyrażenie trójkowe, ponieważ przyjmuje trzy operandy (operand - argument).
Jako ciekawostke można dodać, że jest to jedyny operator w JavaScripcie, który przyjmuje trzy operandy.
Odniesienie: [Conditional (ternary) Operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)

* Czym jest `arity` funkcji?
* Co to jest `callback`?

Callback to funkcja, ktora przekazujemy do innej funkcji jako argument. Funkcja, która otrzymuje callback jako argument może go wywołac w swoim ciele. To wykonanie może być natychmiastowe w synchronicznym wywołaniu zwrotnym lub może zostać wykonane po czasie w sposób asynchroniczny. 

[Callback](https://en.wikipedia.org/wiki/Callback_(computer_programming))

* Czemu, na ogół, dobrym pomysłem jest nie ruszanie globalnej przestrzeni strony?

Generalnie nie deklarowanie zmiennych globalnych jest zalecane, ponieważ cały kod posiada jedną przestrzen nazw.
Zbyt duża ilość zmiennych globalnych może skutkować konfliktem pomiędzy różnymi skryptami na stronie.
Najlepszym rozwiązaniem, aby uniknąć zanieczyszczania globalnej przestrzeni jest użycie IIFE.

Odniesienie: [Global variables disscusion](http://stackoverflow.com/questions/2613310/ive-heard-global-variables-are-bad-what-alternative-solution-should-i-use)

* Co oznacza `"use strict";`? Jakie są zalety i wady takiego rozwiązania?

  "use strict" włącza bardziej restrykcyjną wersje JavaScriptu.
  Kod jest inaczej odczytywany przez silnik w niektórych przypadkach.

  Zalety:
    - Eliminuje niektóre ciche błędy, a zamiast nich wyrzuca błąd.
    - Naprawia niektóre pomyłki, które sprawiają, że JavaScriptowe silniki mają trudność z optymalizacją kodu (wersja kodu w strict mode może być szybsza niż normalna).
    - Rezerwuje składnię, która prawdopodobnie będzie użyta w przyszłych wersjach ECMAScript.

  Wady:
    - Przeglądarki, które nie wspierają strict mode'u będą wykonywać kod zgodnie z normalnymi standardami.
  
  Odniesienie: [Strict mode](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode)

* Czym rozni sie dziedziczenie w jsie od klasycznego dziedziczenia?
 
 Podmiotem dziedziczenia klasycznego, są klasy natomiast w js dziedziczenie (zwane prototypowym) odbywa się bezpośrednio na obiektach.
 Konsekwencją tego, że w dziedziczeniu klasycznym hierarchia tworzona jest za pomocą klas, które są jakby opisem przyszłego obiektu, co uniemożliwia zmiany metod, które są dziedziczone. Nie dzidziczy się również stanu (gdyż klasy go nie posiadają).
 W dziedziczeniu prototypowym, opartym na obiektach, każda zmiana metody czy atrybutu na obiektach, z których się dziedziczy, jest natychmiast odzwierciedlana na obiekcie dziedziczącym. Dziedziczy się także stan obiektu.
 
Classical vs Prototypal![Stackoverflow - classical vs prototypal](http://softwareengineering.stackexchange.com/a/99438)

* Jaka jest roznica miedzy funkcja a obiektem?

Tak naprawdę funkcja jest specyficznym typem obiektu w JavaScript, posiadającym wszystkie właściwości normalnego obiektu. Jedyną różnicą, między funkcją a zwykłym obiektem, jest możliwość wywołania funkcji, co jest możliwe dzięki wewnętrznej metodzie [[Call]], którą posiadają tylko funkcje.
Prototypem funkcji jest Object, konstruktorem funkcji jest Function();

* Po co uzyłbyś czegoś takiego jak zdarzenie `load`? Czy posiada ono jakieś wady? Czy znasz jakieś alternatywy, i jeżeli tak to czemu użyłbyś ich?

Zdarzenie `load` jest wywolane, gdy strona została w całości załadowana.
Jedną z wad jest to, że zdarzenie `load` czeka na całą zawartość strony - nawet arkusze stylów i obrazki.
Najbardziej polecaną alternatywą jest zdarzenie `DOMContentLoaded`, które zostaje wywołane, gdy podstawowy HTML dokumnetu został kompletnie załadowany i sparsowany.

Odniesienia: [Load](https://developer.mozilla.org/en-US/docs/Web/Events/load), [DOMContentLoaded](https://developer.mozilla.org/en-US/docs/Web/Events/DOMContentLoaded)

* Wytlumacz czym jest single-page application i jak można sprawić, by była ona bardziej przyjazna dla SEO.

Single-page application (SPA) to aplikacja internetowa lub strona, która mieści się na jednej stronie internetowej w celu dostarczenia jak najlepszych doznan, porównywalnych do tych odczuwalnych w desktopowych aplikacjach. W SPA, albo cały kod - HTML, JavaScript i CSS - jest pobierany przy załadowaniu strony, albo jest dynamicznie doładowywany i dodawany do strony w razie zapotrzebowania. Single-page application nigdy nie się nie przeładowywuje w trakcie używania, chociaż `location hash` i `HTML5 History API` może zostać użyte, aby wprowadzić uczucie nawigacji po osobnych stronach w aplikacji.
Stronę można uczynić przyjazną dla SEO poprzez server-side rendering i używanie semantycznych znaczników HTML5.

[Single-page application](https://en.wikipedia.org/wiki/Single-page_application)

* Wytlumacz różnicę pomiędzy zmiennymi i niezmiennymi obiektami.
  * Jaki jest przykład niezmienialnego obiektu w JavaScripcie?
  * Jakie są wady i zalety niezmienności?
  * Jak możesz osiągnąć niezmienność w Twoim kodzie?

Zmienny obiekt może zostać zmieniony.
Niezmienny obiekt nie może zostać zmieniony. Przy każdej zmianie zostaje zwrócony nowy obiekt.

Zalety:
 - Mniej skomplikowany w użyciu.
 - Operacje mogą być łączone.
 - Może być łatwo skopiowany.
 - Nigdy nie zmienia swojego stanu.
 - Łatwo można go przekazywać.
 - Łatwe debugowanie.

Wady:
  - Większe zużycie pamięci.
  - Ciężki do zbudowania.

Można osiągnąć niezmienność obiektu poprzez użycie Object.freeze lub Object.seal.
Można również użyć bibliotek np. Immutable.js.

Odniesienie: [Dyskusja na Quora](https://www.quora.com/What-are-the-advantages-and-disadvantages-of-immutable-data-structures),
[Dyskusja na Stackoverflow](http://stackoverflow.com/questions/1863515/pros-cons-of-immutability-vs-mutability)

* Jakie sa wady i zalety używania obietnic zamiast callbacków?

Zalety:
  - Unikanie "callback hell".
  - Wieksze mozliwosci.
  - Bogaty interfejs.
  - Obsługa błędów.

Wady:
  - Środowisko musi wspierać obietnice.
  - Kod jest bardziej skomplikowany.

* Jak bardzo jesteś zaznajomiony z `Promises` i/czy ich polyfillami?

Używam `Promises` od pewnego czasu, prawdopodobnie coś około połowy roku.
Dzięki `Promises` mój asynchroniczny kod wygląda o wiele lepiej i przestałem utykać w tzw. "callback hell".
Jedyny polyfill, który znam to `Bluebird`.

* Czym jest dziedziczenie?
 
Dziedziczenie jest mechanizmem współdzielenia funkcjonalności między klasami i/lub obiektami (w rozumieniu klasycznym) lub obiektami (w dziedziczeniu prototypowym - jak w js). Klasa dziedzicząca (zwana klasą pochodną) otrzymuje dostęp do udostępnionych zachowń oraz atrybutów od klasy, z której następuje dziedziczenie (zwanej klasą bazową).
 
Dziedziczenie![Wikipedia - dziedziczenie](https://pl.wikipedia.org/wiki/Dziedziczenie_(programowanie))

* Czym jest obietnica (`Promise`)?

Obietnica jest używana do asynchronicznych operacji. Reprezentuje wartość, która może być dostępna teraz, w przyszłości albo nigdy.
Może posiadać jeden z trzech stanów:

- oczekujacy: stan początkowy, nie jest ani spełniona ani odrzucona.
- spełniony: operacja przebiegła pomyślnie.
- odrzucony: operacja się nie powiodła.

Oczekująca obietnica może być spełniona z jakąś wartością lub odrzucona z jakimś powodem (błędem). Gdy tak się stanie, przypisane funkcje w metodzie then zostaną wykonane.

[Promise](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Promise)

* Jakich narzędzi i technik używasz do debugowania kodu JavaScript?

Używam DevTools z Chrome.
Używam następujących technik:
  - Przerywanie wykonywania kodu przy zmianie wybranego elementu DOM.
  - Breakpointy przy wysyłaniu żądan.
  - Przerywanie wykonywania kodu przy wyjątku.
  - Sprawdzanie optymalizacji kodu przy pomocy Audits (zakładka w DevTools).

Odniesienie: [Wskazówki](http://www.zsoltnagy.eu/javascript-debugging-tips-and-tricks/)

* Zasieg zmiennych w JavaScript?

W JavaScripcie, przed wersją ES6, były tylko dwa zakresy zmiennych. Zakres globalny oraz lokalny - funkcja.
W ES6 jest jeszcze jeden zakres - zasięg blokowy, który dotyczy zmiennych zadeklarowanych przy użyciu let i const (zasięg w {}).

[var](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var)
[let](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Statements/let)
[const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)
[inne](http://stackoverflow.com/a/500459)

* Jakich konstrukcji językowych używasz do iterowania po obiekcie i tablicy? 

Do iterowania po obiekcie używam pętli for...in z sprawdzaniem właściwości za pomocą hasOwnProperty.
Do iterowania po tablicy używam pętli for i metod Array.prototype, takich jak .forEach lub .map.

Odniesienie: [hasOwnProperty](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty),
[Array.prototype](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype)

* Wytłumacz różnice pomiędzy synchronicznymi i asynchronicznymi funkcjami.

Synchroniczna funkcja zostanie wykonana i kiedy się zakonczy, następne zadanie zostanie wykonane.
Asynchroniczna funkcja zostanie wykonana i niezależnie od tego czy się zakonczy czy nie, następne zadanie zostanie wykonane.

Odniesienie: [Asynchronicznosc vs synchronicznosc](http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean)

* Czym jest event life cycle (event flow)?

Event lifecycle (event flow) opisuje cykl życia eventu w drzewie DOM. Przy każdym zdarzeniu, przeglądarka tworzy event i rozsyła go po drzewie DOM. Propagacja / rozsyłanie eventu odbywa się w trzech fazach:

- capturing faze - w tej fazie event przesyłany jest od najwyżeszego rodzica w drzewie DOM, aż do elementu, na którym nastąpiło zdarzenie.
- on the object faze - występuje na elemencie, na którym nastąpiło zdarzenie
- bubbling faze - w tej fazie event przesyłany jest od elementu na którym nastąpiło zdarzenie, aż do najwyżeszego rodzica w drzewie dom

Event flow![Event Life Cycle](http://www.quirksmode.org/js/events_order.html)

### Przykłady kodu JS:

```javascript
~~3.14
```
Pytanie: Jaka wartość zostanie zwrócona przez powyższe wyrażenie?
**Odpowiedź: 3**

```javascript
"i'm a lasagna hog".split("").reverse().join("");
```
Pytanie: Jaka wartość zostanie zwrócona przez powyższe wyrażenie?
**Odpowiedź: "goh angasal a m'i"**

```javascript
( window.foo || ( window.foo = "bar" ) );
```
Pytanie: Jaka jest wartość window.foo?
**Odpowiedź: "bar"**
tylko jeśli window.foo było fałszywe, w innym przypadku zwraca swoją wartość.

```javascript
var foo = "Hello"; (function() { var bar = " World"; alert(foo + bar); })(); alert(foo + bar);
```
Pytanie: Jaki będzie wyniki wywołania dwóch powyższych poleceń `alert`?
**Odpowiedź: "Hello World" & ReferenceError: bar is not defined**

```javascript
var foo = [];
foo.push(1);
foo.push(2);
```
Pytanie: Jaka jest wartość foo.length?
**Odpowiedź: `2`

```javascript
var foo = {};
foo.bar = 'hello';
```
Pytanie: Jaka jest wartość foo.length?
**Odpowiedź: `undefined`

### Pytania jQuery:

* Wyjaśnij termin "chaining".
* Wyjaśnij termin "deferreds".
* Jakie przykłady optymalizacji jQuery potrafisz wykonać?
* Co robi `.end()`?
* Jak i dlaczego użyjesz przestrzeni nazw przy obsłudze wiązania zdarzeń?
* Podaj 4 różne wartości, jakie możesz przekazać do metody jQuery.
  * Selektor (string), HTML (string), funkcja zwrotna, HTMLElement, obiekt, tablica, element tablicy, obiekt jQuery itd.
* Co to jest kolejka effects (lub fx)?
* Jakie są różnice między `.get()`, `[]`, i `.eq()`?
* Jakie są różnice między `.bind()`, `.live()`, i `.delegate()`?
* Jakie są różnice między `$` i `$.fn`? Czym jest `$.fn`?
* Zoptymalizuj selektor:
```javascript
$(".foo div#bar:eq(0)")
```

### Pytania CSS:

* Jaka jest różnica między klasami oraz idendyfikatorami w CSS?
  Idendyfikatory są unikalne, każdy element może posiadać tylko jeden identyfikator, dodatkowo przeglądarka może używać identyfikatorów do nawigacji (scrollując do elementu z danym ID). Klasy nie są unikalne oraz elementy mogą posiadać więcej niż jedną klasę, nie mają większego znaczenia dla samej przeglądarki.
* Opisz BFC(Block Formatting Context) i powiedz jak działa.
  Blokowe formatowanie kontekstu jest częścią wizualnego renderingu CSS strony. Jest to miejsce, w którym występuje układ elementów blokowych i, w którym float'y komunikują się między sobą. W BFC każde 'pudełko' dotyka lewą zewnętrzną krawędzią kontenera (dla formatowania od-prawej-do-lewej dotyka prawej krawędzi). Zasady dla pozycjonowania i czyszczenia float'ów działają w tym samym blokowym formatowaniu kontekstu. Dodatkowo BFC powoduje nakładanie się marginesów (margin collapsing).

  https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Block_formatting_context
* Opisz czym jest z-index oraz jak tworzony jest układ warstw.
  Właściwość z-index kontroluje pionowe nakładania się elementów, które nachodzą na siebie. Bez wartości z-index, elementy układają się w kolejności w jakiej pojawiają się w DOM (najniżej położony element w DOM pojawia się na samej górze). Zagnieżdżanie jest również ważne, jeśli element B jest nad elementem A, dziecko elementu A nigdy nie będzie wyżej niż element B.

  https://css-tricks.com/almanac/properties/z/z-index/
* Jaka jest różnica między resetowaniem, a normalizowaniem styli CSS? Którą wybrałbyś i dlaczego?
  Reset CSS służy usunięciu wszystkich styli CSS nadanych przez przeglądarki, więc trzeba je ostylować na nowo. Normalizowanie styli ustawia takie same style elementów dla każdej przeglądarki oraz naprawia część błędów, więc konieczne jest tylko stylowanie elementów, które różnią się wyglądem od pożądanego efektu. Użyłbym normalizowania, ponieważ każda zmiana będzie miała taki sam efekt w każdej przeglądarce.

  http://stackoverflow.com/questions/6887336/what-is-the-difference-between-normalize-css-and-reset-css

* Jakie są różne metody czyszczenia i które są odpowiednie dla jakich kontekstów?
  - Metoda pustego Div'a:
    <div style="clear:both;"></div>
    Nie używam tej metody, ponieważ w kodzie pozostaje pusty, niepotrzebny div z zahardcorowanym stylem. Tej metody można używać przy tworzeniu layoutów strony (często w stopce)
  - Metoda Overflow: ustawienie wartości 'auto' lub 'hidden' właściwości overflow na elemencie-rodzicu
    Jeśli dodasz overflow: hidden do elementu, który posiada pływające dzieci, automatycznie dopasuje wysokość biorąc pod uwagę dzieci
  - Metoda łatwego czyszczenia: używa selektora elementu-rodzica :after, by dodać 'clear: both'
    .clearfix:after {
      content: ".";
      visibility: hidden;
      display: block;
      height: 0;
      clear: both;
    }
    Często używam tego podejścia, jednak generuje to niepotrzebną zawartość, która nie ma zastosowania.

  https://css-tricks.com/all-about-floats/
* Opisz, czym jest plik "reset" dla CSS i dlaczego jest użyteczny.
* Opisz jak działa właściwość `float`.
  Float'y mogą by używane do opakowywania tekstu wokół obrazka/elementu lub to tworzenia całych layoutów. Pływające elementy pozostają częścią flow strony, w odróżnieniu od elementów o ustalonym położeniu, które są usuwane z flow strony i nie uczestniczą w dostosowywaniu zawartości np. do zmieniającej się szerokości okna.

  https://css-tricks.com/all-about-floats/

* Jak podejdziesz do rozwiązywania problemów dotyczących stylizacji konkretnych przeglądarek?
  - użycie osobnych stylów CSS, które ładowałyby się tylko wtedy gdy dana przeglądarka jest używana
  - używając przedrostków CSS dotyczących poszczególnych przeglądarek (-moz-, -webkit-, itd)
  - resetując lub normalizując CSS

* Jakie znasz techniki kasowania (clearing) i kiedy wskazane jest ich stosowanie?

* Wyjaśnij technikę "CSS sprites" oraz sposób jej wdrożenia na stronie.
  Jest to sposób na zmniejszenie zapytań HTTP, łącząc obrazy w jeden duży. Użyłbym do tego generatora sprite'ów, łącząc wszystkie obrazy w jeden duży, zazwyczaj odseparowane od siebie o piksel. W CSS, umieściłbym obraz tła w klasie sprite, który używałbym do każdego elementu z obrazkiem. Aby określić konkretny obraz lub ikonę, utworzyłbym inną klasę z pozycją obrazu tła i jego wymiarami.

  https://css-tricks.com/css-sprites/
* Jakie znasz techniki kasowania (clearing) i kiedy wskazane jest ich stosowanie?
* Jakie są Twoje ulubione techniki zastępowania obrazów i kiedy je stosujesz?
  Zastępowanie obrazów CSS jest techniką zastępowania tekstowego elementu (zazwyczaj tagu nagłówkowego) obrazem. Można użyć do tego <h1> i tekstu dla benefitów płynących z dostępności oraz SEO.
  Używam zastępowania obrazów (w zależności od potrzeby), kiedy chcę by moja strona była bardziej dostępna dla urządzeń takich jak czytniki itp. Zazwyczaj używam do tego celu ukrywania tagu span poprzed 'display: none'.

  #1: Ukrywanie tagu span poprzez 'display: none'
  <h1 id="logo">
    <span>CSS-Tricks</span>
  </h1>

  h1#logo {
    width: 250px;
    height: 25px;
    background-image: url(logo.gif);
  }
  h1#logo span {
    display: none;
  }

  #2: Text-indent poza zasięgiem wzroku(ekranu)
  <h1 id="logo">
    CSS-Tricks
  </h1>

  h1#logo {
    width: 300px;
    height: 75px;
    background: url(test.png);
    text-indent: -9999px;
  }

  #3: Niewidzialny tekst
  <h3 class="leon">
    <span>CSS-Tricks</span>
  </h3>

  h3.leon {
    width: 300px;
    height: 75px;
    background: url(test.png);
  }
  h3.leon span {
    display: block;
    width: 0;
    height: 0;
    overflow: hidden;
  }

  https://css-tricks.com/css-image-replacement/
* Haczyki właściwości CSS, warunkowe dołączanie plików .css lub... coś innego?
* Jak serwujesz strony dla przeglądarek z ograniczonym wsparciem funkcji?
  - oddzielne style CSS, które ładują się gdy dana przeglądarka jest używana
  - oddzielny layout
  - polyfills (Pollyfil jest kodem, który wykrywa czy są braki w oczekiwanym API i manualnie implementuje je)
  
  * Jakie techniki stosujesz?
      - Graceful Degradation
      
  https://www.sitepoint.com/progressive-enhancement-graceful-degradation-basics/
* Jakie istnieją sposoby wizualnego ukrycia treści (uczynienia ich dostępnymi tylko dla czytników ekranu)?
  - visibility: hidden
  - width: 0; height: 0;
  - text-indent: -1000px
  - absolute position - poza ekranem
* Czy kiedykolwiek używałeś systemów siatek, a jeśli tak, to jakie preferujesz?
  Używałem Boostrap oraz Angular Material. Dodatkowo słyszałem o Skeleton i Foundation. Preferuję Bootstrapa, ponieważ tworzenie stron z tym gridem jest bardzo proste. Jeśli potrzebujesz stałego grida lub responsywnego, jest to kwestia paru zmian. Wyrównanie i zagnieżdżanie kolumn jest również możliwe w obu przypadkach, stałej i zmieniającej się szerokości layoutów.
* Czy używałeś 'media queries' lub tworzyłeś konkretne układy i arkusze dla urządzeń mobilnych?
  Tak, używałem 'media queries' po stworzeniu projektu z użyciem siatki Boostrapa, by nauczyć się jak działają strony responsywne. Kierowałem się zasadą mobile-first, by uzyskać stronę w pełni responsywną i czytelną na każdym urządzeniu bez dodatkowej, niepotrzebnej zawartości.
  'media queries' pozwalają na kontrolowanie używania zadeklarowanych styli CSS bazując na - na przykład - wielkości ekranu, orientacji urządzenia lub gęstości wyświetlacza. Pozwala to na wyświetlanie strony na różne sposoby na różnych urządzeniach.

  http://cssmediaqueries.com/
* Czy miałeś styczność ze stylizacją SVG?
  Małą. Zmieniałem kolor paru SVG.
  Generalnie SVG jest niezależne rozdzielczościowo (skalowalne bez utraty jakości), nie dodaje żadnych dodatkowych i niepotrzebnych zapytań HTTP i jest bardzo proste do skryptowania. Za jego pomocą można stworzyć mapy dróg, grafy, kompleksowe elementy UI, loga i proste gry. Możesz użyć CSS do stylowania SVG jak chcesz. Możliwe jest również użycie animacji, które poruszą całym SVG lub tylko ścieżkami (częściami SVG).

  https://www.smashingmagazine.com/2014/11/styling-and-animating-svgs-with-css/
  https://code.tutsplus.com/articles/why-arent-you-using-svg--net-25414
* Jak optymalizujesz swoje strony do druku?
  - tworzę specjalny arkusz styli do druku
  - staram się unikać niepotrzebnych tabel
  - staram się określić, które partie strony nie mają wartości dla druku (np. poprzez dawanie im klas .no-print z display: none)
  - używam łamania stron (page breaks) w miejscach, gdzie powinny się łamać (.page-break { page-break-before: always; display: none; })
  - ustalam rozmiar strony do druku (szerokość najlepiej podać w calach lub centrymetrach(oba rekomendowane))
  
  https://davidwalsh.name/optimizing-structure-print-css
* Jakie są zalety/wady używania preprocessorów CSS? (SASS, Compass, Stylus, LESS)
  Zalety
    - lepsza organizacja wynikająca z zagnieżdżania selektorów
    - zdolność do definiowania zmiennych i mixinów
    - matematyczne funkcje
    - łączenie plików
    - w paru przypadkach czystsza składnia
  Wady
    - głównie dla projektantów - mniejszy komfort wynikający z używania wiersza poleceń lub konceptów programistycznych
  * Opisz co podoba ci (lub nie) w używanych wcześniej przez ciebie preprocessorów.
    Używałem SASS'a i naprawdę podoba mi się zagnieżdżanie, zmienne i matematyczne funkcje, które pomagają bardzo w stylowaniu. Nie bylo rzeczy, których nie lubiłem, możliwe że moja wiedza o SASS'ie jest zbyt mała.

  http://nosleepforsheep.com/using-a-css-preprocessor/
* Jakie stosujesz "sztuczki" przy pisaniu efektywnych CSS?
  - unikam selektorów, które łapią duże ilości elementów (tagi i uniwersalne selektory)
  - preferuję klasy i identyfikatory zamiast selektorów tagów
  - unikam redundancji selektorów
  - staram się grupować i ponownie wykorzystywać wspólne wartości

  https://css-tricks.com/efficiently-rendering-css/
* Czy używasz narzędzi do przetwarzania CSS? (SASS, Compass, Stylus, LESS)
  * Jeśli tak, opisz cechy, które lubisz i nie lubisz w używanych narzędziach.
* Jak tworzysz i wdrażasz projekt używający niestandardowych czcionek?
  - używając '@font-face' do renderowania czcionki (używa 'src' dla zahardcorowanych zasobów)
  - linkując do zewnętrznego serwisu z czcionkami jako arkusz styli, używając @import lub javascript (link z np. google fonts)
* Wyjaśnij jak przeglądarka określa elementy pasujące do selektora CSS?
  Przeglądarki szukają selektorów od-prawej-do-lewej. Najpierw szuka wszystkich elementów pasujących do danego key selectora (najdalszego na prawo). Później sprawdza czy ten selektor pasuje lub jest w następnym (najdalszym na lewo) elemencie.
* Opisz czym są pseudo-elementy i do czego służą
  Pseudo-elementy zaczynają się od '::' i są używane do stylowania specyficznych części elementu
  Składnia: 'selector::pseudo-element {}'
  Rozróżniamy następujące pseudo-elementy:
   - ::after - dodaje dodatkową warstwę/zawartość po elemencie
   - ::before - dodaje dodatkową warstwę/zawartość przed elementem
   - ::first-letter - wybiera pierwszą literę
   - ::first-line - wybiera pierwszą linię
   - ::selection - wybiera część elementu zaznaczoną przez użytkownika
* Wymień jak najwięcej wartości właściwości 'display'
  display: value; - wyświetla element jako...
  - inline - element liniowy, domyślne ustawienie
  - block -  element blokowy
  - inline-block - blokowy element liniowy
  - flex - blokowo-poziomowy płynny kontener (flex container)
  - inline-flex - liniowo-poziomowy płynny kontener (inline-flex container)
  - inline-table - liniową tabelę
  - run-in - blok lub liniowy element, w zależności od kontekstu
  Pozwala elementowi zachowywać się jak...
  - list-item - <li>
  - table - <table>
  - table-caption - <caption>
  - table-column-group - <colgroup>
  - table-header-group - <thead>
  - table-footer-group - <tfoot>
  - table-row-group - <tbody>
  - table-cell - <td>
  - table-column - <col>
  - table-row - <tr>
  - none - element nie zostanie wyświetlony
  - initial - ustawia wartość tej właściwości do jej domyślnej wartości
  - inherit - odziedzicza wartość po elemencie nadrzędnym (rodzicu)

  https://www.w3schools.com/cssref/pr_class_display.asp
* Jaka jest różnica między display: 'inline' i 'inline-block'
  Elementy z 'display: inline-block' są jak elementy z 'display: inline', lecz mogą mieć szerokość oraz wysokość. To znaczy, że można używać elementów 'inline-block' jako bloków wewnątrz tekstu lub innych elementów.
  
  Różnica w wspieranych stylach:
    inline: tylko margin-left, margin-right, padding-left, padding-right
    inline-block: margin, padding, height, width
* Wyjaśnij czym jest według ciebie model pudełkowy (box model) i jak powiesz przeglądarce używając CSS do renderowania layoutu w różnych modelach pudełkowych.
  Dla celów wyświetlania, każdy element na stronie jest traktowany jako pudełko. Model pudełkowy dotyczy specyfikacji atrybutów pudełka, takich jak szerokość, padding, obramowanie i margines.
  Model pudełkowy można ustawić dodając właściwość 'box-sizing'. Wartości: 'content-box' (standardowo), 'padding-box' i 'border-box'.
  - Content-box: szerokość i wysokość uwzględniają zawartość, ale nie padding/obramowanie/margines
  - Padding-box: uwzględniają powyższe razem z paddingiem, lecz bez obramowania/marginesu
  - Border-box uwzględniają powyższe z obramowaniem, lecz bez marginesu
* Co robi ```* { box-sizing: border-box; }```? Jakie są tego zalety?
  Jest to IE6 Quirks mode (tryb dziwactw): jeśli uwstawisz szerokość, dodasz paddingi oraz obramowanie, całkowita szerokość nie zmieni się. Wewnętrzna szerokość dostosuje się do reszty.

  Zalety: Możesz ustawiać wartości paddingów i obramowania bez przejmowania się o 'rozjechanie', rozszerzenie się pudełka. Jest to bardzo wygodne dla kolumnowych layoutów. Możesz również używać na przemian wartości w procentach i pikselach, więc nie musisz polega na elemencie podrzędnym dla paddingu.
* Pracowałeś kiedykolwiek z ekranami Retina? Jeśli tak, jakich technik użyłeś do tego celu?
  Ekrany retina mają podwójną gęstość pikseli, pozwala to na tworzenie ostszych obrazów na mniejszych ekranach. Potrzebne jest dostarczenie odpowiednich obrazów dla tych ekranów.

  Zmiana rozmiaru obrazów
    - używanie alternatywnych obrazów wysokiej rozdzielczości
    - używanie @face-fonts zamiast obrazkowych ikon
    - używanie obrazów SVG zamiast bitmapowych
    - używanie JavaScript do zamieniania wszystkich zwykłych obrazów na te z podwójną rozdzielczością
  Praca z faviconami wysokiej rozdzielczości

  https://www.sitepoint.com/css-techniques-for-retina-displays/
* Czym różni się projekt responsywny od adaptywnego? 
  Responsywny: Jeden podstawowy wygląd, który dostosowwuje się do zmian ekranu
  Adaptywny: Dla każdej możliwej wielkości ekranu dedykowany jest osobny wygląd
* Używałeś Flexboxa lub Grida?
  Tak, używam flexboxa w moich projektach. Jest bardzo prosty i komfortowy w użyciu i daje wspaniałe efekty. Wygląda na to, że grid jest wspierany przez wszystkie większe przeglądarki (oprócz Edge, który wspiera starą składnie), więc warto jest się go nauczyć.

  http://caniuse.com/#feat=css-grid
  https://css-tricks.com/snippets/css/a-guide-to-flexbox/
  https://css-tricks.com/snippets/css/complete-guide-grid/
* Jakiego frameworka CSS używałeś lokalnie, lub na produkcji? Jak byś go zmienił/ulepszył?
  Używałem Boostrapa i Angular Material. Boostrap jest świetny dla małych stron, jednak dla większych projektów jest za dużo do zmieniania. Każdy framework narzuca swój własny styl strony, więc wiele stron wygląda tak samo, tylko ze zmienionymi kolorami. To jest to co chciałbym zmienić w frameworkach CSS - więcej wolności i dopasowywania, by tworzyć strony, które nie wyglądają tak samo jak milion innych.

* Jakie są różnice między relatywnie, statycznie, absolutnie i stale pozycjonowanych elementach?
  Elementy są pozycjonowane statycznie domyślnie. Kiedy element nie ma nadanego 'position', będzie on pozycjonowany statycznie. Te elementy będą układać się jeden pod drugim.
  
  Pozycjonowanie relatywne
  Możesz ustawić pozycję elementu relatywnie pozycjonowanego używając 'top: XXX', 'bottom: XXX', 'left: XXX', 'right: XXX'. Element poruszy się od określonej strony, więc jeśli napiszesz 'top: 50px;' element ruszy się 50 pikseli od góry w dół. Nie ma to wpływu na elementy pozycjonowane statycznie, więc element relatywny oraz statystyczny mogą się na siebie nakładać.

  Elementy pozycjonowanie absolutnie są usunięte z DOM i pozycjonują się bazując na najbliższym nadrzędnym elemencie pozycjonowanym relatywnie. W przeciwieństwie do relatywnie pozycjonowanych elementów, które nie mają wpływu na statyczne elementy, jeśli dasz elementowi 'position: absolute' to tak jakby w ogóle nie istniał (w danym miejscu). To znaczy, że inne statyczne elementy będą poruszać się do góry w miejsce absolutnie pozycjonowanego tak jakby go tam nie było. Jeśli wszystkie nadrzędne elementy są statyczne lub nie ma ich w ogóle, element pozycjonowany absolutnie będzie bazował na <body>.

  Stałe elemenety są kompletnie niezależne od wszystkiego na stronie. Bez względu na rodziców, stały element będzie zawsze pozycjonowany na bazie okna przeglądarki. Interesującą rzeczą jest to, że po zescrollowaniu strony element będzie dalej w tym samym miejscu w oknie przeglądarki, więc zawsze będzie widoczny.

* 'C' w CSS oznacza 'kaskadowe'. Jak 
* The 'C' in CSS stands for Cascading. Jak wyznacza się pierwszeństwo w przypisywaniu stylów? Jak można wykorzystać ten system na swoją korzyść?
  Pierwszeństwo w CSS jest zdeterminowane przez specyficzność oraz dziedziczenie.
  Rosnąca kolejność znaczenia:
    1. Deklaracje 'user agent'
    2. Deklaracje użytkownika
    3. Deklaracje autora
    4. Deklaracje '!important' autora
    5. Deklaracje '!important' użytkownika

  Specyficzność: ID > klasa, pseudo-klasa > element, pseudo-element
  Dziedziczenie: Określona wartość → obliczona wartość → używana wartość → aktualna wartość

  Wiedząc to, mogę określić jak zaplanować mój kod używając specyficzności oraz dziedziczenia, więc będą stanowić tylko minimalny (lub wcale) problem.

  https://www.smashingmagazine.com/2010/04/css-specificity-and-inheritance/

### Pytania z testowania:

* Jakie są niektóre z plusów/minusów testowania pisanego kodu?

  Testowanie kodu (testy jednostkowe) zapewniają, że kod działa tak jak powinien, pozwala prowadzić refaktoryzację kodu i sprawdzać, czy nic nie zostało zepsute.

  Minusem jest to, że testy także potrzebują refaktoryzacji oraz jest to znacznie więcej kodu do konserwacji.

* Jakich narzędzi użyłbyś do testowania swojego kodu?

  * Jasmine - framework TDD
  * Karma - runner testów
  * Selenium driver - testowanie End-to-End

* Jaka jest różnica pomiędzy testami jednostkowymi a testami funkcjonalnymi/integracyjnymi?

  Testy jednostkowe sprawdzają czy poszczególne części kodu (funkcje) działają poprawnie. Natomiast testy funkcjonalne/integracyjne sprawdzają działanie części systemu, lub systemu jako całości, jak komponenty systemu funkcjonują miedzy sobą etc.

* Jakie zadanie ma tzw. code style linter?

  Eliminacja prostych błędów już podczas pisania kodu. Zapewnia jednakowe, konsekwentne formatowanie kodu dla wszystkich członków zespołu.

### Pytania z wydajności:

* Jakich narzędzi użyłbyś do testowania błędu związanego z wydajnością twojego kodu?

  Chrome Dev-Tools Profiler - pozwala sprawdzić ile czasu wykonuje się jaka funkcji i w ten sposób określić które funkcje zabierają najwięcej procesora.

  [więcej info](https://developers.google.com/web/tools/chrome-devtools/rendering-tools/js-execution)

* Jakie są niektóre ze sposób na poprawienie wydajności przewijania strony?

  * Rozmiar grafik powinien być dostosowany do rozmiaru ich kontenera, powinny być zoptymalizowane aby nie zabierać za dużo transferu.
  * Unikanie używania dużej ilości box-shadow i innych styli wymagających dużej ilości skomplikowanego rysowania przez przeglądarke.
  * Unikanie metod/właściwości JavaScript które powodują reflow/repaint strony przez przeglądarkę, takich jak offset elementów, wielkość kontenerów etc.
  * Używanie debounce w eventach przewijania.

* Wyjaśnij różnicę pomiędzy fazami layout, painting i compositing przeglądarki.

  * layout - jest to faza, w której przeglądarka sprawdza ile miejsca potrzeba dla każdego komponentu na stronie.
  * painting - wypełnianie pixelami, rysowanie tekstów, kolorów, grafiki.
  * compositing - składanie komponentów i wyświeltanie ich we właściwej kolejności, na właściwym miejscu - renderowanie całej strony.

  [źródło](https://developers.google.com/web/fundamentals/performance/rendering/?hl=en)

### Pytania z sieci:

* Dlaczego lepiej serwować zasoby strony z wielu domen?

  Ponieważ zwiększa to prędkość ładowania strony:
  * Paralelizacja - pozwala na wysłanie wielu requestów naraz do wielu różnych serwerów, co pozwala na zmniejszenie ogólnego czasu ładowania zasobów.
  * Zmniejszone zużycie zasóbów przez headery - zazwyczaj serwer wysyła klientowi pliki cookie, które dołączane są potem do każdego zapytania w tej samej domenie co strona. Serwując statyczny content z innych domen niż strona unikamy potrzeby wysyłania plików cookie przy każdym zapytaniu.

  [źródło](https://travishorn.com/why-it-is-better-to-serve-site-assets-from-multiple-domains-972a2bf69d71)

* Postaraj się wyjaśnić jak wygląda proces wczytywania strony, od czasu wpisania jej adresu do czasu zakończenia jej ładowania.

  1. Pobranie z DNS adresu IP serwera, bazując na wpisanym adresie URL.
  2. Wysłanie zapytania HTTP do serwera.
  3. Parsowanie odpowiedzi i renderowanie strony.

  [więcej szczegółów](http://stackoverflow.com/a/2092602)

* Jakie są różnice pomiędzy Long-Polling, WebSockets i Server-Sent Events?

  * Long-polling - Klient wysyła zapytanie do serwera. Kiedy serwer będzie miał nową informację do zaraportowania, odpowiada klientowi. Ten proces jest jednorazowy.
  * WebSockets - Klient łączy się z serwerem i utrzymuje połączenie. Klient może wtedy wymieniać informacje z serwerem.
  * Server-Sent Events - Klient łączy się z serwerem wysyłając zapytanie. Połączenie jest utrzymywane, a serwer może odpowiadać gdy ma nowe informacje do zaraportowania. Połączenie to w przeciwieństwie do WebSocketów jest jednokierunkowe.

  [więcej informacji](http://stackoverflow.com/a/12855533)

* Wyjaśnij poniższe nagłówki zapytania i odpowiedzi:

  * Różnica pomiędzy Expires, Date, Age i If-Modified-Since
  * Do Not Track
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options

  * Date - data wysłania wiadomości.
  * Expires - data po której wiadomość jest uznawana za nieważną.
  * Age - liczba sekund którą wiadomość spędziła w cache.
  * If-Modified-Since - pozwala serwerowi odpowiedzieć statusem 304 gdy wiadomość nie została zmieniona od daty zawartej w tym nagłówku.
  * DNT (Do Not Track) - prosi serwer aby nie śledził użytkownika.
  * Cache-Control - kontroluje opcje związane z cachowaniem, np. jak długo wiadomość może pozostawać w cache.
  * Transfer-Encoding - forma kodowania wiadomości, np.: chunked, compress, deflate, gzip, identity.
  * ETag - może być użyte w celu wersjonowania wiadomości.
  * X-Frame-Options - kontroluje ochronę przed "clickjackingiem".

  [źródło](https://en.wikipedia.org/wiki/List_of_HTTP_header_fields)

* Co to są metody HTTP? Wymień wszystkie które znasz i krótko je opisz.

  Metody HTTP wskazują jaką akcję klient chce wykonać na wskazanym zasobie.

  * GET - pobiera zasób bez jego modyfikacji.
  * HEAD - takie samo jak GET, ale nie pobiera danych zasobu. Może być przydatne gdy potrzebne są jedynie nagłówki.
  * POST - dodaje nowy zasób.
  * PUT - aktualizuje zasób.
  * DELETE - usuwa zasób.
  * TRACE - zwraca dane otrzymane w zapytaniu bez ich modyfikacji.
  * OPTIONS - zwraca metody obsługiwane przez serwer dla danego zasobu.
  * CONNECT - konwertuje połączenie w tunel TCP/IP.
  * PATCH - nakłada częściowe modyfikacje na zasób.

  [źródło](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol#Request_methods)

### Pytania z kodowania:

* Jaka jest wartość `foo`?
```javascript
var foo = 10 + '20';
```

  `1020` (string)

* Jak napisałbyś tą funkcję?
```javascript
add(2, 5); // 7
add(2)(5); // 7
```

  ```javascript
  const add = (a, b) => {
  if (!b) {
    return b => a + b;
  }

  return a + b;
  };
  ```

* Co zwraca poniższe zapytanie?
```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

  `goh angasal a m'i`

* Jaka jest wartość `window.foo`?
```javascript
( window.foo || ( window.foo = "bar" ) );
```

  Jeśli `window.foo` było wcześniej zdefiniowane to jego wartość się nie zmienia, jeśli nie było to jego wartość to `bar`.

* Jaki jest wynik poniższych dwóch wywołań `alert`?
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

  Drugie wywołanie skutkuje błędem, ponieważ zmienna `bar` jest zdefiniowana w innym block-scope.

* Jaka jest wartość `foo.length`?
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

  `2`

* Jaka jest wartość `foo.x`?
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

  `undefined` - po tym jak `x` jest przypisane do zmiennej `foo`, do zmiennej `foo` zostaje przypisany inny obiekt który nie ma przypisanego `x`. `x` jest wciąż przypisany do poprzedniego obiekty, który teraz znajduje się w zmiennej `bar`.

* Jaki jest wynik poniższych wywołań?
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

  ```
  one
  three
  two
  ```
  
### Pytania AngularJS

* Czym jest AngularJS?
  AngularJS jest JavaScriptowym frameworkiem MVC działającym po stronie klienta do do budowania dynamicznych aplikacji webowych. AngularJS został stworzony jako projekt Google, jednak teraz jest open source.
  AngularJS bazuje na HTML oraz JavaScript, więc nie ma potrzebny uczenia się innej składni lub języka.
  AngularJS zmienia statyczny HTML w dynamiczny. Rozwija możliwości HTML dodając wbudowane atrybuty i komponenty i dostarcza możliwości to tworzenia własnych atrybutów używając JavaScirpt.

  https://docs.angularjs.org/guide/introduction
  http://www.tutorialsteacher.com/angularjs/what-is-angularjs
* Wyjaśnij dyrektywę ng-controller.
  Dyrektywa ng-controller dołącza klasę kontrolera do widoku. Jest to kluczowy aspekt tego, jak Angular wspiera MVC. Ng-controller tworzy również nowy zakres.

* Czym jest $rootScope?
  $rootScope odnosi się do obiektu, który jest dostępny z każdego miejsca w aplikacji. Możesz myśleć o $rootScope jako globalnej zmiennej oraz $scope jako lokalnej.

* Jakie jest zastosowanie $routeProvider w AngularJS?
  $routeProvider jest używany do konfigurowania routów w aplikacji.

  https://docs.angularjs.org/api/ngRoute/provider/$routeProvider

* Wyjaśnij dyrektywę ng-include.
  Jest to sposób na pobranie, kompilację i dołączenie szablonu/fragmentu html z innych plików.

* Jak pobierać dane używając AJAX w AngularJS?
  Do pobierania danych używając AJAX można użyć serwisów $http oraz $https
  ```
  $http({
    method: 'GET',
    url: '/someUrl'
  }).then(function successCallback(response) {
    // this callback will be called asynchronously
    // when the response is available
  }, function errorCallback(response) {
    // called asynchronously if an error occurs
    // or server returns response with an error status.
  });
  ```

* Jak weryfikować dane w AngularJS?
  Możesz użyć przepływu danych w dwie strony (data binding, ng-model) by weryfikować dane. Weryfikacja dzieje się w warstwie modelu, gdzie masz dużo opcji do weryfikacji danych używając JavaScriptu i jego metod.

  AngularJS zapewnia podstawową implementację większości typów danych wejściowych HTML5 (text, number, url, emial, date, radio, checkbox) oraz parę dyrektyw dla weryfikacji danych (required, pattern, minlength, maxlength, min, max).

* Jakie są podstawowe kroki do jednostkowego przetestowania filtra w AngularJS?
  1. Wstrzyknąć '$filter'
  2. Wywołać to w ten sposób: '$filter(nazwaFiltra)(daneWejsciowe, opcje)'
  Przykład:
  ```
  describe('The test filter', function () {
  'use strict'; 

  var $filter;

  beforeEach(function () {
    module('myTestFilterModule');

    inject(function (_$filter_) {
      $filter = _$filter_;
    });
  });

    it('should capitalize a string', function () {
      // Arrange.
      var foo = 'hello world', result;

      // Act.
      result = $filter('testFilter')(foo, 'capitalize');

      // Assert.
      expect(result).toEqual('HELLO WORLD');
    });
  });
  ```

  http://stackoverflow.com/questions/21094569/how-to-unit-test-a-filter-in-angularjs-1-x

  * Czym jest wiązanie danych (data binding) w AngularJS?
  Data-binding w aplikacjach w AngularJS jest automatyczną synchronizacją danych między warstwą modelu oraz warstwą widoku komponentów. Sposób w jaki AngularJS implementuje data-binding pozwala traktować warstwę modelu jako jedno-źródło-prawdy w aplikacji. Warstwa widoku jest projekcją warstwy modelu przez cały czas. Kiedy zachodzą zmiany w warstwie modelu, warstwa widoku również się zmienia i vice versa.

  https://docs.angularjs.org/guide/databinding

* Czym jest zakres (scope) w AngularJS?
  Scope jest obiektem, który odnosi się do warstwy modelu aplikacji. Jest kontekstem wykonawczym dla wyrażeń. Zakresy są zorganizowane w hierarchiczną strukturę, które imitują strukurę DOM aplikacji. Zakresy mogą obserwować wyrażenia i propagować zdarzenia.

  https://docs.angularjs.org/guide/scope

* Czym są kontrolery w AngularJS?
  W AngularJS, kontrolery są zdefiniowane jako JavaScriptowe konstruktory, które są używane do powiększenia zakresu (scope) AngularJS. Kiedy kontroller jest załączony w DOM przez dyrektywę 'ng-controller', AngularJS wypromuje nowy obiekt kontrollera używając określonych kontruktorów kontrolera. Nowe dziecko zakresu (scope'u) zostanie stworzone i będzie dostępne jako wstrzykiwalny parametr do konstruktora kontrolera jako '$scope'. Jeśli kontroler został załączony używając kontrolera jako składni, wtedy instancja kontrolera będzie przypisana do właściwości nowego zakresu.

  Używaj kontrolerów do:
    Ustawiania początkowych stanów obiektu $scope
    Dodawania zachowań do obiektu $scope

  Nie używaj kontrolerów do:
    Manipulowania DOM - Kontrolery powinny zawierać tylko logikę biznesową. Wrzucanie jakiejkolwiek logiki prezentacji do kontrolerów znacząco ma wpływ na ich testowalność. AngularJS posiada data-binding dla większości przypadków i dyrektywy do enkapsulacji manualnej manipulacji DOM.
    Formatowania danych wejściowych - Używaj do tego kontrolerów formularzy
    Filtrowania danych wyjściowych - Używaj do tego filtrów
    Współdzielenia kodu lub stanu pomiędzy kontrolerami - Używaj do tego serwisów
    Zarządzania cyklem życia (life-cycle) innych komponentów (np. tworzenie instacji serwisów)

  https://docs.angularjs.org/guide/controller

* Czym są serwisy w AngularJS?
  Serwisy są substytucyjnymi obiektami, które łączone są razem za pomocą wstrzykiwania zalezności (dependency injection). Możesz używać serwisów do organizacji i dzielenia kodu w aplikacji.
  
  Serwisy w AngularJS są:
    Leniwie tworzone (lazily instantiated) - AngularJS tworzy serwisy tylko wtedy kiedy komponent aplikacji zależy od niego
    Singletonami - Każdy komponent zależny od serwisu dostaje referencję to pojedynczej instracji generowanej przez fabrykę serwisu.

  AngularJS oferuje kilka użytecznych serwisów (np. $http), ale dla większości aplikacji będziesz mógł potrzebował (oraz mógł stworzyć) swoje własne.

  https://docs.angularjs.org/guide/services

* Czym są filtry w AngularJS?
  Filtry formatują wartość wyrażenia dla pokazania go użytkownikowi. Mogą być używane w szablonach widoku, kontrolerach oraz serwisach. AngularJS posiada kolekcję wbudowanych filtrów, łatwo jest jednak definiować własne.

  Podstawą dla API jest $filterProvider.

  https://docs.angularjs.org/guide/filter

* Wyjaśnij dyrektywy w AngularJS.
  Wysokopoziomowo, dyrektywy są markerami na elementach DOM (jak na przykład atrybut, nazwa elementu, komentarz lub klasa CSS), które mówią kompilerowi HTML AngularJS ($compile), by dołączył określone zachowanie do tego elementu DOM (np. przez słuchacz zdarzeń (event listener)), lub nawet przekształcać element DOM i jego dzieci.
  
  https://docs.angularjs.org/guide/directive

* Wyjaśnij szablony w AngularJS.
  W AngularJS szablony są pisane z użyciem HTML, który zawiera specyficzne dla AngularJS elementy oraz atrybuty. AngularJS łączy szablon z informacjami warstwy modelu i kontrolera, by renderować dynamiczny widok, który użytkownik widzi w przeglądarce.

  Typy elementów i atrybutów AngularJS, które możesz używać:
    Dyrektywy - Atrybut lub element, który rozszerza istniejący element DOM lub reprezentuje komponent DOM możliwy do ponownego użycia.
    Znacznik (Markup) - Podwójne nawiasy klamrowe {{ }}, by powiązać wyrażenie z elementem
    Filtr - Formatuje dane do wyświetlenia
    Kontrolowane formularze (form controls) - walidują dane wejściowe użytkownika

  https://docs.angularjs.org/guide/templates

* Czym jest routing w AngularJS?
  AngularJS wspiera SPA używając modułu routującego ngRoute. Ten moduł bazuje na url. Kiedy użytkownik żąda określonego url, silnik routingu przechwytuje ten url i renderuje widok bazując na zdefiniowanych zasadach routingu. 

  https://docs.angularjs.org/api/ngRoute/service/$route
  http://www.tutorialsteacher.com/angularjs/angularjs-routing

* Czym są głębokie powiązania (deep linking) w AngularJS?
  Deep linking jest użyciem URL, który bierze określoną stronę (zawartość) bez przeładowywania aplikacji. Pomaga to indeksować, więc te URL mogą być łatwo znalezione przez silniki wyszukiwarek takie jak Google, Yahoo itp.

  Używając AngularJS, deep linking jest domyślnie robione z prefiksem '#' (kiedy tryb HTML5 nie jest ustawiony).

* Jakie są zalety używania AngularJS?
  Zrobiony przez Google
    AngularJS został opracowany tak dobrze jak i utrzymywany przez dedykowanych inżynierów Google'a. To oznacza ogromną społeczność, od której można się uczyć.
  Wspaniałe MVC
    Większość frameworków wymaga od programistów dzielenia aplikacji na wiele komponentów MVC, później programista musi napisać kod, który połączy znów wszystko razem. Jednakże AngularJS łączy wszystko automatycznie.
  Intuicyjność
    AngularJS jest bardziej intuicyjny, jako że robi użytek z HTML jako deklaratywnego języka. Co więcej, jest mniej kruchy na reorganizację.
  Wszechstronność
    AngularJS jest wszechstronną odpowiedzią na szybki programowanie front-endu. Nie potrzebuje żadnych dodatkowych pluginów lub frameworków. Co więcej, posiada szeroki wachlarz właściwości, które zawierają RESTfulowe akcje, budowanie danych, wstrzykiwanie zalezności, testowanie na poziomie przedsiębiorstwa.
  Gotowy do testów jednostkowych
    AngularJS jest gotowy do testów jednostkowych i jest to jedna z jego najlepszych zalet.

* Jakie są wady AngularJS?
  Dezorientacja
    Istnieje wiele sposób na stworzenie tej samej rzeczy używając AngularJS. Czasami dla nowicjuszy może być trudne określenie, który sposób jest lepszy dla danego zadania.
  Powolne UI
    Jeśli jest więcej niż 2000 obserwatorów, mogą wystąpić duże opóźnienia dla interfejsu użytkownika. To oznacza, że możliwa złożoność formularzy Angular jest limitowana. Może to wystąpić w listach i dużych sieciach danych.
  Konflikty nazw
    W AngularJS nie ma możliwości tworzenia paru ng-app (aplikacji) na tej samej stronie. Może to spowodować konflikty nazw.

* Jakie są główne dyrektywy w AngularJS?
  - ng-app − Ta dyrektywa definiuje i linkuje aplikację w HTML
  - ng-model − Ta dyrektywa wiąże wartości danych z aplikacji z HTML'owymi kontrolerami danych wejściowych 
  - ng-bind − Ta dyrektywa wiąże dane aplikacji z tagami HTML

* Wyjaśnij dyrektywę ng-model
  Dyrektywa ng-model jest używana do przepływu danych w dwie strony (two-way data binding). Wiąże elementy <input>, <select> lub <textarea> do określonych wartości na obiekcie #scope. Wartości tych elementów będą wartościami właściwości i vice-versa.

* Wyjaśnij dyrektywę ng-bind.
  Dyrektywa ng-bind łączy właściwość warstwy modelu zadeklarowaną w $scope, dyrektywie ng-model lub rezultat wyrażenia z elementem HTML. Uaktualnia również element, jeśli wartość wyrażenia się zmieniła.

* Wyjaśnij dyrektywę ng-app w AngularJS.
  Dyrektywa ng-app jest punktem startującym aplikację AngularJS. Inicjalizuje framework automatycznie. AngularJS najpierw szuka dyrektywy ng-app w dokumencie HTML po załadowaniu całego dokumentu. Jeśli znajdzie ng-app, ładuje sam siebie i kompiluje szablon HTML.
  Dyrektywa ng-app powinna znajdować się w głównych tagach dokumentu HTML, np. <html> lub <body>, pozwala to kontrolować całą wewnętrzną hierarchię DOM. Jednakże, możesz umieścić ng-app w każdym elemencie DOM.
  AngularJS będzie przetwarzał tylko ten element DOM oraz wszystkie jego dzieci.

### Pytania dodatkowe (zabawne):

* Opowiedz o najfajniejszej rzeczy jaką kiedykolwiek zakodowałeś. Z czego jesteś najbardziej dumny?
* Jakie są Twoje ulubione części narzędzi programistycznych, których używasz?
* Czy masz jakiś swój własny projekt na boku? Jaki?
* Jaka jest Twoja ulubiona funkcja w Internet Explorer?

### React

* Jeśli stworzyłbyś element taki jak Twitter poniżej, jak wyglądała by definicja tego componentu?

```jsx
<Twitter username='tylermcginnis33'>
 {(user) => user === null
   ? <Loading />
   : <Badge info={user} />}
</Twitter>
```

props.children działa jak każde inne prop, może przekazać każdy rodzaj danych, nie tylko te dane, które React wie jak renderować. Dzieci przekazane do niestatndardowego componentu mogą być wszystkim, dopóki komponent ten przekształca je do formy, jaką React zrozumie przed renderowaniem.


```jsx
import React, { Component, PropTypes } from 'react'
import fetchUser from 'twitter'
// fetchUser take in a username returns a promise
// which will resolve with that username's data.

class Twitter extends Component {
  state = {
    user: null,
  }

  componentDidMount () {
    fetchUser(this.props.username)
      .then((user) => this.setState({user}))
  }
  render () {
    return this.props.children(this.state.user)
  }
}

Twitter.propTypes = {
  username: PropTypes.String.isRequired,
};
```

Functions as children![Functions as children](https://facebook.github.io/react/docs/jsx-in-depth.html#functions-as-children)

* Jaka jest różnica między kontrolowanym a niekontrolowanym komponentem?

Komponent kontrolowany jest to komponent w którym React kontroluje wszystko i jest "jedynym źródłem prawdy" dla danych formularza. W komponentach tych wartość elementu pchodzi ze stanu komponentu, a nie bezpośrednio z DOM.

W komponentach niekontrolowanych dane pochodzą bezpośrednio z drzewa DOM. Aby dostać się do tych danych używa się event handlerów lub ref (polecane).

Controlled components![Controlled components](https://facebook.github.io/react/docs/forms.html#controlled-components)
Uncontrolled components![Uncontrolled components](https://facebook.github.io/react/docs/uncontrolled-components.html)

* W którym zdarzeniu cyklu życia elementu wykonuje się rządania AJAX i dlaczego?

Rządania ajax powinny być wykonywane w zdarzeniu componentDidMount. Dzieje się tak ponieważ, gdy rządanie zwróci dane, zazwyczaj chcemy je przypisać do stanu komponentu, a to może zostać wykonane tylko na komponentach już zamontowanych.

State and lifecycle![State and lifecycle](https://facebook.github.io/react/docs/state-and-lifecycle.html)

* Co robi shouldComponentUpdate i dlaczego jest takie ważne?

shouldComponentUpdate jest ważne z powodów wydajnościowych.
Jeżeli wiemy, że pewna cześć naszego UI się nie zmieni, nie ma powodu żeby React dokonywał sprawdzania, czy powinien uaktualniać tę część. Zwracając false z metody shouldComponentUpdate, dajemy znać Reactowi że obecny komponent i wszystkie jego dzieci pozostaną niezmienione.

Optimizing performance![Optimizing performance](https://facebook.github.io/react/docs/optimizing-performance.html)

* Jak dać znać Reactowi, żeby zbudował w Production mode i co to dokładnie spowoduje?

Przeważnie powinno się użyć DefinePlugin dla Webpacka aby ustawić wartość zmiennej środowiskowej NODE_ENV na "production". Spowoduje to usunięcie dodatkowych ostrzeżeń oraz m.in. walidacji propTypes.

Development and production![Development and production](https://facebook.github.io/react/docs/installation.html#development-and-production-versions)

* Dlaczego użyłbyś React.Children.map(props.children, () => ) zamiast props.children.map(() => )

Ponieważ props.children może być zarówno tablicą komponentów, ale także pojedynczym komponentem. Jeśli przekażemy pojedynczy komponent do natywnej funkcji map, funkcja zwróci bład. React.Children.map potrafi obsłużyć dwa przypadki, gdy children są tablicą oraz elementem.

React.Children.map![React.Children.map](https://facebook.github.io/react/docs/react-api.html#react.children.map)

* Opisz eventy w React.

W React natywne eventy opakowane są w instancje SyntheticEvent, które rozwiązują problem różnić w działaniu eventów między przeglądarkami. SyntheticEvent używa się tak samo jak natywnych eventów, mają ten sam interfejs.
React w rzeczywistośći nie przypisuje eventów do samych child nodes. Nasłuchuje on wszystkich eventów na najwyższym komponencie i używa pojedynczego event listenera.

Handling events![Handling events](https://facebook.github.io/react/docs/handling-events.html)

* Jaka jest różnica między createElement i cloneElement?

createElement jest funkcją, która przekształca JSX na obiekt zrozumiały dla React, który jest używany do tworzenia elementów (obiektowej reprezentacji interfejsu użytkownika). cloneElement służy do klonowaina elementów i przekazywania im nowych props.

Create Element![Create Element](https://facebook.github.io/react/docs/react-api.html#createelement)
Clone Element![Clone Element](https://facebook.github.io/react/docs/react-api.html#cloneelement)
 
* Czym jest drugi argument, który możemy przekazać do funkcji setState i do czego służy?

Funkcja setState jest asynchroniczna dlatego przyjmuje callback jako drugi argument. Funkcja ta jest wykonywana, gdy setState skończył swoje wykonanie i komponent jest ponownie renderowany.

setState![setState](https://facebook.github.io/react/docs/react-component.html#setstate)

* Co jest nie tak z tym kodem?

```jsx
this.setState((prevState, props) => {
 return {
   streak: prevState.streak + props.count
 }
})
```

Nic. setState może także przyjmować funkcję jako pierwszy argument. Funkcja ta pozwala na ustawienie obecnego stanu na podstawie stanu poprzedniego.

setState![setState](https://facebook.github.io/react/docs/react-component.html#setstate)
