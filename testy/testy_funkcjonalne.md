# Przypadek testowy nr 1 (do przypadku użycia nr 3)

Nazwa: Planowanie biegów

Opis: Sprawdzenie poprawności działania funkcjonalności planowania biegów.

Oczekiwany rezultat: Użytkownik może zaplanować bieg.

## Część pierwsza: Wprowadzenie trasy.

### Warunki 1

Warunki wstępne: Użytkownik chce pobiec nową trasą.

Kroki wykonania:

1. Wciskam guzik **ołówek-na-mapie -- stwórz trasę**.
2. Oglądam ładne animacje, mapa wlatuje mi na ekran w mniej niż `200ms`.
3. Rysuję ścieżkę, po której chcę pobiec.
   ...

### Warunki 2

Warunki wstępne: Użytkownik chce wybrać sprawdzoną trasę.

Kroki wykonania:

1. Wciskam guzik **ołówek-na-mapie -- stwórz trasę**.
2. Wciskam guzik **zwój - poprzednie trasy**.
3. Oglądam historię map moich poprzednich tras.
4. Wybieram park w którym ostatnio kiepsko mi poszło.
5. Buddy mówi mi, że mam okazję pobić swój czas, bo ostatnio jestem w formie.
   ...

## Część druga: Wybór czasu.

### Warunki A

Warunki wstępne: Użytkownik wprowadził trasę na zapas.

Kroki wykonania:

1. Decyduję się nie planować biegu. Naciskam **zachowaj na później**.

### Warunki B

Warunki wstępne: Użytkownik od razu chce biec. W wybranych godzinach będzie dobra pogoda.

Kroki wykonania:

1. Wybieram czas mojego pierwszego biegu po nowej trasie.
2. System dodaje bieg do mojego dziennika.

### Warunki C

Warunki wstępne: Użytkownik od razu chce biec. W wybranych godzinach będzie kiepska pogoda. Użytkownikowi nie przeszkadza zła pogoda.

Kroki wykoninia:

1. System informuje mnie o złej pogodzie.
2. Decyduję się nie rezygnować z biegu.
3. System dodaje bieg do mojego dziennika.

### Warunki D

Warunki wstępne: Użytkownik od razu chce biec. W wybranych godzinach będzie kiepska pogoda. Użytkownikowi przeszkadza zła pogoda.

Kroki wykoninia:

1. System informuje mnie o złej pogodzie.
2. Decyduję się zrezygnować z biegu.
3. System przenosi mnie do strony głównej aplikacji.

# Przypadek testowy nr 2 (do przypadku użycia nr 5.1)

Nazwa: Znajdowanie partnera do biegu

Opis: Sprawdzenie poprawności działania funkcjonalności znajdowanie partnera do biegu.

Oczekiwany rezultat: Użytkownik może znaleźć partnera do biegu.

## Część pierwsza: znalezienie potencjalnych partnerów do biegu.

Warunki wstępne: użytkownik chce znaleźć partnera

Kroki wykonania:

1. Klikam w zakładkę **your runner buddies**.
2. Wpisuję preferowany czas biegu.
3. Widzę listę proponowanych partnerów do biegu oraz proponowaną trasę.

## Część druga: zaplanowanie wspólnego treningu

### Warunki A

Warunki wstępne: Użytkownikowi podoba się zaproponowana trasa i chętnie dołącza do grupowej konwersacji.

Kroki wykonania:

1. Dołączam do grupowej konwersacji.

### Warunki B

Warunki wstępne: Użytkownikowi nie podoba się zaproponowana trasa biegu. Chiałby zaproponować zmiany.

Kroki wykonania:

1. Proponuję pewne zmiany odnośnie trasy biegu.
2. Mam możliwość rozmowy z innymi użytkonikami w celu przedyskutowania przebiegu trasy.
3. Zostaje wygenerowana nowa trasa.

## Część trzecia: potwierdzenie biegu

### Warunki A

Warunki wstępne: Użtkownik oraz inni użytkownicy chcą wziąść udział w treningu

Kroki wykonania:

1. Klikam przycisk **RUN**, potwierdzając swój udział w treningu.
2. Znajdują się także inni chętni do wspólnego beigu.
3. Bieg zostaje zapisany w dzienniku.

### Warunki B

Warunki wstępne: Użytkownik chce wziąść udział w biegu, ale nie ma innych chętnych

Kroki wykonania:

1. Klikam przycisk **RUN**, potwierdzając swój udział w treningu.
2. Widzę, że gdy po pewnym czasie nadal nie ma żadnych chętnych system zaczyna odliczać czas.
3. System informuje mnie, że nikt nie jest chętny do biegu i przenosi do strony głównej aplikacji.

### Warunki C

Warunki wstępne: Użytkownik nie jest zadowolony z ustaleń na temat trasy i nie decyduje się brać w nim udziału.

Kroki wykonania:

1. Klikam przycisk **PASS**, rezygnując ze wspólnego treningu.
2. System przenosi mnie do strony głównej aplikacji.

# Przypadek testowy nr 3 (do przypadku użycia nr 5.2)

Nazwa: Dołączenie do znajomego podczas biegu

Opis: Sprawdzenie poprawności działania funkcjonalności znajdowania swoich znajomych na mapie i możliwości dołączenia do nich.

Oczekiwany rezultat: Użytkownik może znaleźć swojego znajomego na mapie i do niego dołączyć.

## Część pierwsza: Znalezienie znajomego

## Warunki A

Warunki wstępne: Użytkownik chce znaleźć swoich znajomych na mapie i conajmniej jeden jego znajomy w tym czasie biega.

Kroki wykonania:

1. Klikam opcję **see the map**.
2. Widzę, że moj znajomy biega w okolicy.
3. Klikam na jego avatar i wyświetlają mi się informacje dotyczące biegu mojego znajomego -- czas trwania, prędkość.
4. Klikam przycisk **join**, chcąc do niego dołączyć.
5. Zostaje wyświetlona informacja, mówiąca że mój znajomy został powiadomiony o tym, że planuję do niego dolączyć.

## Warunki B

Warunki wstępne: Użytkownik chce znaleźć swoich znajomych na mapie, ale nikt z jego znajomych nie biega w tym czasie.

Kroki wykonania:

1. Klikam opcję **see the map**.
2. Widzę, że nikt z moich znajomych nie biega akurat w tym czasie.
3. Mam możliwość przejścia do poprzedniej strony.

<!--stackedit_data:
eyJoaXN0b3J5IjpbNTAzMjY5NjYyXX0=
-->