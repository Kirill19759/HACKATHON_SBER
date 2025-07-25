# Создание и обучение модели прогнозирования целевых действий пользователей на платформе 'СберАвтоподписка'
Проект в качестве учебного задания в рамках курса: магистратура ТГУ «Науки о данных и машинное обучение»
Учебная практика (хакатон)

Работу выполнили: 

Тимлид:	Гришин Сергей
  
Члены команды: 
  Вишняков Дмитрий, 
	Данилова Елена, 
	Коваленко Екатерина, 
	Тагильцев Кирилл, 
	Шерин Иван
 
## Цель проекта

Разработать модель для прогнозирования вероятности совершения пользователем целевого действия:
- «Оставить заявку»
- «Заказать звонок»

## Используемые данные

Сервис будет использовать следующие данные:
- Время визита (`visit_*`)
- Рекламные метки (`utm_*`)
- Характеристики устройства (`device_*`)
- Геоданные (`geo_*`)
- Событие (`hit_*`)
- Действие (`event_*`)

## Формат работы сервиса

### Входные данные:
Все перечисленные атрибуты, например:
- `utm_source`
- `device_type`
- `geo_country`
- и другие

### Выходные данные:
Бинарный прогноз:
- `0` — целевое действие не будет совершено
- `1` — целевое действие будет совершено

## Требования к модели

1. **Качество модели:**
   - ROC-AUC > 0.65

2. **Производительность:**
   - Время предсказания ≤ 3 секунд

Полностью задание можно прочитать и скачать в виде [файла](https://lms-cdn.skillfactory.ru/assets/courseware/v1/d71c2fe9706361f6010e7d05243fb4a2/asset-v1:skillfactory+TGUDS-2sem+2025+type@asset+block/%D0%A3%D1%87%D0%B5%D0%B1%D0%BD%D0%B0%D1%8F_%D0%B7%D0%B0%D0%B4%D0%B0%D1%87%D0%B0_%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7_%D1%81%D0%B0%D0%B9%D1%82%D0%B0.docx).

Данные для выполнения практического задания можно скачать [отсюда](https://cloud.mail.ru/public/PXoc/hDmWMRLe6).

## О компании [«СберАвтоподписка»]

«СберАвтоподписка» — это сервис долгосрочной аренды автомобилей для физлиц.

Клиент платит фиксированный ежемесячный платёж и получает в пользование машину на срок от шести месяцев до трёх лет. 

Также в платёж включены:
* страхование (КАСКО, ОСАГО, ДСАГО);
* техническое обслуживание и ремонт;
* сезонная смена шин и их хранение;
* круглосуточная служба поддержки.

За дополнительную сумму можно приобрести услугу консьерж-сервиса — доставку автомобиля до сервисного центра и обратно на техническое обслуживание, сезонную замену шин, ремонт.

## Описание структуры проекта:

