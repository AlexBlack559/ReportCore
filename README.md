[![GitHub issues](https://img.shields.io/github/issues/taxnuke/collocore.svg)](https://github.com/AlexBlack559/ReportCore/issues)
[![GitHub license](https://img.shields.io/github/license/taxnuke/collocore.svg)](https://github.com/AlexBlack559/ReportCore/blob/master/LICENSE)

## Ядро для создания отчетов в LaTeX

> Обратная совместимость не гарантируется, поэтому если какой-то проект использует более старую версию, то лучше её и использовать

### Инструкция по применению

Для инициализации проекта выполнить `./collocore/init.sh`


### Устройство collocore, назначение директорий, файлы подключения библиотек и тд.

|    Файл        |                       Роль                                   |
| :------------: | :----------------------------------------------------------: |
| `core.tex`     | самый главный файл, совершает все импорты и вызовы           |
| `packages.tex` | подключает всякие зависимости, окружения LaTeX               |
| `custom.tex`   | для кастомных макросов, логики ядра и блоков текста          |
| `structs.tex`  | форматы нумерации и всё, что определяет структуру документа  |
| `provision`    | "провизия" для автоматической генерации новых проектов       |
| `init.sh`      | скрипт создания нового проекта для использования с collocore |

### Конфигурирование

Чтобы всё работало, у проекта, который это ядро использует, должен быть файл `config.tex`. Примерное содержание данного файла:

<!-- ![config.tex](https://i.imgur.com/v8r5dDB.png) -->
