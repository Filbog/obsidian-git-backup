 - Jak wyróżnić się, gdy jest 600 CVek na 1 miejsce
 - Jest bardzo mało ofert pracy dla juniorów na stronach typu justjoin.it, pracuj.pl etc. Czy szukać gdzieś indziej? Cold emails?
 - CV - zdjęcie czy bez zdjęcia
 - "Kropki" przy skillach - wg Wiktora całkiem spoko
-

Ogólne:
 - **Co to jest rozdzielczość ekranu?**
	 - Rozmiar ekranu w pikselach; ile px miesci się na ekranie
 - **KISS/YAGHI/DRY**
	 - **KISS** - Keep it simple stupid - używaj najprostszych rozwiązań, nie kombinuj
	 - **DRY** - don't repeat yourself
	 - **YAGNI** - 
- **Jak rozumiesz pojęcie "all modern browsers"**
	- Chrome, FF, Safari, Edge, przeglądarki mobilne/wszystkie przeglądarki mające >5%
- **CI/CD**
	- **Continuous Integration** and **Continuous Delivery/deployment
	- CD - automatyczny deploy po wykryciu zmian, np po pushu do repo
	- CI - automatyczne testy
- **CORS** - 
	- mechanizm bezpieczeństwa w przeglądarkach
	- Nie pozwala na użycie elementów przez inne "originy"- CDNy, multimedia. Origin sprawdzamy za pomocą: protokół/host/port
	- Ustawienia CORS są po stronie stron, z których "ciągniemy" - np bootstrap CDN po stronie bootstrapa, iframe'y youtuba - po stronie Youtube
- **Button w <form />? Jak spowodować, żeby zachowywał się domyślnie, jak zwykly button?**
	- zachowuje się jako type:submit. możemy ustawić type='button' w HTML (lepsze), lub preventDefault() w JS (troszkę gorszy)
- **Accesibility - co to? Jakie znasz sposoby na wprowadzanie tego?**
	- Dostosowanie strony/aplikacji na potrzeby osób niepełnosprawnych lub nie mających myszki. Niepełnosprawności wzrokowe, słuchowe, ruchowe
	- napisy do audio/video
	- alt
	- semantyczny HTML - uzywanie footer, nav
	- aria- atrybuty, np. aria-label
	- tabowanie po stronie - zazwyczaj ogólnie strona sobie z tym radzi, ale są sposoby, żeby samemu to ustawiać. Np tab-index
- **Wymień sposoby na pokazanie obrazka na stronie**
	- tag img
	- CSS background-image
	- tag picture - daje więcej możliwości niż img, np wyświetlanie konkretnego img w zależności od wielkości viewportu
- **Sposoby na trzymanie danych w przeglądarce**
	- localStorage - dane trzymane tak dlugo, póki ich nie usuniemy
	- sessionStorage - jak zamkniemy kartę/okno to znikają
	- cookies - mają expiration date, ktorą możemy ustawić
- **Mobile first** - co o tym wiesz? Warto?
	- Podejście w projektowaniu storn internetowych i appek mobilnych, gdzie wersja mobilna jest priorytetem, a dopiero później tworzy się wersję desktopową. Najpierw interfejs etc tworzy się pod mobilki, a dopiero potem dostosowuje pod większe ekrany.
	- Plusy:
		- aktualnie większy ruch na mobilkach
		- mobilka zazwyczaj wygląda lepiej na desktopach niż desktop na mobilce
		- strona mobilna na dekstopie nadal będzie czytelna, dekstop na mobilce nie

JS:
1. Sposoby na debuggowanie aplikacji
2. Var VS let VS const
3. Co to jest hoisting?
4. Kiedy warto używać funkcji strzalkowej?
5. Łączenie z API - async/await, then(). Np. "napisz przykład zapytania do API z obsługą blędów. Raz zrób z async/await, raz z then. Użyj dowolnego darmowego API"
6. Co to jest ***strict mode?***
7. Co to jest ***Intersection Observer***? Jeśli nie wiesz, to zaimplementuj jakiś przykład korzystając z internetu
	1. obczaj - lazy loading
Angular
1. Co to Typescript
2. Co to Data binding
3. SPA
4. Dekoratory - zmieniamy nimi zachowanie funkcji, np mamy dekorator @Component
5. Dyrektywy i ich rodzaje
6. pipe'y - funkcje służące to przekształcania danych. Wywolujemy je w templacie, więc dane źródłowe nei są zmienione(?)(pure functions?)
7. co to je modul
8. metody na formularze w Angular
	1. template-driven (RxJS)
	2. reactive
9. Enkapsulacja
10. Lifecycle hooks
	1. co je pierwsze w komponencie, onChange czy onInit - onChange, bo musi załadować potencjalne dane z inputów do komponentu, zanim w ogóle go wyświetli
11. Dependency injection
	1. wstrzykiwanie zależności poprzez:
		1. **constructor**
		2. dekorator **@inject** 
12. Co to router - moduł pozwalający zarządzać URLami na stronie


Mniej istotne
JS
1. Dependencies VS dev dependencies
	1. dev dependencies nie muszą być na produkcji

#coding #frontend #javascript #angular #webdev