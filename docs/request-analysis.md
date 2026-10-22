# Анализ HTTP-запроса

## Выбранный запрос

- URL: https://github.com/
- Метод: GET
- Статус ответа: 200 OK
- Content-Type: text/html; charset=utf-8
- Дата ответа по заголовку Date: 22 октября 2026 года, 09:58:15 GMT (12:58:15 МСК).

## Источник данных

Данные взяты из предоставленной записи DevTools → Network → Headers для запроса https://github.com/. Значения Request Headers и Response Headers ниже относятся к этому одному запросу.

## Request Headers

| Заголовок | Фактическое значение | Назначение |
| --- | --- | --- |
| Accept | `text/html,application/xhtml+xml,application/xml;q=0.9,image/jxl,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7` | Типы содержимого, которые принимает браузер; q задаёт их относительный приоритет. |
| Accept-Language | `ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7` | Предпочтительные языки ответа: русский имеет наибольший приоритет. |
| Cache-Control | `max-age=0` | Браузер требует свежего ответа; кешированная копия может потребовать проверки у сервера. |
| Upgrade-Insecure-Requests | `1` | Браузер сообщает о предпочтении защищённого соединения. |

## Response Headers

| Заголовок | Фактическое значение | Назначение |
| --- | --- | --- |
| Date | `Thu, 22 Oct 2026 09:58:15 GMT` | Время формирования ответа по данным сервера. |
| Content-Type | `text/html; charset=utf-8` | Ответ содержит HTML в кодировке UTF-8. |
| Cache-Control | `max-age=0, private, must-revalidate` | Ответ предназначен для частного кеша и требует проверки актуальности перед повторным использованием. |
| Strict-Transport-Security | `max-age=31536000; includeSubdomains; preload` | Политика HSTS предписывает использовать HTTPS в течение года, включая поддомены. |
| X-Content-Type-Options | `nosniff` | Запрещает MIME-sniffing в предусмотренных браузером случаях. |
| X-Frame-Options | `deny` | Запрещает отображение страницы внутри фрейма. |
| Server | `github.com` | Значение, которым сервер обозначил себя в ответе. |

Cookie, Set-Cookie, Authorization и другие данные сессии не включены в отчёт.

## Краткий анализ

Браузер отправил GET-запрос к главной странице GitHub и получил ответ 200 OK. Content-Type показывает, что сервер вернул HTML-документ в UTF-8. Request Headers описывают допустимые форматы и языки ответа, а Response Headers — тип содержимого, правила кеширования и ограничения безопасности. Все приведённые значения относятся к выбранному запросу, а не к разным примерам.
