# Projekt HTML i CSS

Projekt na zaliczenie części **HTML i CSS** z laboratorium **Technologie Internetowe**.

Uniwersytet Rzeszowski, Informatyka I st. II rok
Wykonał: **Maciej Biel**

Link do działającej wersji: https://ti-project-htmlcss.vercel.app/

W pliku tym pliku została zawarta wymagana dokumentacja.

## Opis Projektu

Tematem mojego projektu jest przykład sklepu internetowego, oferującego cyfrowe gry komputerowe na różne dostępne platformy. Mozna na nim przeglądać dostępne w sklepie gry internetowe, przeglądać jak poglądowo wygląda, opis danej gry, jej wymagania oraz opinie o niej. Strona może zostać rozszerzona o funkcjonalnośc koszyka, składania zamówień, panelu administratora oraz użytkownika.

### Struktura i Omówienie

Strona składa się z czystego HTML i CSS napisanego od zera, nie używałem żadnych zewnętrznych bibliotek do gotowych komponentów CSS czy ikon.

Struktura projektu to:

- w pliku `index.html` - głównego widoku z listą dostępnych gier do kupienia
- w pliku `page.html` - podstrony z konkretnie wybraną grą
- w pliku `login.html` - podstrona z logowaniem
- w pliku `register.html` - podstrona z rejestracją
- w katalogu `img/` znajdują się wszystkie grafiki na stronie
- w pliku `css/styles.css` zawarłem wszystkie style wraz z stylami dla RWD

Strona główna składa się z:

- Nagłówka z nawigacją
- Części głównej z lista kategorii gier oraz platform po lewej stronie oraz listą dostępnych gier w danej kategorii po prawej stronie
- Pod lista gier znajdują się dwie reklamy wewnętrzne strony
- Całkiem na dole znajduje się stopka strony z podstawowymi danymi strony oraz szybką nawigacją

Podstrona składa się z:

- Nagłówka z nawigacją
- Części głównej z galerią zdjęć danej gry, opisem jej, wymaganiami oraz opiniami po lewej stronie oraz możliwością zakupu jej po prawej stronie
- Reklamy i stopka jak w pliku `index.html`

Podczas tworzenia HTML'a użyłem semantycznych znaczników z `HTMLs5`:

- nagłówek strony to `<header>`, w którym znajduje się nawigacja `<nav>`
- główna częśc strony znajduje się w `<main>`
- stopka strony jest oznaczona jako `footer`

Polskie znaki są poprawnie wyświetlane dzięki kodowaniu `UTF-8`.

Hierarchia znaczników `<h1>` - `<h6>` jest poprawna i tworzy łatwy do przeglądania kontekst strony.

Do stylowania nie używałem id tylko samych klas. Każdy tag posiada swoją własną klasę, zgodną z moją wewnętrzną konwencją nazewnictwa opartą na komponentach (`.Komponent-dziecko--modyfikator`), po to aby uniknąć błędów związanych z CSS Specificity.

Wszystkie grafiki zostały skompresowane oraz zmniejszone za pomocą strony https://tinypng.com/, by zapewnić stronie krótki czas ładowania i optymalizację pobierania dużych plików dla użytkowników moblinych, dysponujących wolnym połączeniem internetowym.

Do elementów interaktywych użyłem natywnych elementów HTML takich jak guziki, klikalne ikony, pola wprowadzania tekstu użyłem np. `<button>`, `<select>`, `<input>`, by zapewnić stronie dostępność w najbardziej podstawowym stopniu. Wszystkie zdjęcia posiadają opisany tag `alt`.

Strona jest w pełni zgodna ze standardami W3C dla HTML i CSS.

- https://validator.w3.org/nu/?doc=https%3A%2F%2Fti-project-htmlcss.vercel.app%2Findex.html
- https://validator.w3.org/nu/?doc=https%3A%2F%2Fti-project-htmlcss.vercel.app%2Fpage.html
- https://validator.w3.org/nu/?doc=https%3A%2F%2Fti-project-htmlcss.vercel.app%2Flogin.html
- https://validator.w3.org/nu/?doc=https%3A%2F%2Fti-project-htmlcss.vercel.app%2Fregister.html
- https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fti-project-htmlcss.vercel.app%2F&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=pl-PL

Strona również otrzymała pozytywny wynik SEO, ponieważ spełnia jego podstawowe kryteria:

- posiada tag `<title>`
- posiada tag `<meta name="description">`
- posida favicone
- ma szybki czas ładowania
- wyświetla się dobrze na każdym urządzeniu
- Szczegóły: https://www.seoptimer.com/ti-project-htmlcss.vercel.app

### UI / Wygląda Desktop

Tworząc wygląd strony wzorowałem się na:

- projekcie sklepu z Behance - https://www.behance.net/gallery/88530265/game-store-concept
- stronie Epic Games - https://www.epicgames.com/store/pl/
- stronie Battle net - https://eu.shop.battle.net/pl-pl

Tak wygląda strona główna z pliku `index.html`:

![ti-project-htmlcss vercel app_index html](https://user-images.githubusercontent.com/6316812/147149073-11b11d5c-395f-4940-81fb-285421700e09.png)

Tak wygląda podstrona z pliku `page.html`:

![ti-project-htmlcss vercel app_page html (1)](https://user-images.githubusercontent.com/6316812/147149085-354fc66e-4216-4386-b066-6d3284aa1e72.png)

Tak wygląda podstrona z pliku `login.html`:

![127 0 0 1_5501_login html](https://user-images.githubusercontent.com/6316812/149089686-1d03bcab-6642-4dce-ac46-6401d815f888.png)

Tak wygląda podstrona z pliku `register.html`:

![127 0 0 1_5501_register html](https://user-images.githubusercontent.com/6316812/149089694-bf7a765a-cfff-4f27-80bd-8ac79b9d5e0e.png)

### RWD / Wygląda Mobile

Strona została napisana podejściem Desktop First, jest w pełni responsywna oraz wyświetla się na każdej rozdzielczości:

<img src="https://user-images.githubusercontent.com/6316812/147149318-14e3b487-96b7-4756-8e1f-ded1efbc195b.png" style="max-height: 70%"/>
<img src="https://user-images.githubusercontent.com/6316812/147150007-01c97171-6b3d-47be-9e2d-2e909d746ec5.png" style="max-height: 70%"/>
