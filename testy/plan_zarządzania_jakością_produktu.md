# Plan zarządzania jakością produktu


## Wytwarzanie oprogramowania

Aby zapewnić jak najwyższą jakość oprogramowania zamierzamy uwzględnić następujące narzędzia w procesie tworzenia produktu:

* CircleCi - jako narzędzie do *continous integration*
* Sentry - platforma do monitorowania błędów pochodzących ze wszystkich naszych serwisów
* Prometheus + Grafana - w celu wizualizacji i analizy danych oraz zapytań do bazy danych
* Testy automatyczne
* Testy funkcjonalne

## Przepływ pracy z kontrolą wersji

* Zablokowany branch główny (development). Merge możliwy jedynie poprzez **pull request**.
* Aby **pull request** został zmergowany, muszą zostać spełnione następujące warunki:
	* Akceptacja przez współpracowników poprzez Code Review.
	* Udany build na CircleCI (kompilacja, testy automatyczne i styleguide).

```mermaid
graph LR;
	d#1[development]-->feature/cool-stuff;
	d#1[development]-->feature/pretty-ui;
	feature/pretty-ui--finish feature-->d#2[development];
	d#3[development]--merge fixes downstream-->feature/cool-stuff;
	fix/cant-login-->d#3[development]
	d#2[development]-->fix/cant-login;
	feature/cool-stuff--finish feature-->d#4[development];
	
	style d#1 
	classDef dev fill: pink;
	class d#1d#2,d#3,d#4 dev;
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjE0MjcyOTAzMl19
-->