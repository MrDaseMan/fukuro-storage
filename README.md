# fukuro-storage
Хранилище для веб-сайта: www.fukuro.su

## Условия использования в личных целях
В случае, если вы решите использовать спрайты/фоны/аудио из данного репозитория, уважительная просьба оставлять ссылки на авторов модов (создателей) и наш проект.

Не забываем о [лицензии](https://github.com/MrDaseMan/fukuro-storage/blob/main/LICENSE), на условиях которой распространяются данные файлы и лицензии, установленные авторами тех или иных изображений/аудио файлов.

## Я хочу добавить свой спрайт/локацию на сайт:
О том, как работать с Open-Source репозиториями и изменять файлы можно, например, почитать [здесь](https://www.dataschool.io/how-to-contribute-on-github/).
**Однако стоит усвоить одно простое правило**: Отправляйте pull request тогда и только тогда, когда полностью уверены, что всё работоспособно и целостно. Не стоит создавать десяток реквестов на одну и ту же тематику, работайте внутри одного!

### Как получить прямую ссылку на спрайт/фон в репозитории:
* **Переходим к интересующему нас изображению:**
![image](https://user-images.githubusercontent.com/48094227/164989805-d5338a97-9e84-476d-b048-7f6fc670a100.png)

* Копируем адрес из адресной строки (Должно получиться нечто в духе: https://github.com/MrDaseMan/fukuro-storage/blob/main/publicstorage/graphics/sprites/el/el_1_grin.png)
* **[Данный пункт устарел]** ~~Заменяем начало в адресе с "https://github.com/MrDaseMan/fukuro-storage/blob/" на "https://raw.githubusercontent.com/MrDaseMan/fukuro-storage/". Должны получить ссылку в формате: https://raw.githubusercontent.com/MrDaseMan/fukuro-storage/publicstorage/graphics/sprites/el/el_1_grin.png, готовую для использования в конфигах.~~
* Убираем из адреса "https://github.com/MrDaseMan/fukuro-storage/blob/main/public", получаем в данном случае ссылку вида "storage/graphics/sprites/el/el_1_grin.png", которую можно использовать в конфигах

### Проверка работоспособности конфига:
Для проверки корректности отредактированных файлов, рекомендую использовать [данный сайт](https://jsonlint.com/)

### Как оформлять спрайты для добавления/изменения:
Все файлы (Одежда/Эмоции/Аксессуары и тела) должны быть переименованы по следующему принципу:

***Тэг-персонажа_Номер-позы_Название***. (Например: **el_1_normal**).

Название файла не должно содержать пробелов и состоять исключительно из латинских символов и знаков "\_".

Тэг персонажа - краткое имя (Например, сокрашение от имени персонажа: "Электроник" -> "el").
Номер позы - соответствующее численное обозначение позы персонажа.
Название - краткое словесное описание элемента персонажа ("Эмоция улыбки" -> smile, "Одежда плащ" -> coat, "Аксессуар часы" -> watches).

Все эти файлы необходимо складировать в папку, названную тэгом персонажа. Допускается разделение спрайта на позы, в отдельные папки для одежды/эмоций/аксессуаров.

Также все спрайты должны быть в разрешении 900x1080.

В случае, если добавляются спрайты из модификаций, следует также приложить скриншот с разрешением автора, либо же просто ссылку на его проект.

### Работа со спрайтами:
Ссылка на конфиг спрайтов: https://github.com/MrDaseMan/fukuro-storage/blob/main/public/configs/characters.json

Рассмотрим работу со спрайтами на примере Электроника:
```json
{
    "name": "Электроник",
    "file": "storage/graphics/sprites/el/el_1_body.png",
    "emotions": [
      "storage/graphics/sprites/el/el_1_grin.png",
      "storage/graphics/sprites/el/el_1_normal.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_shy.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_shy2.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_shy3.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_smile2.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_think.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_think2.png",
      "storage/graphics/sprites/el/el_1_smile.png"
    ],
    "clothes": [
      "storage/graphics/sprites/el/el_1_pioneer.png",
      "storage/graphics/sprites/el/el_1_shirt_alive.png",
      "storage/graphics/sprites/el/el_1_shirt_dead.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_nude.png",
      "storage/graphics/sprites/el/el_1_uniform.png"
    ],
    "offset": "48% 16%",
    "accessories": [ 
      "storage/graphics/sprites/sprites_hitbox_1.png" 
    ]
  },
  {
    "name": "Электроник",
    "file": "storage/graphics/sprites/el/el_2_body.png",
    "emotions": [
      "storage/graphics/sprites/el/el_2_fingal.png",
      "storage/graphics/sprites/el/el_2_sad.png",
      "storage/graphics/sprites/el/el_2_scared.png",
      "storage/graphics/sprites/el/el_2_shocked.png",
      "storage/graphics/sprites/el/el_2_surprise.png",
      "storage/graphics/sprites/el/el_2_upset.png"
    ],
    "clothes": [
      "storage/graphics/sprites/el/el_2_pioneer.png",
      "storage/graphics/sprites/el/el_2_shirt_alive.png",
      "storage/graphics/sprites/el/el_2_shirt_dead.png",
      "storage/graphics/sprites/mods/Additional/el/el_2_nude.png",
      "storage/graphics/sprites/el/el_2_uniform.png"
    ],
    "offset": "51% 16%",
    "accessories": [ 
      "storage/graphics/sprites/sprites_hitbox_1.png"
    ]
  },
  {
    "name": "Электроник",
    "file": "storage/graphics/sprites/el/el_3_body.png",
    "emotions": [
      "storage/graphics/sprites/el/el_3_angry.png",
      "storage/graphics/sprites/el/el_3_laugh.png",
      "storage/graphics/sprites/el/el_3_serious.png"
    ],
    "clothes": [
      "storage/graphics/sprites/el/el_3_pioneer.png",
      "storage/graphics/sprites/el/el_3_shirt_alive.png",
      "storage/graphics/sprites/el/el_3_shirt_dead.png",
      "storage/graphics/sprites/mods/Additional/el/el_3_nude.png",
      "storage/graphics/sprites/el/el_3_uniform.png"
    ],
    "offset": "44% 16%",
    "accessories": [ 
      "storage/graphics/sprites/sprites_hitbox_1.png" 
    ]
}
```

Каждая поза заключена в отдельные '{ ... }' и разделяется запятой. Каждый элемент внутри позы также разделяется запятой и имеет вид:
```json
"Название поля": "Значение",
```
Либо:
```json
"Название поля": [
    "Значение 1",
    "Значение 2",
    "Значение 3"
]
```

Пройдёмся по основным полям:

**"name"**:
```json
"name": "Электроник",
```
Здесь указывается имя персонажа, которое должно быть уникальным на протяжении всего конфига, поэтому рекомендуется записывать его в виде (Заместо звёздочек подставить своё):

**"file"**:
```json
"file": "storage/graphics/sprites/el/el_1_body.png",
```
```json
"file": "storage/graphics/sprites/el/el_2_body.png",
```
```json
"file": "storage/graphics/sprites/el/el_3_body.png",
```
Прямая ссылка на изображение тела персонажа в репозитории. В нашем случае таковое имеется и проблем не возникает, однако может случиться ситуация, когда такового не имеется. В данной ситуации необходимо использовать **hitbox** заглушки, расположенные [здесь](https://github.com/MrDaseMan/fukuro-storage/tree/main/publicstorage/graphics/sprites):
![image](https://user-images.githubusercontent.com/48094227/164989978-e8902db3-2321-44dc-98d5-4b3e327ec1cb.png)

Примером использования такой заглушки может послужить, например, спрайт Виолы:

```json
{
    "name": "Виола",
    "file": "storage/graphics/sprites/sprites_hitbox_1.png",
    "emotions": [
      "storage/graphics/sprites/cs/cs_1_normal.png",
      "storage/graphics/sprites/cs/cs_1_grin.png",
      "storage/graphics/sprites/cs/cs_1_smile.png",
      "storage/graphics/sprites/cs/cs_1_laugh.png",
      "storage/graphics/sprites/cs/cs_1_shy.png",
      "storage/graphics/sprites/cs/cs_1_upset.png",
      "storage/graphics/sprites/cs/cs_1_serious.png",
      "storage/graphics/sprites/cs/cs_1_fear.png",
      "storage/graphics/sprites/cs/cs_1_angry.png",
      "storage/graphics/sprites/cs/cs_1_rage.png",
      "storage/graphics/sprites/cs/cs_1_sad.png",
      "storage/graphics/sprites/cs/cs_1_sad2.png",
      "storage/graphics/sprites/cs/cs_1_cry.png"
    ],
    "clothes": [
      "storage/graphics/sprites/cs/cs_1_labcoat.png",
      "storage/graphics/sprites/cs/cs_1_casual.png",
      "storage/graphics/sprites/cs/cs_1_civil.png",
      "storage/graphics/sprites/cs/cs_1_civil2.png",
      "storage/graphics/sprites/cs/cs_1_shirt.png",
      "storage/graphics/sprites/cs/cs_1_dress.png",
      "storage/graphics/sprites/cs/cs_1_dress2.png",
      "storage/graphics/sprites/cs/cs_1_labcoatns.png",
      "storage/graphics/sprites/cs/cs_1_swim2.png",
      "storage/graphics/sprites/cs/cs_1_swim.png"
    ],
    "offset": "50% 15%",
    "accessories": [
      "storage/graphics/sprites/sprites_hitbox_1.png",
      "storage/graphics/sprites/cs/cs_1_glasses.png",
      "storage/graphics/sprites/cs/cs_1_sun_glasses.png",
      "storage/graphics/sprites/cs/cs_1_glasses_over.png",
      "storage/graphics/sprites/cs/cs_1_glasses_through.png",
      "storage/graphics/sprites/cs/cs_1_stethoscope.png"
    ]
  }
```
Здесь в качестве тела в поле **file** используется заглушка storage/graphics/sprites/sprites_hitbox_1.png

**[Внимание!]** Если спрайт имеет несколько поз, то повторение ссылок в поле "file" недопустимо! В ином случае вероятно появление различных артефактов в отображении на сайте.

**emotions**:
```json
"emotions": [
      "storage/graphics/sprites/el/el_1_grin.png",
      "storage/graphics/sprites/el/el_1_normal.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_shy.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_shy2.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_shy3.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_smile2.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_think.png",
      "storage/graphics/sprites/mods/Additional/el/el_1_think2.png",
      "storage/graphics/sprites/el/el_1_smile.png"
    ],
```

Представляет из себя массив, в котором перечислены эмоции персонажа. Значениями полей массива также являются прямые ссылки на изображения в репозитории, разделяющиеся запятыми. 

**clothes**:
```json
    "clothes": [
      "storage/graphics/sprites/el/el_3_pioneer.png",
      "storage/graphics/sprites/el/el_3_shirt_alive.png",
      "storage/graphics/sprites/el/el_3_shirt_dead.png",
      "storage/graphics/sprites/mods/Additional/el/el_3_nude.png",
      "storage/graphics/sprites/el/el_3_uniform.png"
    ],
```

Представляет из себя массив, в котором перечислены наборы одежды персонажа. Значениями полей массива также являются прямые ссылки на изображения в репозитории, разделяющиеся запятыми.

**[Внимание!]** Если спрайт имеет несколько поз, то значение соответствующих элементов массива должно содержать один и тот же тип одежды. Рассмотрим пример с электроником:

```json
    "clothes": [
      "storage/graphics/sprites/el/el_1_pioneer.png",
      "storage/graphics/sprites/el/el_1_shirt_alive.png",
```
```json
    "clothes": [
      "storage/graphics/sprites/el/el_2_pioneer.png",
      "storage/graphics/sprites/el/el_2_shirt_alive.png",
```
```json
    "clothes": [
      "storage/graphics/sprites/el/el_3_pioneer.png",
      "storage/graphics/sprites/el/el_3_shirt_alive.png",
```

На примере можно заметить, что первым элементом для 1, 2 и 3-х поз находится пионерская форма, а вторым - футболка. 
Если на одной из поз соответствующая одежда отсутствует, необходимо вставить на место соответствующего элемента значение "NONE". Допустим, у спрайта Электроника отсутствует одежда storage/graphics/sprites/el/el_3_shirt_alive.png, тогда в конфиг будет необходимо записать:
```json
    "clothes": [
      "storage/graphics/sprites/el/el_1_pioneer.png",
      "storage/graphics/sprites/el/el_1_shirt_alive.png",
```
```json
    "clothes": [
      "storage/graphics/sprites/el/el_2_pioneer.png",
      "storage/graphics/sprites/el/el_2_shirt_alive.png",
```
```json
    "clothes": [
      "storage/graphics/sprites/el/el_3_pioneer.png",
      "NONE",
```

**offset**:
```json
    "offset": "44% 16%",
```
Поле, определяющее смещение иконок в меню выбора эмоций:

![image](https://user-images.githubusercontent.com/48094227/164990971-d0761358-c839-4309-af59-81ba11ed3f9e.png)

Где *44%* определяет горизонтальное смещение, *16%* - вертикальное. Связано это с тем, что персонажи имеют разный рост и для каждого необходимо подбирать индивидуальные значения.

**accessories**:
```json
    "accessories": [
      "storage/graphics/sprites/sprites_hitbox_1.png",
      "storage/graphics/sprites/cs/cs_1_glasses.png",
      "storage/graphics/sprites/cs/cs_1_sun_glasses.png",
      "storage/graphics/sprites/cs/cs_1_glasses_over.png",
      "storage/graphics/sprites/cs/cs_1_glasses_through.png",
      "storage/graphics/sprites/cs/cs_1_stethoscope.png"
    ]
```

Представляет из себя массив, в котором перечислены наборы аксессуаров персонажа. Значениями полей массива также являются прямые ссылки на изображения в репозитории, разделяющиеся запятыми.

**[Внимание!]** Если на одной из поз соответствующая одежда отсутствует, необходимо вставить на место соответствующего элемента *"hitbox"* заглушку. Внутри одного набора (массива) аксессуаров повторение одинаковых ссылок не допускается!

**В заключении**:
Внимательно проверяйте наличие всех запятых там, где это нужно и их отсутствие там, где их быть не должно. Даже если изменённые файлы будут корректными, это ни в коем случае не означает, что добавленные/изменённые персонажи обязательно будут загружены на сайт. Последние слово остаётся за разработчиком!
