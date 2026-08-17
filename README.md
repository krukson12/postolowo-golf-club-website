# Postołowo Golf Club — strona internetowa

Publiczny front-end serwisu [postolowo.com](https://www.postolowo.com) oraz
[golf.com.pl](https://www.golf.com.pl). Obie domeny serwują te same pliki.

## Zawartość

| Plik | Opis |
|---|---|
| `index.html` | Strona główna — rezerwacja tee time, kursy golfowe, vouchery, galeria, Stay & Play |
| `ggcc.html` | Podstrona Gdańsk Golf & Country Club — członkostwo, składki, Środowa Liga Golfa |

Obie strony są samodzielnymi plikami: style i skrypty osadzone są bezpośrednio
w dokumencie, bez kroku budowania i bez zależności do zainstalowania. Wystarczy
wgrać je na serwer.

## Technologia

- czysty HTML, CSS i JavaScript, bez frameworka
- [Supabase](https://supabase.com) — baza danych i funkcje brzegowe
- [ING Pay](https://www.ing.pl/bramka-platnicza-ing-pay) — bramka płatnicza
  (BLIK, przelewy online, karty, portfele elektroniczne)
- dwie wersje językowe, polska i angielska, przełączane bez przeładowania strony

## Czego tu nie ma

Repozytorium zawiera wyłącznie warstwę publiczną. Poza nim pozostają panel
administracyjny, funkcje brzegowe, schemat bazy, konfiguracja serwera oraz
dokumenty firmowe.

Klucz Supabase widoczny w kodzie to klucz `anon` — publiczny z założenia,
osadzony w każdej stronie korzystającej z Supabase. Dostęp do danych chronią
polityki RLS po stronie bazy, nie ukrywanie tego klucza.

## Licencja

Treść, zdjęcia i znaki towarowe należą do Postołowo Golf Club Sp. z o.o.
Kod udostępniony do wglądu; wykorzystanie wymaga zgody właściciela.
