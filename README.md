# Corne-zmk-studio

Скачиваем ZMK Studio и устанавливаем:

https://github.com/zmkfirmware/zmk-studio/releases

немного по сплитам змк

Во-первых, сама по себе правая работать по дефолту не должна. С хостом она общается только через левую.

Во-вторых, между заливами на контроллер прошивок от разных половин нужно шить ресет. Иначе происходит пижня с блютусом, они отказываются спариваться.

В-третьих, сейчас процедура: залил на обе ресет, залил на левую левую, а на правую правую, ресетнул вместе (в течение полсекунды). Должны соединиться, по USB от левой будут приходить клавиши от обоих.

левая половинка главная.
т.е. правая коннектится к левой, а левая к компу. это соответственно влияет и на время работы аккума. левая около недели, правая около 3.

основные доки по прошивке тут:

https://zmk.dev/


![alt text](https://i.imgur.com/UFhfC3h.png)

включение - переключатели должны быть во внутрь на обеих половинках направлены (т.е. зеркально) - направление помечено зеленым :)
для спаривания с компом на моей прошивке  - нажать одновременно красные кнопки, а синие отвечают за порядковый номер подключения. (клавиатура может быть сопряжена с несколькими компами и переключаться между ними по нажатию)
желтое - разблокировать клавиатуру для визуального интерфейса zmk-studio

![alt text](https://i.imgur.com/OBRnq5t.png)

вот это самое важное, редактирование расположения кнопок
сверху - это просто ни на что не влияющий визуал, чтобы удобнее читать было и красивишно оформлено

а касательно раскладки и компановки кнопок в прошивке - у вотчмена есть отличные пресеты, с которых можно начать. они на базе qwerty

https://github.com/aroum/Watchman-layouts


По сути все просто
Редачишь файлик с нужными кодами и их actions забираешь архив с прошивкой через пару минут из вкладки Actions
![alt text](https://i.imgur.com/iJjqwZi.png)
![alt text](https://i.imgur.com/yTVCzIx.png)
![alt text](https://i.imgur.com/9I6MyoF.png)

![alt text](https://i.imgur.com/oWzV0RG.png)


