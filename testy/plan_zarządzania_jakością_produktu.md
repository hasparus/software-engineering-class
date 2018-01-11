# Plan zarządzania jakością produktu


## Wytwarzanie oprogramowania

Aby zapewnić jak najwyższą jakość oprogramowania zamierzamy uwzględnić następujące narzędzia w procesie tworzenia produktu:

* CircleCi - jako narzędzie do *continous integration*
* Sentry - platforma do monitorowania błędów pochodzących ze wszystkich naszych serwisów
* Prometheus + Grafana - w celu wizualizacji i analizy danych oraz zapytań do bazy danych

## Przepływ pracy z kontrolą wersji

* Zablokowany master. Merge możliwy jedynie poprzez **pull request**.
* Aby **pull request** został zmergowany, muszą zostać spełnione następujące warunki:
	* Akceptacja przez współpracowników poprzez Code Review.
	* Testy  

```mermaid
graph LR;
	master--start feature-->feature-branch;
	
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA3NzQ1NjcyOV19
-->