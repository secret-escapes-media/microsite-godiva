---
layout: default
id: offers
title: Offers
nav: true
nav-order: 1

banner:
  content: >
    <div class="container container--xxl">
      <img class="width width--title width--left" src="{{site.img}}/content/title.svg" alt="{{site.title}}">
    </div>
---

<div class="container">
  <div class="width width--xl text--center space--xxxl">
    <p class="text--xxl">{{site.description}}</p>
    <p class="text--xxl">Choose your sumptuous escape below and we’ll sweeten your break with Godiva. Each day of your stay, you’ll find Godiva chocolates waiting for you in your room. Indulge in the handcrafted flavours of the Masterpieces Collection for a truly delicious escape.</p>
    <div class="space--sm"></div>
    <a href="{{site.client.link}}" class="btn btn--outline btn--outline-red js-open-modal" data-open-modal="shops">Shop Godiva Now</a>
  </div>
</div>

{% include offer/all-offers.html %}