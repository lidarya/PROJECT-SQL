# project_1. Анализ вакансий на hh.ru

## Оглавление  
[1. Описание проекта](.README.md#Описание-проекта)  
[2. Предварительный анализ данных](.README.md#Предварительный-анализ-данных) 
[3. Детальный анализ вакансий](.README.md#Детальный-анализ-вакансий)  
[4. Анализ работодателей](.README.md#Анализ-работодателей)  
[5. Предметный анализ](.README.md#Предметный-анализ)    
[6. Общий вывод и доп. исследования](.README.md#Общий-вывод-и-доп.исследования)

### Описание проекта    

В проекте реализуется анализ вакансий, размещённых на hh.ru, с помощью SQL-запросов. 
Наши данные представляют собой 5 связанных таблиц:
1. VACANCIES - хранит в себе данные по вакансиям (название вакансии, зарплатная вилка, тип графика, тип трудоустройства, требуемый опыт, ключевый навыки, id вакансии, региона и работодателя),
2. AREAS - хранит код города и его название,
3. EMPLOYERS - хранит список работодателей (название и id),
4. INDUSTRIES - хранит варианты сфер деятельности работодателей (название и id),
5. EMPLOYERS_INDUSTRIES - дополнительная таблица, которая существует для организации связи между работодателями и сферами их деятельности (хранит их id).

Проект состоит из пяти частей: предварительный анализ данных, детальный анализ вакансий, анализ работодателей, предметный анализ, общий вывод и дополнительные исследования.


### Предварительный анализ данных

В этом разделе мы знакомимся со структурой данных, определяем их охват, посчитав количество включенных в неё вакансий (49197), работодателей (23501), регионов (1362) и сфер деятельности (294).


### Детальный анализ вакансий

Здесь мы определяем количество вакансий в каждом регионе, средние границы зарплатной вилки (71 065, 110 537), количество вакансий для каждого сочетания типа рабочего графика и типа трудоустройства, количество вакансий для каждой величины опыта работы.


### Анализ работодателей

В этом разделе мы 
1. смотрим, сколько вакансий открыто у различных работодателей, 
2. для каждого региона определяем количество работодателей и вакансий в нем,
3. для каждого работодателя считаем количество регионов, в которых у него есть вакансии,
4. определяем количество работодателей, у которых сфера деятельности не указана, а также находим работодателей с определенным количеством/названиями сфер деятельности,
5. выводим распределение количества вакансий конкретного работодателя по городам-миллионникам.


### Предметный анализ

Здесь мы ищем вакансии, связанные с данными, а также вакансии конкретно для дата-сайентистов. Среди последних мы считаем количество тех, которые подходят начинающим специалистам, а также количество вакансий, в которых в качестве ключевых навыков указаны SQL/Postrges или Python, находим среднее количество требуемых ключевых навыков, определяем среднюю зарплату в зависимости от опыта.


### Общий вывод и доп. исследования