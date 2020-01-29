---
layout: default
id: products
title: Products
permalink: /products/
nav: true
nav-order: 2
intro: Immerse yourself in a world of wonder with the finest bites of chocolate, designed to make special moments even sweeter. Make your world more wonderful with treats that promise moments of unmissable delight. Treat yourself to the handcrafted flavours of the Masterpieces Collection and discover a world of wonder...

features:

  - id: masterpieces
    title: Masterpieces
    description: Treat yourself to the best. The Godiva Masterpieces Collection is the signature selection of only the most indulgent Godiva offerings. From dark chocolate filled with a rich ganache to chocolate hazelnut oysters, each is individually wrapped for those moments when you need something a little special.

  - id: heritage
    title: The Godiva Story
    description: Nothing is more synonymous with fine chocolate than Belgium, and it’s there that the Godiva story started. Since 1926, Godiva master chocolatiers have been crafting deliciously rich, smooth chocolate using only the finest ingredients, set to delight and indulge the senses.
    link: https://www.godivachocolates.co.uk/history-of-godiva


products:

  - id: caramel-lion
    title: Caramel Lion with Belgian Milk Chocolate
    link: https://www.ocado.com/products/godiva-masterpieces-milk-chocolate-caramel-lion-bar-418397011

  - id: ganache-heart
    title: Ganache Heart with Belgian Dark Chocolate
    link: https://www.ocado.com/products/godiva-masterpieces-dark-chocolate-ganache-heart-bar-418395011

  - id: crispy-hazelnut
    title: Crispy Hazelnut Chocolate Domes
    link: https://www.ocado.com/products/godiva-domes-milk-chocolate-hazelnut-447212011

  - id: milk-caramel-lion
    title: Milk Chocolate Caramel Lion of Belgium
    link: https://www.ocado.com/products/godiva-masterpieces-milk-chocolate-caramel-lion-bar-418396011

  - id: raspberry-crunch
    title: Raspberry Crunch Chocolate Domes
    link: https://www.ocado.com/products/godiva-domes-dark-chocolate-raspberry-447210011

  - id: caramel-lion-with-belgian-milk-chocolate
    title: Caramel Lion with Belgian Milk Chocolate
    link: https://www.ocado.com/products/godiva-masterpieces-milk-chocolate-caramel-lion-assortment-418392011
---

<div class="container vpad--xxl">
  <div class="width width--xl text--center">
    <p class="text--xxl">{{page.intro}}</p>
    <div class="space--sm"></div>
    <a href="{{site.client.link}}" class="btn btn--lg btn--red js-open-modal" data-open-modal="shops">Shop Godiva Now</a>
  </div>
  <div class="space--xxxl">
    {% for item in page.features %}
      <div class="bob{% cycle '', ' bob--swap' %}">
        <div class="bob__img">
          <div class="bg-img bg-img--4-3 bg-img--border" style="background-image: url('{{site.img}}/content/{{page.id}}/{{item.id}}.jpg');">
            {% if item.id == 'masterpieces' %}
              <a href="{% if item.link %}{{item.link}}{% else condition %}{{site.client.link}}{% endif %}" class="bg-img__link js-open-modal" data-open-modal="shops"></a>
            {% else %}
              <a id="track-{{page.id}}-{{item.id}}-img" href="{% if item.link %}{{item.link}}{% else condition %}{{site.client.link}}{% endif %}" class="bg-img__link"></a>
            {% endif %}
          </div>
        </div>
        <div class="bob__text">
          <h2 class="title title--sm">{{item.title}}</h2>
          <p class="text--xl">{{item.description}}</p>
          <div class="space--sm"></div>
          {% if item.id == 'masterpieces' %}
            <a href="{% if item.link %}{{item.link}}{% else condition %}{{site.client.link}}{% endif %}" class="btn btn--sm btn--outline btn--outline-red js-open-modal" data-open-modal="shops">Shop Now</a>
          {% else %}
            <a id="track-{{page.id}}-{{item.id}}-btn" href="{% if item.link %}{{item.link}}{% else condition %}{{site.client.link}}{% endif %}" class="btn btn--sm btn--outline btn--outline-red">Find out more</a>
          {% endif %}
        </div>
      </div>
    {% endfor %}
  </div>
</div>

<div class="bg--light">
  <div class="container vpad--xxl">
    <div class="text--center">
      <h2 class="title title--md">latest products</h2>
    </div>
    <div class="space--lg"></div>
    <div class="width width--xl">
      <div class="row row--md-6-6 row--xl-4-4-4 row--gutters-lg">
        {% for item in page.products %}
          <div class="col text--center">
            <div class="bg-img bg-img--1-1" style="background-image: url('{{site.img}}/content/{{page.id}}/{{item.id}}.jpg');">
              <a id="track-{{page.id}}-product-{{item.id}}-img" href="{{item.link}}" class="bg-img__link"></a>
            </div>
            <div class="vpad--xs text--normal">
              <h3 class="text--xxl">{{item.title}}</h3>
              <div class="space--xs"></div>
              <a id="track-{{page.id}}-product-{{item.id}}-btn" href="{{item.link}}" class="btn btn--outline btn--outline-red btn--sm">Shop Now</a>
            </div>
          </div>
        {% endfor %}
      </div>
    </div>
    <div class="space--xxl"></div>
    <div class="text--center">
      <a href="{{site.client.link}}" class="btn btn--lg btn--red js-open-modal" data-open-modal="shops">Shop Godiva Now</a>
    </div>
  </div>
</div>