# Исследовательский анализ приложения

Доходы (выручка) от транзакций в приложении не покрывают расходы на привлечение новых пользователей и следовательно бизнес несет убытки.

**Цель**: Определить причину убытка в связи с неоправданными инвестициями в рекламу для привлечения новых пользователей.

**Задачи**:
* провести анализ привлеченных пользователей;
* оценить расходы на маркетинг;
* проанализировать эффективность инвестиций в маркетинг.

**Источники данных**:
* лог сервера с информацией о посещениях сайта;
* информация о заказах;
* информация о затратах на маркетинг.

**Библиотеки, использованные для проекта**:
* pandas
* matplotlib
* datetime, timedelta
* numpy

**Ключевые выводы**:
В целом, приложение или рекламную кампанию нельзя назвать убыточными, не зная маржинальности - фактически общая выручка покрывает расходы на привлечение новых пользователей. Увидеть реальную картинку в динамике позволяет когортный анализ, где ROI стабильно находится ниже черты окупаемости. Причина этому - непропорционо растущие затраты на продвижение в США и через канал FaceBoom, куда направлена большая часть бюджета из-за максимальных значений по конверсии. При этом минимальные значения по удержанию в тех же направлениях указывают на необходитмость пересмотреть стратегию продвижения (привлекаются либо нерелевантные/неплатежеспособные пользователи) или перераспределить рекламный бюджет в пользу каналов с минимальным значением ДРР. Стоит также рекомендовать чаще проводить аудит кампаний, чтобы отслеживать изменения и реагировать быстрее, чем по прошествии полугода - с ожидаемой конверсией в покупку за 14 дней, такая ревизия показателей требуется ежемесячно или даже чаще в зависимости от ресурсов и задач
