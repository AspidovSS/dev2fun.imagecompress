# Оптимизация картинок - автоматически и без сторонних сервисов
Модуль который делает оптимизацию jpeg/png картинок для 1С-Битрикс.

Модуль доступен в [маркетплейсе битрикс](http://marketplace.1c-bitrix.ru/solutions/dev2fun.imagecompress/).

## Преимущества модуля:

* модуль использует рекомендуемые google: jpegoptim и optipng
* сжатие картинок в 5-10 раз
* пройдете анализ PageSpeed Insights
* автоматическая оптимизация (на лету)
* оптимизация картинок при ресайзе (на лету)
* не использует сторонние сервисы
* не использует curl
* почти не нагружает сервер
* оптимизирует без грязи
* освободится значительное кол-во места на диске (в 5-10 раз!)
* progressive jpeg
* возможность оптимизации через консоль (в фоне)
* гибкие настройки
* вкл/выкл автоматического уменьшение размера картинок. Можно задать максимальный размер и все картинки которые больше будут автоматически уменьшаться до этого размера.

## Поддержка оптимизации при:
* загрузки картинки превью и детальной у элементов
* загрузки картинки в свойство FILE Image у элементов
* загрузки картинки в разделы элементов
* загрузки картинки в модуль main
* ресайзе картинки (в т.ч. кэшируемой)

## Что также идет:
* вкл/выкл оптимизация у элементов/разделов/ресайза
* можно установить качество jpeg-файлов при сжатии
* можно установить степень сжатия у png-файлов
* вкл/выкл progressive jpeg
* можно сжать все имеющиеся картинки прям из админки

## Консольный скрипт:
/bitrix/modules/dev2fun.imagecompress/console/optimize.php


## Поддерживаемые события

|  название события | передаваемые переменные  | описание 
|---|---|---| 
| OnBeforeResizeImage | $intFileID - идентификатор файла  | Событие запускается перед началом оптимизации (до поиска файла в базе) |
| OnBeforeResizeImageJpegoptim | &$strFilePath - путь до файла,<br> &$quality - качество картинки,<br> &$params - дополнительные параметры  | Событие запускается перед началом оптимизации jpeg-картинок |
| OnBeforeResizeImageOptipng | &$strFilePath - путь до файла,<br> &$quality - степень сжатия картинки,<br> &$params - дополнительные параметры  | Событие запускается перед началом оптимизации png-картинок |
| OnAfterResizeImage | &$strFilePath - путь до файла | Событие запускается после оптимизации |


## Donate

|   |  |
| ------------- | ------------- |
| Yandex.Money  | 410011413398643  |
| Webmoney WMR (rub)  | R218843696478  |
| Webmoney WMU (uah)  | U135571355496  |
| Webmoney WMZ (usd)  | Z418373807413  |
| Webmoney WME (eur)  | E331660539346  |
| Webmoney WMX (btc)  | X740165207511  |
| Webmoney WML (ltc)  | L718094223715  |
| Webmoney WMH (bch)  | H526457512792  |
| PayPal  | [@darkfriend](https://www.paypal.me/darkfriend)  |
| Payeer  | P93175651  |
| Bitcoin  | 15Veahdvoqg3AFx3FvvKL4KEfZb6xZiM6n  |
| Litecoin  | LRN5cssgwrGWMnQruumfV2V7wySoRu7A5t  |
| Ethereum  | 0xe287Ac7150a087e582ab223532928a89c7A7E7B2  |
| BitcoinCash  | bitcoincash:qrl8p6jxgpkeupmvyukg6mnkeafs9fl5dszft9fw9w  |