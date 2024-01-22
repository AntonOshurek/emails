# emails
all my email templates :)

***

# Полезные ссылки - инструменты

[Инлайнер - ](https://www.campaignmonitor.com/resources/tools/css-inliner/)

[Проверка поддержки свойств - ](https://www.caniemail.com/)

[Проверка поддержки свойств - ](https://caniuse.email/)

[Валидатор - ](https://validator.w3.org/)

[Тесты - ](https://putsmail.com/) и [ещё тут](www.emailonacid.com)


***

# Основные правила

* **обязательный доктайп**
```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
```

* **обязательный HTML**
```
<html xmlns="http://www.w3.org/1999/xhtml">
```

* **обязательный META тег**
```
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
```

* **Для адаптивной вёрстки нужно добавить это**
```
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

* **Использовать таблицы**
```
<table cellpadding="0" cellspacing="0" width="100%" bgcolor="#00abdf"> 
```

* **Используйте valign и align**
```
<td align="left">
```

* **Прописывать шрифты в теге с текстом**
```
<p style="font-family: Arial, Helvetica, sans-serif, 'Railway';">Dzień dobry</p>
```

* **Не использовать вебшрифты, только безопасные**
[Безопасные шрифты тут, по ссылке](https://websitesetup.org/web-safe-fonts-html-css/)

* **Не забывайте про атрибуты title у ссылок, alt у картинок**
**Путь к картинке должен быть полный!**
```
<img src="https://serwis.geberit.pl/domcfg.nsf/logo-geberit.png?OpenImageResource" alt="logo" width="600px"/>
```

* **Закрывать тег br**
```
<br />
```

* **Делайте телефон и почту - ссылками**
```
<a class="copyright--link" href="www.geberit.pl" style="font-family: Arial, Helvetica, sans-serif, 'Railway'; color: #ffffff;">
    www.geberit.pl
</a>
```

* **Писать значения цветов полностью: #ffffff вместо #fff**
**Не забывать добавлять !important**
```
.copyright {
    color: #ffffff !important;
}
```

* **Стили можно писать в style**
**Потом использовать инлайнер стилей, большинство клиентов не поддерживает <style>**
*Ниже приведён пример со стандартными стилями которые лучше использовать в каждом письме.*
*Так называемые обнуляющие стили*
```
    <style type="text/css">
        body {
            width: 100% !important;
            -webkit-text-size-adjust: 100%;
            -ms-text-size-adjust: 100%;
            margin: 0;
            padding: 0;
            line-height: 100%;
        }
        table {
			border-collapse: collapse;
			mso-table-lspace: 0pt;
			mso-table-rspace: 0pt;
		}
        table td {
			border-collapse: collapse;
		}
    </style>
```

* **Медиа можно писать в теге style, потом их инлайнить через инлайнер**
```
    @media (max-width: 700px) {
      .table-600 {
        width: 500px !important;
      }

      .table-500-inner {
        width: 400px !important;
      }
    }
```

* **Стили для изображений**
```
    img {
        outline: none;
        text-decoration: none;
        border:none;
        -ms-interpolation-mode: bicubic;
        max-width: 100%!important;
        margin: 0;
        padding: 0;
        display: block;
    }
```

* **border-radius не работает в outlook**
нужно вставлять закруглённые края картинкой или же обходиться без них.

* **margin в большинстве клиентах не работает**
От margin лучше отказаться и использовать padding. 
Так же, нужно учитывать что у текстовых элементов ```<span> <p> <div> ...``` не должно быть отступов!
Padding задаём только табличному тегу ```<td>```

**Не использовать background-image, ибо outlook не поддерживает (9% поддержка outlook)**

**Важно писать стили полностью (не padding: 5px 5px, а padding-top: 5px; padding-left: 5px и так далее)**
```
.table-info {
    padding-top: 40px;
    padding-left: 20px;
    padding-right: 20px;
    padding-bottom: 50px;
    border-radius: 10px;
}
```

**Предупредить, что outlook изначально не загружает никакие фотографии, лишь по клику внутри письма**
**Соблюдать порог 102кб (не считая картинок) у кода письма, ибо gmail сожмет письмо**
