## Проект для магазина «Викишоп»
Интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию.

В нашем распоряжении набор данных с разметкой о токсичности правок. Задача - обучить модель классифицировать комментарии на позитивные и негативные.

Требование: значение метрики качества F1 должно быть не меньше 0.75.

## Полученный вывод

В проекте были рассмотрены тексты описаний товаров и комментариев пользователей в интернет-магазине "Викишоп". Задачей было построить модель, определяющую тональность текста - позитивную или негативную. Критерием оценки была метрика F1.

Для выполнения этой задачи тексты были очищены от регулярных выражений, лемматизированы и векторизированы.

Далее было рассмотрено несколько моделей классификации для предсказания тональности: наивный байесовский классификатор, логистическая регрессия, стохастический градиентный спуск и LGBMClassifier. Лучший результат показал стохастический градиентный спуск: на тестовой выборке F1 составила 0.79.
