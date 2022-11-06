# Требования к проекту 
# 1 Введение
## 1.1 Название продукта 
Music Station
## 1.2 Назначение документа
Документ был разработан для однозначной трактовки требований к разработке программного обеспечения между разработчиком и заказчиком. Здесь описаны функциональные и нефункциональные требования к desktop-приложению «Music Station» для OC Windows 10  и старше. 
## 1.3 Бизнес-требования
### 1.3.1 Исходные данные
В наше время прослушивание музыки является одним из самых доступных способов расслабиться и провести досуг. Еще 10-15 лет назад основным способом для прослушивания музыки выступало радио или домашние магнитофоны и граммофоны. Конечно, данные способы прослушивания музыки пользуются популярностью и сейчас, однако они накладывают ряд неудобств: в случае с радио - зависимость от расписания радиостанций, а в случае с магнитофонами - зависимость от наличия записанных песен на физическом носителе. С развитием интернет-технологий стриминговые сервисы начали набирать популярность всё сильнее, ведь люди получили возможность выбирать любую интересующую их песню и слушать ее в любой момент. В связи с этим сейчас появляется огромное количество музыкальных стриминговых сервисов.
### 1.3.2 Возможности бизнеса
Многие люди абсолютно разных возрастов желают иметь сервис, позволющий прослушивать музыку, изучать информацию о любимых коллективах, жанрах и альбомах, обладая при этом минимальной технической грамотностью. Подобное приложение с интуитивным и структурированным интерефейсом позволит пользователям тратить меньше времени на поиск необходимой песни или альбома, а для каждого зарегистрированного пользователя, после заполнения анкеты о музыкальных предпочтениях, будет предложена постоянно обновляющаяся с учетом последних прослушиваний подборка музыклаьных композиций.
### 1.3.3 Границы проекта
Приложение «Music Station» позволит зарегистрированным пользователям прослушивать музыкальные композиции и альбомы любых жанров и любого года выпуска в формате потоковой передачи данных. Кроме того должны быть реализованы возможности оценивать песни и альбомы, оставлять отзывы и рецензии, просматривать информацию о музыкальных жанрах и направлениях. На основе оценок пользователей у каждой сущности формируется рейтинг, на основе которого будут формироваться подборки для пользователей. Возможность использования приложения для незарегистрированных пользователей не должна быть предусмотрена.
## 1.4 Аналоги 
Spotify — стриминговый сервис, позволяющий легально прослушивать музыкальные композиции, аудиокниги и подкасты, не скачивая их на устройство.

SoundCloud — онлайн-платформа и сайт для распространения оцифрованной звуковой информации (например, музыкальных произведений) обладающая функциями социальной сети, а также одноимённая компания.

Rate Your Music — база метаданных, позволяющая пользователям оценивать и рецензировать музыкальные альбомы, мини-альбомы, синглы, видео, бутлеги и (начиная с 2009 года) фильмы. Эти данные используются впоследствии для выработки рекомендаций пользователям и чартов релизов.
#1.4.1 Отличия от аналогов
Можно заметить, что в Spotify возможность какой либо оценки песен крайней ограничена, а в RYM, наоборот, несмотря на отличные возможности рецензирования и оценок, крайне неудобно реализовано прослушивание музыки. Таким образом, разрабатываемое приложение должно совместить достинства двух этих сервисов.
## 2 Требования пользователя  
## 2.1 Программные интерфейсы 
Продукт должен иметь графический интерфейс. Для этого будет использоваться фреймворк Qt. Все данные, кроме самих песен, будут храниться в базе данных mysql. Вместо самих песен в базе данных будут располагаться их названия, а непосредственно сами композиции должны располагаться в папке на диске. Приложение должно быть написано на языке программирования с++ с использовванием фреймворка Qt.  
## 2.2 Интерфейс пользователя  
(https://github.com/ev1escr/TRITPO_LAB2/blob/main/mockups/profile.png)

(https://github.com/ev1escr/TRITPO_LAB2/blob/main/mockups/suggestions.png)
## 2.3 Характеристики пользователей  
Пользователь приложения - любитель тяжелой музыки, любого возраста и обзраования. Соответственно, он может не иметь опыта работы с вычислительной техникой, поэтому интерфейс должен быть интуитивно понятен и пользователь должен без проблем понимать назначение того или иного параметра.
## 2.4 Предположения и зависимости 
Для приложения необходим компьютер с доступом в интернет и немного свободного места на постоянном запоминающем устройстве.
## 3 Системные требования  
Приложение требует установленной базы данных MySQL, файлов Qt.ОС Windows 10, а также небольшого количества свободного места на диске.
## 3.1 Функциональные требования 
1. Просмотр информации о музыкантах, коллективах, жанрах, треках.
2. Редактирование информации о музыкантах, коллективах, жанрах, треках для владельца продукта. А также возможность добавления отдельных пунктов, например биографии для музыкантов или истории развития жанров.
3. Возможность оценки альбомов и треков.
4. Для каждого альбома и трека предусмотреть блок с ссылками на стриминговые сервисы, где можно будет с ними ознакомиться.
5. Создание учетной записи, после этого понравшиеся сущности можно будет добавить в избранное, где они будут отображаться и пользователь сможет быстро просмотреть интересующий его материал. 
6. Возможность соритровки жанров, коллективов, музыкантов, треков в алфавитном порядке и по популярности. Для треков и альбомов дополнительно добавить возможность сортировки по доте выхода
## 3.2 Нефункциональные требования  
## 3.2.1 Атрибуты качества
Атрибуты важные для пользователя:  
1.Удобство в использовании  
2.Понятный интерфейс   
3.Легкость редактирования ошибок   
