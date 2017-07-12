{% extends "extends/simple.html" %}
{% include "macro/macro.html" %}

{% set subject   = 'Тема письма' %}
{% set preheader = 'Текст прехедера' %}

# Привет!

Ваш адрес был указан при регистрации на сайте [SiteName](https://example.com/)!. Это несомненно, были вы!

Отлично, следующий шаг - подтвердить регистрацию. Жмакните на кнопку ниже!

{{ button('Подтвердить', 'https://example.com/') }}
