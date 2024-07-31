# Полная инструкция использования бота «Белозерский стражник»
Белозерский стражник — чат-бот модерации чатов сообществ информационного проекта «Белозерское» в социальной сети ВКонтакте *(далее — бот)*.  
Чтобы бот обработал команду — её нужно написать в один из чатов, где состоит бот. Некоторые команды нужно просто написать и отправить, а некоторые пишутся в ответ на чье-то сообщение. Внимательно читайте описание каждой нужной команды.
## Содержание
* [Уровни прав доступа](https://belozerskoe45.github.io/strajnik/#уровни-прав-доступа)
* Система стоп-листа (автоматического удаления собщений)
* Команды, доступные обычным пользователям
  * Посмотреть свою информационную статистику
  * Посмотреть информационную статистику другого пользователя
  * Информация об экстренных службах Белозерского округа
    * Районные электрические сети
    * Центральная районная больница, регистратуры
    * Отдел полиции МО "Белозерское"
    * Пожарно-спасательная часть №21
* Команды, доступные модераторам чатов
  * Исключить пользователя
  * Выдать предупреждение пользователю
  * Снять предупреждение пользователя
  * Удалить сообщение пользователя
* Команды, доступные администраторам системы
  * Назначить модератора чатов
  * Снять модератора чатов
  * Повысить пользователя
  * Очистить статистику пользователя
  * Установить количество максимальных предупреждений
  * Управлять стоп-листом

## Уровни прав доступа ##
В системе Стражника существует три уровня доступа:
|№|Наименование|     
|:-:|:--|     
|0|Обычный пользователь без дополнительных привелегий|     
|1|Модератор чатов медиапроекта "Белозерское"|    
|2|Администратор системы модерации "Белозерский стражник"|    

Бот реагирует на определенные команды, проверяя, относится ли отправитель этой команды к уровню доступа. Например, команда назначения модераторов доступна только "Администраторам системы модерации".

## Система стоп-листа (автоматического удаления сообщений)
В боте используется система стоп-листа. Если пользователь отправит сообщение со словом, которое внесено в список, то Стражник автоматически удалит это сообщение, а пользователя исключит из чата.   Список слов настроен так, что за несколько месяцев работы этой системы ложных срабатываний не происходило.

## Команды, доступные обычным пользователям
### Посмотреть свою информационную статистику
После отправки команды в чат, бот отправит вашу информационную статистику, в которую будет включены данные вашей страницы, ID (порядковый номер в боте), количество предупреждений, уровень вашего доступа и примечание системы.  
Команда: **!я**  
(фото)

### Посмотреть информационную статистику другого пользователя
После отправки команды в чат, бот отправит информационную статистику пользователя, на которого вы ответите, в которую будет включены данные вашей страницы, ID (порядковый номер в боте), количество предупреждений, уровень доступа пользователя и примечание системы.  
Команда: **!стат** в ответ на сообщение нужного пользователям  1
(фото)

### Информация об экстренных службах Белозерского округа
#### Районные электрические сети
После отправки команды в чат, бот отправит номер телефона Белозерской РЭС, телефон диспетчера и приложит к сообщению две кнопки, по нажатию которой можно перейти на сайт ПАО «СУЭНКО» и ознакомиться с плановыми или аварийными отключениями.  
Команда: **!рэс**   
(фото)

#### Центральная районная больница, регистратура
После отправки команды в чат, бот отправит номера телефонов руководства, взрослой и детской регистратуры Белозерской ЦРБ, а также напишет ее адрес.  
Команда: **!больница**  
(фото)

#### Отдел полиции МО «Белозерское
После отправки команды в чат, бот отправит номер телефона дежурной части отделения полиции «Белозерское» МО МВД "Варгашинский" и его адрес.  
Команда: **!полиция**  
(фото)

#### Пожарно-спасательная часть №21 
После отправки команды в чат, бот отправит номер телефона ПСЧ #21 и ее адрес.  
Команда: **!мчс**  
(фото)

## Команды, доступные модераторам чатов
Эти команды доступны пользователям, с уровнем доступа [1] Модератор чатов медиапроекта "Белозерское" и выше.

### Исключить пользователя
Отправив эту команду в ответ на сообщение пользователя, которого нужно исключить, бот удалит сообщение, на которое вы отвечали, исключит нужного пользователя и оставит отметку в его информационной статистике. Такая мера воздействия применяется к нарушителям правил, отправляющих спам.  
Команда: **!кик** в ответ на сообщение нужного пользователя  
(фото)

### Выдать предупреждение пользователю
Отправив эту команду в ответ на сообщение пользователя, которому нужно выдать предупреждение. Если количество предупреждений пользователя будет равно максимальному количеству — бот исключит его.  
Команда: **!пред** в ответ на сообщение нужного пользователя  
(фото)

### Снять предупреждение пользователя
Отправив эту команду в ответ на сообщение пользователя, которому нужно снять предупреждение, бот снимет у пользователя одно преупреждение.  
Команда: **!снять_пред** в ответ на сообщение нужного пользователя  
(фото)

### Удалить сообщение пользователя
Отправив эту команду в ответ на нужное сообщение, бот бесследно удалит его.  
Команда: **!дел** в ответ на сообщение  

## Команды, доступные администраторам системы
Эти команды доступны пользователям, с уровнем доступа [2] Администратор системы модерации "Белозерский стражник".

### Назначить модератора чатов
Отправив эту команду в ответ на сообщенте нужного пользователя, которому нужно выдать права, бот выдаст ему уровень доступа [1] Модератор чатов медиапроекта "Белозерское".  
Команда: **!модер** в ответ на сообщение  
(фото)

### Снять права доступа к боту
Отправив эту команду в ответ на сообщение нужного пользователя, с которого нужно снять права, бот снимет с него все права доступа.  
Команда: **!снять** в ответ на сообщение  
(фото)

### Управление стоп-листом
После отправки команды в чат, система стоп-листа будет отключена, либо включена. Если система включена - бот будет реагировать на сообщения пользователей, внесенные в список стоп-слов.  
Команда: **!слист**  
(фото)

### Повысить пользователя
После отправки команды в ответ на сообщение нужного пользователя, которого нужно повысить, бот повысит его на 1 уровень доступа выше того, что был до отправки команды. *Например: если у пользователя N был 1 уровень, то после команды он станет 2-м*   
Команда: **!повысить**

### Очистить статистику пользователя
После отправки команды в ответ на сообщение нужного пользователя, которому нужно очистить статистику, бот удалит у пользователя все примечания и отметки в статистике.

### Установить количество максимальных предупреждений
После отправки команды в чат, бот установит количество максимальных предупреждений, по достижению количества которых бот будет выдавать наказания автоматически.

-----
*Чат-бот модерации чатов сообществ информационного проекта «Белозерское» в социальной сети ВКонтакте «Белозерский стражник», его сообщество, Настоящий сайт являются собственностью медиапроекта «Белозерское».  
2023 — 2024 | Россия, Курганская область, Белозерский муниципальный округ*
