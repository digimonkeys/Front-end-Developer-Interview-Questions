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
* Opisz różnicę między stopniowym ulepszaniem (progressive enhancement) i wdzięczną degradacją (graceful degradation)?
  * Dodatkowe punkty za opisanie wykrywania obsługi cech (feature detection)  
  
* Wyjaśnij, co kryje się za terminem "semantyczny HTML".  
Semantyczny HTML - jest to używanie znaczników / tagów HTML zgodnie z ich przeznaczeniem i znaczeniem semantycznym, a nie tylko do prezentowania danych. Znaczniki nadają sens i w różnym kontekście mogną oznaczać do innego. Np <i> i <em> <b> i <strong>, section, aside, nav. Jest to ważne dla robotów indeksujących google, dla czytników przeznaczonych dla osób niepełnosprawnych etc.  

* Jak optymalizowałbyś zasoby strony internetowej?  
Optymalizacja obrazków, łączenie plików, Zmniejszenie rozmiaru plików przy użyciu uglifyjs, stosowanie minifikacji, używanie SVG i css sprites (jeden obrazek, używany wiele razy), Zasoby CDN - mogą być serwowane w zależności od odległości od użytkoniwka, response time etc, cachowanie, nie ładować dużych bibliotek jeśli potrzebujemy z nich tylko jednej funkcji  

* Dlaczego serwowanie zasobów strony przez wiele domen jest lepsze?
  * Ile zasobów pobiera przeglądarka z danej domeny w jednej chwili?
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
* Jak serwujesz stronę z treścią w wielu językach?  
Zawsze należy używać atrybutu language na tagu html do określenia domyślnego języka strony. Zawartość w innym języku należy otoczyć jakimś elementem do którego dodamy równiez atrybut language. Dla stron html należy używać atrybutu lang, zaś dla xhtml xml:lang. W html 1.x i w html 5 obu. 
https://www.w3.org/International/questions/qa-html-language-declarations  

* Jaka jest przydatność atrybutów `data-`
* Rozpatrujemy HTML5 jako otwartą platformę internetową. Jakie składniki tworzą HTML5?
* Opisz różnice między cookies, sessionStorage i localStorage.

### Pytania JS:

* Wyjaśnij delegację zdarzeń.
* Wyjaśnij jak działa `this` w JavaScripcie.
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
function Person(){} var person = Person() var person = new Person()
```
* Jaka jest różnica między `.call` i `.apply`?
* Wyjaśnij `Function.prototype.bind`?
* Czym jest callback?

Callback jest to funckcja przekazywana do innej funkcji poprzez argument. Funkcja, która przyjmuje callback jako argument może w swoim ciele wywołać przekazaną funkcję. Wywołanie to może nastąpić natychmiast (synchronicznie), albo późniejszym czasie (asynchronicznie).

Callback![Callback](https://en.wikipedia.org/wiki/Callback_(computer_programming))

* Kiedy optymalizujesz swój kod?
* Wyjaśnij działanie dziedziczenia w JavaScript?
* Kiedy użyłbyś `document.write()`?
    Document.write() jest zawsze dostępny, jest dobrym wyborem dla dostawcow skryptow zewnetrznych aby mogli dodać oni swoj kod.
    Wiele generowanych reklam używa `document.write()` choć nie jest to mile widziane.

* Jakie są różnice między wykrywaniem obsługi funkcji, wnioskowaniem obsługi funkcji i używaniem ciągu UA?
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
* Co oznacza `"use strict";`? Jakie są zalety i wady takiego rozwiązania?
* Jaka jest roznica miedzy funkcja a obiektem?
Tak naprawdę funkcja jest specyficznym typem obiektu w JavaScript, posiadającym wszystkie właściwości normalnego obiektu. Jedyną różnicą, między funkcją a zwykłym obiektem, jest możliwość wywołania funkcji, co jest możliwe dzięki wewnętrznej metodzie [[Call]], którą posiadają tylko funkcje.
Prototypem funkcji jest Object, konstruktorem funkcji jest Function();

* Czym jest obietnica (`Promise`)?

Obietnica jest używana do asynchronicznych operacji. Reprezentuje wartość, która może być dostępna teraz, w przyszłości albo nigdy.
Może posiadać jeden z trzech stanów:

- oczekujacy: stan początkowy, nie jest ani spełniona ani odrzucona.
- spełniony: operacja przebiegła pomyślnie.
- odrzucony: operacja się nie powiodła.

Oczekująca obietnica może być spełniona z jakąś wartością lub odrzucona z jakimś powodem (błędem). Gdy tak się stanie, przypisane funkcje w metodzie then zostaną wykonane.

[Promise](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Promise)

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
* Czy używałeś 'media queries' lub tworzyłeś konkretne układy i arkusze dla urządzeń mobilnych?
  Tak, używałem 'media queries' po stworzeniu projektu z użyciem siatki Boostrapa, by nauczyć się jak działają strony responsywne. Kierowałem się zasadą mobile-first, by uzyskać stronę w pełni responsywną i czytelną na każdym urządzeniu bez dodatkowej, niepotrzebnej zawartości.
  'media queries' pozwalają na kontrolowanie używania zadeklarowanych styli CSS bazując na - na przykład - wielkości ekranu, orientacji urządzenia lub gęstości wyświetlacza. Pozwala to na wyświetlanie strony na różne sposoby na różnych urządzeniach.

  http://cssmediaqueries.com/
* Czy miałeś styczność ze stylizacją SVG?
* Jak optymalizujesz swoje strony do druku?
  - tworzę specjalny arkusz styli do druku
  - staram się unikać niepotrzebnych tabel
  - staram się określić, które partie strony nie mają wartości dla druku (np. poprzez dawanie im klas .no-print z display: none)
  - używam łamania stron (page breaks) w miejscach, gdzie powinny się łamać (.page-break { page-break-before: always; display: none; })
  - ustalam rozmiar strony do druku (szerokość najlepiej podać w calach lub centrymetrach(oba rekomendowane))
  
  https://davidwalsh.name/optimizing-structure-print-css
* Jakie stosujesz "sztuczki" przy pisaniu efektywnych CSS?
  - unikam selektorów, które łapią duże ilości elementów (tagi i uniwersalne selektory)
  - preferuję klasy i identyfikatory zamiast selektorów tagów
  - unikam redundancji selektorów
  - staram się grupować i ponownie wykorzystywać wspólne wartości

  https://css-tricks.com/efficiently-rendering-css/
* Czy używasz narzędzi do przetwarzania CSS? (SASS, Compass, Stylus, LESS)
  * Jeśli tak, opisz cechy, które lubisz i nie lubisz w używanych narzędziach.
* Jak tworzysz i wdrażasz projekt używający niestandardowych czcionek?
  * Czcionki sieciowe (serwisy czcionek jak: Google Webfonts, Typekit itd.)
* Wyjaśnij jak przeglądarka określa elementy pasujące do selektora CSS?
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

### Pytania z NodeJS:

* Jaka jest preferowana metoda obsługi unhandlaed exceptions w Node.JS?

  Dodanie listener'a event-u procesu `uncaughtException`:

  ```javascript
  process.on('uncaughtException', function(err) {
    // Handle error
    console.log(err);
  });
  ```

### Pytania dodatkowe (zabawne):

* Opowiedz o najfajniejszej rzeczy jaką kiedykolwiek zakodowałeś. Z czego jesteś najbardziej dumny?
* Jakie są Twoje ulubione części narzędzi programistycznych, których używasz?
* Czy masz jakiś swój własny projekt na boku? Jaki?
* Jaka jest Twoja ulubiona funkcja w Internet Explorer?
