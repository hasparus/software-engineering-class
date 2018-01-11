# Plan zarządzania jakością produktu


## Wytwarzanie oprogramowania

Aby zapewnić jak najwyższą jakość oprogramowania zamierzamy uwzględnić następujące narzędzia w procesie tworzenia produktu:

* CircleCi - jako narzędzie do *continous integration*
* Sentry - platforma do monitorowania błędów pochodzących ze wszystkich naszych serwisów
* Prometheus + Grafana - w celu wizualizacji i analizy danych oraz zapytań do bazy danych

## Przepływ pracy z kontrolą wersji

* Zablokowany master. Merg

```mermaid
graph LR;
	master--start feature-->feature-branch;
	
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0Mzc4ODkyOTldfQ==
-->