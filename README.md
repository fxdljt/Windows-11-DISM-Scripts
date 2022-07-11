# Windows-11-DISM-Scripts

Оптимизация образа путем удаления предустановленных пакетов программ-мусора, отключение задач обновления, отключение Защитника и другие мелкие изменения. Все это производится стандартными средствами (командами DISM, запросами CMD и изменением ключей реестра).

Все подробности тут: [vk.com/@slmp_mod-windows-11-dism-scripts
](https://vk.com/@slmp_mod-windows-11-dism-scripts)

# Применение:
- Должны быть полные права администратора: Конфигурация компьютера — Конфигурация Windows — Параметры безопасности — Локальные политики — Параметры безопасности — Контроль учетных записей: все администраторы работают в режиме одобрения — Отключено.
- Для применения скриптов понадобиться образ, редакция и контрольные суммы указаны в описании релизов скриптов.
- Образ должен быть смонтирован.
- Понадобиться любой RAM диск, с буквой Z (просто это последняя буква алфавита), размером 11500МБ с которым может работать DISM (SoftPerfect RAM Disk и аналоги).
- Распаковать скрипты, файлы install.wim и boot.wim (из папки source файла .iso) в корень RAM диска.
- Скачать Start11 версии 1.24 и поместить его в Z:\PostClear под именем Start11.exe (по умолчанию скрипты рассчитаны на репак от diakov.net для тихой установки).
- Запустить Clear.bat и ожидать завершение работы окна.
- Убедится в отсутствии ошибок в файле Clear.log по поиску: «операция», «оши», «не ».
- Запустить CMD и выполнить первую команду из файла _readme.txt.
- С помощью UltraISO (или аналогов) удалить в .iso образе файл install.wim и добавить получившийся install.esd и boot.wim.
- Образ готов.
- Во время установки данного образа должен быть выключен интернет, пока система не будет автоматически 2 раза перезагружена.
