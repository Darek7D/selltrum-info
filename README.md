# Selltrum

Selltrum to panel do obsługi sprzedaży w Allegro i WooCommerce. W jednym miejscu możesz przeglądać zamówienia z podłączonych kont i sklepów oraz zarządzać katalogiem produktów, wariantami i stanami magazynowymi. Każda firma ma własny katalog, integracje i uprawnienia użytkowników.

## Allegro

- Połącz konto przez OAuth 2.0. Integracja obsługuje środowisko produkcyjne i osobne środowisko testowe Allegro Sandbox.
- Pobieraj zamówienia, pozycje, statusy oraz dane kupujących i dostawy. Powiąż oferty z lokalnymi wariantami, aby Selltrum mogło rezerwować zapas dla zamówień.
- Włącz synchronizację cen, opisów, zdjęć lub stanów magazynowych dla wybranych powiązań.
- Twórz szkice ofert z katalogu oraz publikuj i kończ oferty utworzone w Selltrum.
- Dla kwalifikujących się zamówień przygotuj etykietę jednej paczki przez **Wysyłam z Allegro**.

Aby sprawdzić integrację na danych testowych, otwórz **Integracje → Allegro**, wybierz **Sandbox** i połącz konto testowe. Operacje w tym środowisku dotyczą konta i ofert w Allegro Sandbox. [Dokumentacja Allegro REST API](https://developer.allegro.pl/) · [Pierwsze kroki z Allegro Sandbox](https://developer.allegro.pl/tutorials/pierwsze-kroki-MRwYEoOq0im)

## WooCommerce

W **Integracje → WooCommerce** podaj publiczny adres HTTPS sklepu i klucz WooCommerce REST API z uprawnieniami do odczytu i zapisu. Przy łączeniu wybierz okres, z którego mają zostać pobrane dotychczasowe zamówienia.

- Nowe i zmienione zamówienia są pobierane w tle. **Pobierz teraz** zleca dodatkowe sprawdzenie, a zamówienia sklepu pojawiają się w sekcji **Zamówienia**.
- Eksportuj produkty i warianty z katalogu, opcjonalnie tworząc nowe produkty jako szkice. Osobno możesz wyeksportować całe drzewo kategorii. Eksport wymaga zgodnej waluty i cen wprowadzanych z podatkiem w ustawieniach sklepu.
- Sprawdzaj wyniki eksportu w panelu integracji i ponawiaj nieudane zadania.

## Katalog i magazyn

Zarządzaj produktami, wariantami, kategoriami, atrybutami, zdjęciami i zapasem. Przy przenoszeniu katalogu z BaseLinkera możesz użyć eksportu XML i sprawdzić podgląd przed uruchomieniem importu.

## Dane i dostęp

Selltrum korzysta z danych konta w zakresie udzielonych uprawnień. Tokeny OAuth Allegro są przechowywane w postaci zaszyfrowanej. Konto Allegro lub sklep WooCommerce można odłączyć w panelu **Integracje**.

## Kontakt

Pytania i problemy zgłaszaj przez zakładkę **Issues**. W publicznych zgłoszeniach pomijaj hasła, klucze API, tokeny i dane kupujących. [Zgłoszenia Selltrum](https://github.com/Darek7D/selltrum-info/issues)
