# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog][keepachangelog] and this project adheres to [Semantic Versioning][semver].

> Правила ведения файла `CHANGELOG.md`:
>
> - Не опубликованные изменения "накапливаются" в секции `## Unreleased`
> - Описание каждого релиза начинается с секции вида `## vX.X.X` _(`%major%.%minor%.%patch%`)_, и содержит в себе 5 опциональных секций _(но не меньше одной на релиз)_:
>   - `### Added` - Добавленный функционал
>   - `### Fixed` - Исправления
>   - `### Deprecated` - Функционал, помеченный как устаревший и подлежащий удалению в скором времени
>   - `### Removed` - То, что было удалено
>   - `### Changed` - Изменения, явно не связанные с предыдущими тремя секциями
> - Секция релиза **может** сопровождаться датой релиза и иметь вид `## vX.X.X - YYYY-MM-DD`, но выставляться она должна непосредственно перед релизом
> - Присвоение значения новой версии должно соответствовать [правилам семантического версионирования][semver], за исключениями:
>   - Причиной поднятия **мажорного** значения версии являются наличие изменений, обратно не совместимых с теми, что в данный момент находятся на продуктовых серверах ("мягкий" откат невозможен). Это могут быть - **миграции**, изменения неймспейсов классов подлежащих **сериализации** в процессе работы приложения, изменения мажорной версии фреймворка, появление зависимости от какого-либо внешнего сервиса, и любые другие "опасные" изменения
> - Все ссылки должны оформляться в виде сносок `[LINK]:https://...` и располагались строго в блоке релиза
> - Каждая запись **должна** завершаться указанием ссылки на того, кто внёс те или иные изменения


## v0.0.23 - 2020-06-03

### Fixed

- Fix message type in birthday chat reminder

## v0.0.23 - 2020-06-03

### Fixed

- Fix UF_BALANCE in template in schedule payment

## v0.0.22 - 2020-06-01

### Fixed

- Fix UF_COMMENT format in template in schedule payment

## v0.0.22 - 2020-06-01

### Fixed

- Fix duplicate period (not copy payment fact)

## v0.0.21 - 2020-06-01

### Fixed

- Fix UF_BALANCE_CREDIT when save period

## v0.0.20 - 2020-05-31

### Added

- Add birthday chat reminder

## v0.0.19 - 2020-05-28

### Fixed

- Fix template in schedule payment (head column width, font size)

## v0.0.18 - 2020-05-28

### Fixed

- Fix number format in template in schedule payment

### Added

- Add message in happy birthday chat

## v0.0.17 - 2020-05-25

### Fixed

- Change period fields width in title schedule payment table

## v0.0.16 - 2020-05-25

### Fixed

- Delete round function in UF_SPEND_NDS

## v0.0.15 - 2020-05-21

### Fixed

- Change date create period to <15 days
- Set UF_CREDIT in new period to 0

## v0.0.14 - 2020-05-19

### Fixed

- Fix background-color for duplicate period
- Fix period auto create from template

## v0.0.13 - 2020-05-18

### Fixed

- Fix background-color for duplicate period
- Fix show field UF_BALANCE_CREDIT

## v0.0.12 - 2020-05-15

### Added

- Added log for schedule payments

## v0.0.11 - 2020-05-06 

### Fix

-Fix clear "UF_SPEND_NDS" for update period

## v0.0.10 - 2020-05-06 

### Fix

- Fix clear "UF_STATUS" for duplicate period

## v0.0.9 - 2020-04-29

### Fix

- Fix order of operations when update period

## v0.0.9 - 2020-04-29

### Fix

- Limit to 2 decimal places in all fields in schedule.payments

### Added

- Add error when field payment.fact < must.pay.total
- Add error when field payment.plan < pay.total

## v0.0.8 - 2020-04-29

### Fix

- Limit to 2 decimal places in field payment.fact in schedule.payments
- Limit to 2 decimal places in field credit in schedule.payments

## v0.0.7 - 2020-04-28

### Fix

- Limit to 2 decimal places in field payment.plan in schedule.payments

### Added

- Add new field Credit.Balance in schedule.payments

## v0.0.6 - 2020-04-28

### Fix

- Round payment.plan in schedule payments

## v0.0.5 - 2020-04-28

### Added

- When period copied, new period has a blue background

## v0.0.4 - 2020-04-28

### Fixed

- Fix birthday chat type (change to closed)

## v0.0.3 - 2020-04-18

### Added

- Added attach lead chat to deal

## v0.0.2 - 2020-04-18

### Added

- Added attach entity in task out entity in chat

### Fixed

- Fix name function in B24Tech/TaskHandler 
- Fix add chat for birthday worker personal
- Fix execute calculate rule for schedule payments

## v0.0.1 - 2020-04-15

### Added

- Added function CreateHappyBirthdayChat() in /local/php_interface/agents.php ([@RogSC])

### Fixed

- Fix b24tech:schedule.payments - PaymentFact+Credit always < PaymentPlan ([@RogSC])