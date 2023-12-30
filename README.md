# MTA-DreamRPG
Gamemod RPG do Multi Theft Auto, napisany w języku Lua.
# AUTORZY
- Soczek
- Łukasz "Wielebny" Biegaj
- IQ
- Pazdam
- Rick.
# LICENCJA
Warunkiem wykorzystania tego kodu jest NIE TWORZENIE serwera o nazwie Play Your Life. Wykorzystaj go swobodnie, ale swoje dzieło nazwij oryginalnie.
# ZAWARTOŚĆ REPOZYTORIUM

W repozytorium znajduje się:
- Kod Lua serwera
- Struktura bazy danych


W repozytorium nie ma:
- konfiguracji forum.

# GDZIE I JAK URUCHOMIĆ SERWER?
Uruchomienie serwera nie wymaga żadnego specjalnego serwera dedykowanego. Aby go uruchomić, wystarczy zwykły hosting. Polecamy:
- Server Project - http://serverproject.pl/

Aby uruchomić serwer należy:
1. Zainstalować serwer MTA w panelu na stronie hostingu
2. Skopiować pliki serwera do katalogu /mods/deathmatch/resources/
4. Zainicjalizować bazę danych plikami zawartymi w sql/schema.sql
5. Zainicjalizować samodzielnie czyste konto w ACL.
7. Zainstalować serwer, uruchomić, zalogować się

Informacje techniczne
========================================================================

### Wstępnie

Nie ma pełnej dokumentacji do wszystkich elementów kodu. Jest on dość spory i obejmuje wiele aspektów. Poniżej wypisane zostały pewne kluczowe aspekty na które należy zwrócić uwagę, pozostałych rzeczy trzeba dowiedzieć się samemu czytając kod źródłowy.

### Obsługa bazy danych.

Komunikacja przez funkcje db... jest realizowana w zasobie DB2

Pisząc dowolny fragment kodu korzystający z baz danych, powinieneś odwoływać się tylko do zasobu DB2
