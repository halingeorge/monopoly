# Монополия


## Сборка и запуск

Клонируйте репозиторий:

```
https://github.com/cmc-haskell-2018/monopoly.git
cd monopoly
```

Соберите проект при помощи [утилиты Stack](https://www.haskellstack.org):

```
stack setup
stack build
```

Собрать проект и запустить игру можно при помощи команды

```
stack build && stack exec monopoly
```

## Правила

Цель
Остаться единственным неотчисленным игроком.

### Начало игры
Фишки всех игроков выстраиваются на поле «Вперед», после чего поочередно каждый делает свой ход.

### Ход игры
Когда подошла ваша очередь, бросьте кубики. Ваша фишка передвинется по доске вперед в направлении по часовой стрелке. Поле, на котором вы остановитесь, определяет, что вам надо делать. На одном поле одновременно могут находиться несколько фишек. В зависимости от того на каком поле вы оказались, вам предстоит:

-купить спецсеминар

-заплатить, если вы оказались на спецсеминаре, который принадлежит другому игроку

-уплатить налоги

-вытащить карточку «Шанс»

-оказаться в академе

-отдохнуть в «Бесплатной курилке»

-получить зарплату в размере 200 научных работ

### Прохождение поля «Вперед»
Всякий раз, когда вы останавливаетесь или проходите поле «Вперед», двигаясь по часовой стрелке, вы получаете 200 научных работ.

### Покупка спецсеминаров
Если вы остановились на поле, обозначающем незанятый другими спецсеминар, у вас будет право первого покупателя на его покупку. Если вы решили назначить преподавателя на спецсемнар, заплатите столько научных работ, сколько указано на игровом поле.

Если вы не купили спецсеминар, то он остается никем не занятым.

### Владение спецсеминарами
Владение спецсеминарами дает вам право взимать научные работы с любых посетителей, которые остановились на поле, обозначающем его. Очень выгодно владеть всеми спецсеминарами одной кафедры. Тогда вы можете назначать преподавателей на любой спецсеминар вашей кафедры.

### Остановка на чужом спецсеминаре
Если вы останавливаетесь на чужом спецсеминаре, который был преобретен ранее другим игроком, с вас могут потребовать научные работы за эту остановку. Количество научных работ, которые придется заплатить, может изменяться в зависимости от того, назначен ли преподаватель на спецсеминар.

### Остановка на поле «Шанс». 
Остановка на таком поле означает, что вам достается одна из карточек. Эти карточки могут потребовать, чтобы вы:

-передвинули вашу фишку

-заплатили научными работами

-получили научные работы

-отправились в академ

-бесплатно освободились из академа

Вы должны немедленно выполнить указания, написанные на карточке. Если вы взяли карточку, на которой написано «бесплатно освободитесь из академа», вы можете оставить ее у себя до тех пор, пока она вам не понадобится, или же вы можете продать ее другому игроку по договорной цене.

Примечание: На карточке может быть написано, что вы должны переместить фишку на другое поле. Если в процессе движения вы пересекаете по часовой стрелке поле «Вперед», то получите 200 научных работ. Если вас отправляют в академ, то поле «Вперед» вы не пересекаете.

### Остановка на поле налогов
Если вы остановились на таком поле, вам просто нужно уплатить соответствующую сумму.

### Бесплатная курилка
Если вы остановились на таком поле, то просто отдохните до следующего вашего хода. Вы находитесь здесь бесплатно и не подвергаетесь никаким штрафам.

### Академ
Вас отправляют в Тюрьму, если:

-Вы остановились на поле «Отправляйтесь в акакдем», или

-Вы взяли карточку «Шанса», на которой написано «Отправляйтесь в академ»

Ваш ход оканчивается, когда вас отправляют в академ. Если вы попадаете в академ по карточке, 200 научных работ вам не выплачивается, где бы вы до того не находились.

Чтобы выйти из академа вам надо:

оставаться здесь, пропуская три своих хода, но каждый раз, когда до вас доходит очередь, бросать кубики, и если на обоих кубиках в один из таких ходов у вас выпадет дубль, вы сможете выйти из академа и пройти такое число полей, которое выпало на кубиках.

После того, как вы пропустили три хода, находясь в академе, вы должны выйти из нее и уплатить 50 научных работ, прежде чем вы сможете передвинуть вашу фишку на выпавшее на кубиках число полей.

Находясь в академе вы имеете право взимать арендную плату за ваши спецсеминары, если она не заложены. Если вы не были отправлены в академ, а просто остановились на этом поле в ходе игры, вы не платите штраф, так как вы «просто посетили» его. Следующим ходом вы можете двигаться дальше, как обычно.


### Отчисление
Если вы должны кому-то больше научных работ, чем вы можете получить по вашим игровым активам, вас объявляют отичсленным, и вы выбываете из игры.

Все спецсеминары, которые принадлежали вам, снова становятся доступны для покупки другим игрокам. Если вы должны были какому-то игроку, ему выплачивается соотвествующее количество научных работ.

### Победитель
Последний оставшийся в игре участник является победителем.


