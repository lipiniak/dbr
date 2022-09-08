## Instalacja

Po zklonowaniu repozytorium trzeba wykonac następująe kroki w katalogu głównym aplikacji.

W celu zainstalowania wszystkich potrzebnych pakierów.

`npm install`

W celu zbudowania aplikacji w środowisku lokalnym po zainstalowaniu pakietów.

`npm run build`

W celu wykonania migracji do bazy danych. Konfiguracja bazy danych znajduje się w pliku `.env`


`php artisan migrate`

Przykładowa konfiguracja bazy danych w pliku `.env`:

`DB_CONNECTION=mysql`
`DB_HOST=127.0.0.1`
`DB_PORT=3306`
`DB_DATABASE=dbr`
`DB_USERNAME=root`
`DB_PASSWORD=root`

---------

W celu uruchomienia lokalnego serwera aplikacji trzeba wykonac:

`php artisan serve`