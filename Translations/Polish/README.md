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
* Z jakimi systemami kontroli wersji pracowałeś / jesteś zapoznany?
Z gitem, pracowałem na githubie i gitlabie. Próbowałem używać interfejsów graficznych gita, ale jednak wolę pracować w command line.
* Opisz kolejne zadania podczas tworzenia strony internetowej?
* Opisz różnicę między stopniowym ulepszaniem (progressive enhancement) i wdzięczną degradacją (graceful degradation)?
  * Dodatkowe punkty za opisanie wykrywania obsługi cech (feature detection)
* Wyjaśnij, co kryje się za terminem "semantyczny HTML".
Semantyczny HTML - jest to używanie znaczników / tagów HTML zgodnie z ich przeznaczeniem i znaczeniem semantycznym, a nie tylko do prezentowania danych. Znaczniki nadają sens i w różnym kontekście mogną oznaczać do innego. Np <i> i <em> <b> i <strong>, section, aside, nav. Jest to ważne dla robotów indeksujących google, dla czytników przeznaczonych dla osób niepełnosprawnych etc.

* Jak optymalizowałbyś zasoby strony internetowej?
  * Myśląc o wielu rozwiązaniach, które zawierają:
    * Łączenie plików
    * Zmniejszenie rozmiaru plików
    * Zasoby CDN
    * Buforowanie
    * itd.
* Dlaczego serwowanie zasobów strony przez wiele domen jest lepsze?
  * Ile zasobów pobiera przeglądarka z danej domeny w jednej chwili?
