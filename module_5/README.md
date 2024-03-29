# Проект5 'Компьютер говорит нет'
### Цель проекта:
Построение скоринг модели для вторичных клиентов банка, которая бы предсказывала вероятность дефолта клиента

### Описания полей:

- client_id - идентификатор клиента
- education - уровень образования
- sex - пол заемщика
- age - возраст заемщика
- car - флаг наличия автомобиля
- car_type - флаг автомобиля иномарки
- decline_app_cnt - количество отказанных прошлых заявок
- good_work - флаг наличия “хорошей” работы
- bki_request_cnt - количество запросов в БКИ
- home_address - категоризатор домашнего адреса
- work_address - категоризатор рабочего адреса
- income - доход заемщика
- foreign_passport - наличие загранпаспорта
- sna - связь заемщика с клиентами банка
- first_time - давность наличия информации о заемщике
- score_bki - скоринговый балл по данным из БКИ
- region_rating - рейтинг региона
- app_date - дата подачи заявки
- default - флаг дефолта по кредиту

### Публичный результат метрики на Kaggle: 0.74117

### Проделанная работа:
1. Проведен разведывательный анализ данных
2. Обработаны все выбросы и пропуски
3. Добавлены новые и удалены лишние признаки
4. Приведены в читаемый для модели вид категориальные и бинарные признаки
5. Решена проблема скоррелированных признаков
6. Подобраны гиперпараметры
7. Построены несколько моделей, из которых была выбрана лучшая

## Выводы:
Я довольна своей работой и результатом на Kaggle. Cчитаю что добилась хороших показаний метрики roc-auc, так же при этом были достигнуты неплохие результаты и у остальных метрик.
Можно было продолжить эксперементировать с добавлением/удалением новых признаков, добавить другие библиотеки с моделями классификации такие как xgboost, lightgbm и другие. 
Но мои эксперименты показывали прирост или уменьшение примерно на 0,0001, поэтому было принято решение завершить проект и сдать работу.

## Была проделана работа над ошибками:
1. Исправлены функции
2. Семплинг был проведен только на трейновой выборке

### Был получен новый результат метрики на Kaggle: 0.74307
