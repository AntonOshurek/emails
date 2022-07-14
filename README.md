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


* ** Если вдруг не нужна поддержка outlook - используйте фреймворк mjml**


* **Не забывайте про атрибуты title у ссылок, alt у картинок**
**Путь к картинке должен быть полный!**
```
<img src="https://serwis.geberit.pl/domcfg.nsf/logo-geberit.png?OpenImageResource" alt="logo" width="600px"/>
```

 Делайте телефон и почту - ссылками

 Писать значения цветов полностью: #ffffff вместо #fff

 Не использовать background-image, ибо outlook не поддерживает (9% поддержка outlook)

  Важно писать стили полностью (не padding: 5px 5px, а padding-top: 5px; padding-left: 5px и так далее)

Предупредить, что outlook изначально не загружает никакие фотографии, лишь по клику внутри письма

Соблюдать порог 102кб (не считая картинок) у кода письма, ибо gmail сожмет письмо