* Podaj 3 sposoby na zmniejszenie czasu ładowania strony. (postrzeganego lub rzeczywistego czasu ładowania)
* Jeśli dołączasz do projektu, w którym używa się tabulacji, a ty używasz spacji, co wtedy zrobisz?
  * Sugerowanie użycia narzędzi w stylu EditorConfig (http://editorconfig.org)
  * Zgodnie z konwencjami (pozostań konsekwentny)
  * `issue :retab! command`
* Napisz prosty pokaz slajdów
  * Dodatkowe punkty, jeśli nie używasz JS.
* Jakich narzędzi używasz do sprawdzenia wydajności swojego kodu?
  * Profiler, JSPerf, Dromaeo
* Gdybyś mógł opanować jedną technologię w tym roku, jaka byłaby to technologia?
* Wyjaśnij znaczenie standardów sieciowych i ich twórców.
* Czym jest FOUC? Jak unikasz FOUC?

### Pytania HTML:

* Co robi `doctype` i jakie znasz przykłady?
* Jaka jest różnica między trybem standardów a trybem dziwactw (quirks mode)?
* Jakie są ograniczenia w serwowaniu stron XHTML?
  * Czy istnieją problemy z serwowaniem stron jako `application/xhtml+xml`?
* Jak serwujesz stronę z treścią w wielu językach?
  * Co jest ważne przy projektowaniu i tworzeniu stron wielojęzycznych?
* Jaka jest przydatność atrybutów `data-`
* Rozpatrujemy HTML5 jako otwartą platformę internetową. Jakie składniki tworzą HTML5?
* Opisz różnice między cookies, sessionStorage i localStorage.

### Pytania JS:

* Wyjaśnij delegację zdarzeń.
* Wyjaśnij jak działa `this` w JavaScripcie.
* Wyjaśnij jak działa dziedziczenie prototypowe.
* Jak radzisz sobie z testowaniem swojego kodu JavaScript?
* AMD kontra CommonJS?
* Czym jest tablica mieszająca (hashtable)?
* Co oznaczają komunikaty `undefined` i `undeclared` dla zmiennych?
* Czym są domknięcia, jak i po co są używane?
  * Ulubiony wzorzec używany do ich tworzenia? argyle (Dotyczy tylko IIFE)
* Jakie znasz typowe użycie funkcji anonimowych?
* Wyjaśnij pojęcie "Moduł JavaScript" i kiedy jest warte stosowania.
  * Dodatkowe punkty za wzmiankę na temat czystości przestrzeni nazw.
  * Co jeśli Twój kod nie używa przestrzeni nazw?
* Jak organizujesz swój kod? (moduły, klasyczne dziedziczenie?)
* Jaka jest różnicza między obiektami typu `host` i `native`?
* Różnica między:
```javascript
function Person(){} var person = Person() var person = new Person()
```
* Jaka jest różnica między `.call` i `.apply`?
* Wyjaśnij `Function.prototype.bind`?
* Kiedy optymalizujesz swój kod?
* Wyjaśnij działanie dziedziczenia w JavaScript?
* Kiedy użyłbyś `document.write()`?
  * Wiele generowanych reklam używa `document.write()` choć nie jest to mile widziane
* Jakie są różnice między wykrywaniem obsługi funkcji, wnioskowaniem obsługi funkcji i używaniem ciągu UA?
* Omów AJAX jak najbardziej szczegółowo.
* Wyjaśnij działanie JSONP (i dlaczego nie jest właściwie AJAX).
* Czy kiedykolwiek używałeś szablonów w JavaScript?
  * Jeśli tak, jakie to były biblioteki? (Mustache.js, Handlebars itd.)
* Wyjaśnij pojęcie "hoisting".
* Zasieg zmiennych w jsie?

 W JS, do wersji ES6 występowały tylko dwa rodzaje zasięgu zmiennych, tj. globalny (global scope) i zasięg lokalny - w obrębie funkcji (function scope).
 Od ES6 i pojawienia się zmiennych deklarowanych jako let i const pojawił się także zasięg blokowy (tj. wewnątrz { }).

var![var](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var)
let![let](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Statements/let)
const![const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)
Other scopes![other scopes](http://stackoverflow.com/a/500459)

* Opisz bąbelkowanie zdarzeń.
* Jak jest różnica między "atrybutem" i "właściwością"?
* Czemu rozszerzanie obiektów wbudowanych w JavaScript jest złym pomysłem?
* Czemu rozszerzanie to dobry pomysł?
* Jak jest różnicą między zdarzeniami `load` i `ready` dla strony internetowej?
* Jaka jest różnica między `==` i `===`?
* Wyjaśnij ewentualny sposób pobrania parametrów z adresu URL w oknie przeglądarki.
* Wyjaśnij politykę `same-origin` w odniesieniu do JavaScript.
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
[1,2,3,4,5].duplicate(); // [1,2,3,4,5,1,2,3,4,5]
```
* Opisz strategię zapamiętywania (unikanie powtarzalnych obliczeń) w JavaScript.
* Dlaczego mówimy wyrażenie trójkowe, co dokładnie oznacza słowo "trójkowy"?
* Czym jest `arity` funkcji?
* Co oznacza `"use strict";`? Jakie są zalety i wady takiego rozwiązania?
* Jaka jest roznica miedzy funkcja a obiektem?

Tak naprawdę funkcja jest specyficznym typem obiektu w JavaScript, posiadającym wszystkie właściwości normalnego obiektu. Jedyną różnicą, między funkcją a zwykłym obiektem, jest możliwość wywołania funkcji, co jest możliwe dzięki wewnętrznej metodzie [[Call]], którą posiadają tylko funkcje.
Prototypem funkcji jest Object, konstruktorem funkcji jest Function();

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

* Opisz czym jest z-index oraz jak tworzony jest układ warstw.
  Właściwość z-index kontroluje pionowe nakładania się elementów, które nachodzą na siebie. Bez wartości z-index, elementy układają się w kolejności w jakiej pojawiają się w DOM (najniżej położony element w DOM pojawia się na samej górze). Zagnieżdżanie jest również ważne, jeśli element B jest nad elementem A, dziecko elementu A nigdy nie będzie wyżej niż element B.

  https://css-tricks.com/almanac/properties/z/z-index/
* Jaka jest różnica między resetowaniem, a normalizowaniem styli CSS? Którą wybrałbyś i dlaczego?
  Reset CSS służy usunięciu wszystkich styli CSS nadanych przez przeglądarki, więc trzeba je ostylować na nowo. Normalizowanie styli ustawia takie same style elementów dla każdej przeglądarki oraz naprawia część błędów, więc konieczne jest tylko stylowanie elementów, które różnią się wyglądem od pożądanego efektu. Użyłbym normalizowania, ponieważ każda zmiana będzie miała taki sam efekt w każdej przeglądarce.

  http://stackoverflow.com/questions/6887336/what-is-the-difference-between-normalize-css-and-reset-css
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
* Haczyki właściwości CSS, warunkowe dołączanie plików .css lub... coś innego?
* Jak serwujesz strony dla przeglądarek z ograniczonym wsparciem funkcji?
  * Jakie techniki stosujesz?
* Jakie istnieją sposoby wizualnego ukrycia treści (uczynienia ich dostępnymi tylko dla czytników ekranu)?
  - visibility: hidden
  - width: 0; height: 0;
  - text-indent: -1000px
  - absolute position - poza ekranem
* Czy kiedykolwiek używałeś systemów siatek, a jeśli tak, to jakie preferujesz?
* Czy używałeś 'media queries' lub tworzyłeś konkretne układy i arkusze dla urządzeń mobilnych?
* Czy miałeś styczność ze stylizacją SVG?
* Jak optymalizujesz swoje strony do druku?
* Jakie stosujesz "sztuczki" przy pisaniu efektywnych CSS?
* Czy używasz narzędzi do przetwarzania CSS? (SASS, Compass, Stylus, LESS)
  * Jeśli tak, opisz cechy, które lubisz i nie lubisz w używanych narzędziach.
* Jak tworzysz i wdrażasz projekt używający niestandardowych czcionek?
  * Czcionki sieciowe (serwisy czcionek jak: Google Webfonts, Typekit itd.)
* Wyjaśnij jak przeglądarka określa elementy pasujące do selektora CSS?

### Pytania z testowania:

* Jakie są niektóre z plusów/minusów testowania pisanego kodu?

  Testowanie kodu (testy jednostkowe) zapewniają, że kod działa tak jak powinien, pozwala prowadzić refaktoryzację kodu i sprawdzać, czy nic nie zostało zepsute.

  Minusem jest to, że testy także potrzebują refaktoryzacji oraz jest to znacznie więcej kodu do konserwacji.

### Pytania dodatkowe (zabawne):

* Opowiedz o najfajniejszej rzeczy jaką kiedykolwiek zakodowałeś. Z czego jesteś najbardziej dumny?
* Jakie są Twoje ulubione części narzędzi programistycznych, których używasz?
* Czy masz jakiś swój własny projekt na boku? Jaki?
* Jaka jest Twoja ulubiona funkcja w Internet Explorer?
