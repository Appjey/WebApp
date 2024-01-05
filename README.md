# Simple String Concatenation Service RELEASE 1.0.0

Сервис с поддержкой веб-формы и RESTful API. Сервис принимает три строки и возвращает их конкатенацию, разделяя их пробелами.

Выполнил студент группы МПИ-23-1-1 Лойко Антон
## Стек
Java 17, Spring Boot, Spring Web, Lombok, Maven

## Запуск (windows)
Для запуска приложения посредством Docker вы можете использовать следующие команды:

1. Перейдите в папку docker из корневого каталога проекта:
```
cd src/main/docker
```
2. Откройте её в терминале и выполните следующую команду:
```
docker-compose up
```
Контейнер с приложением будет доступен по адресу http://localhost:8080/

## Использование

1) Запрос: POST  `/api/dev/concat`
```json
{
  "firstString": "Abc",
  "secondString": "bcd",
  "thirdString": "cde"
}
```
Ответ:
```json
{
  "result": "Abc Bcd Cde"
}
```