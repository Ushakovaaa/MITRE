# MITRE
## v13 
## v14 https://attack.mitre.org/resources/updates/updates-october-2023/
Новые техники в разрезе исследуемых платформ
+ [**T1659: Content Injection**](https://attack.mitre.org/techniques/T1659/) - использование скомпрометированных каналов связи + внедрение вредоносной нагрузки в сетевой трафик (методы детектирования: анализ трафика посредством СОВ, создание файлов и процессов. При этом создание файлов и процессов будет очень сходе с Process Injection, где в качестве процессов будут выступать браузеры)
**T1659: Content Injection** (https://attack.mitre.org/techniques/T1659/)
+ **T1657: Financial Theft** (https://attack.mitre.org/techniques/T1657/) - получение денежных средств посредством компрометации легитимных пользователей (методы детектирования: мониторинг почты и журналы финансовых приложений)
+ **T1654: Log Enumeration** (https://attack.mitre.org/techniques/T1654/) - анализ журналов безопасности, включая хранилище SIEM-системы (детектирование: командные строки/процессы/доступ до файлов логов)
+ **T1656: Impersonation** (https://attack.mitre.org/techniques/T1656/) - злоумышленники выдают себя за доверенное лицо/организацию, чтобы убедить выполнить те или иные действия (детектирование: анализ почты)
+ **T1653: Power Settings** (https://attack.mitre.org/techniques/T1653/) - злоумышленник меняет конфигурацию системы для устранения перебоев доступа к зараженному объекту (чтобы узел не переходил в спящий режим/перезагружался/выключался  др.) (детектирование: командная строка, изменение конфигурации питания узла)
+ **T1564.011: Ignore Process Interrupts** (https://attack.mitre.org/techniques/T1564/011/) - скрытие вредоносной нагрузки от процессов их прерывания (например, выполнение в фоновом режиме и после того, как пользователь выйдет из системы) (детектирование: командная строка/процессы)
+ **T1562.012: Disable or Modify Linux Audit System** (https://attack.mitre.org/techniques/T1562/012/) - изменение настроек аудита (актуализировать правило UC-24.007 Modification of auditing and log sending configs on linux host)
+ **T1567.004: Exfiltration Over Webhook** (https://attack.mitre.org/techniques/T1567/004/) - использование webhook для эксфильтрации данных (детектирование: в рамках подтехники детектирование осуществляется преимущественно логами приложений SaaS (github, Google Workspace и тд))
+ **T1036.009: Break Process Trees** (https://attack.mitre.org/techniques/T1036/009/) - изменение идентификатора родительского процесса (PPID) (детектирование: выполнение API функций + процесс не из типичного расположения UC-57.005 System process launched from unusual location on linux host, UC-57.006 Process execution from an unusual directory on linux host)
+ **T1016.002: Wi-Fi Discovery** (https://attack.mitre.org/techniques/T1016/002/) - исследование wi-fi сети (детектирование: вызовы API + командные строки). windows: netsh wlan show profiles, тулза есть в детекте UC-01.007 Util recon on windows host), linux - ничего
+ **T1566.004: Spearphishing Voice** (https://attack.mitre.org/techniques/T1566/004/) - голосовой фишинг, пользователь сам качает вредоносное ПО, следуя инструкциям по телефону (детектирование: журнал телефонных вызовов)
+ **T1027.012: LNK Icon Smuggling** (https://attack.mitre.org/techniques/T1027/012/) - внедрение ссылки на загрузку вредоносного ПО в метаданные ярлыков (LNK) (детектирование: сложная связка событий, включающая создание ярлыка, требуется Sysmon)

T1053.004: Launchd - удалена
