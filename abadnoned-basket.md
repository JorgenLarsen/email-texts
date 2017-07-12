{% extends "extends/ecommerce.html" %}
{% include "macro/macro.html" %}

{% set subject   = 'Тема письма' %}
{% set preheader = 'Текст прехедера' %}

{% block content %}
# Сергей, добрый день!
Вы добавили в корзину охуительные товары у нас на сайте, но нихуя не купили. Мы сохранили вашу корзину для вас.
{% endblock %}

{% block basket %}
## Ваша корзина
{{ basket() }}
{{ button('Оформить заказ', 'https://example.com/basket/') }}
{% endblock %}

{% block recs %}
## Вас может заинтересовать
{{ recs() }}
{{ button('Показать еще', 'https://example.com/popular/') }}
{% endblock %}
