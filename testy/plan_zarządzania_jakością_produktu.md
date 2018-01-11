# Plan zarządzania jakością produktu


## Wytwarzanie oprogramowania

Aby zapewnić jak najwyższą jakość oprogramowania zamierzamy uwzględnić następujące narzędzia w procesie tworzenia produktu:

* CircleCi - jako narzędzie do *continous integration*
* Sentry - platforma do monitorowania błędów pochodzących ze wszystkich naszych serwisów
* Prometheus + Grafana - w celu wizualizacji i analizy danych oraz zapytań do bazy danych

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
	d#3[development]--merge fixes down-->feature/cool-stuff;
	d#2[development]-->hotfix/boss-cant-login;
	hotfix/boss-cant-login-->d#3[development]	
	
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4MTA2Mzc1ODRdfQ==
-->