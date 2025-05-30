# Сценарии использования

## 1. Учет поступления товара

**Актор**: Работник
**Предусловие**: Товар поступил на склад
**Основной сценарий**:
1. Работник открывает форму добавления товара
2. Вводит название, количество, поставщика
3. Система предлагает место хранения
4. Работник подтверждает сохранение
5. Товар добавлен и сохранён в БД

## 2. Учет отгрузки товара

**Актор**: Работник
**Предусловие**: Есть заказ на отгрузку
**Основной сценарий**:
1. Работник выбирает товар из списка
2. Указывает количество к отгрузке и получателя
3. Система проверяет остатки
4. Подтверждение операции
5. Товар списывается и сохраняется в журнал

## 3. Определение места хранения

**Актор**: Работник
**Предусловие**: Имеется поступивший товар без местоположения
**Основной сценарий**:
1. Работник выбирает товар
2. Система предлагает свободные ячейки склада
3. Работник выбирает подходящее место
4. Система сохраняет привязку

## 4. Получение отчёта по остаткам

**Актор**: Работник
**Сценарий**:
1. Открывает страницу отчёта
2. Использует фильтры по типу товара, дате поступления, местоположению
3. Получает таблицу с результатами
