Przegląd i odpowiedzialność poszczególnych komponentów

## https://openweathermap.org/current strona udostępniająca darmowe zewnętrzne API które użyliśmy do pobierania danych pogodowych.
/src/App.js to główny plik odpowiedzialny za działanie aplikacji. Tam znajdziemy też kod:
```
const api_call = await fetch(
        `http://api.openweathermap.org/data/2.5/weather?q=${city},${country}&appid=${Api_Key}`
        );
```
w który zostają wstawione dane wpisane przez użytkownika na podstawie których zostaje wysłane odpowiednie żądanie do API. 

Grafiki użyte do obrazkowego przedstawienia aktualnej pogody zostały wzięte z repozytorium https://github.com/erikflowers/weather-icons i zaimplementowane przez konsole w projekcie. W zależności od danych pobranych z API wyświetla się w aplikacji odpowiednia grafika. 


