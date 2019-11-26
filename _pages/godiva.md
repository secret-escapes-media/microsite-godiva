---
layout: default
id: godiva
title: Godiva
nav: true
nav-order: 2
intro: Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste repellendus molestias, nulla sint reiciendis cupiditate eius ea, ipsa magnam, nisi culpa explicabo! Eos, voluptatibus nulla! Recusandae harum tenetur laudantium nihil earum veniam quo, iusto cumque debitis quidem rem vel libero?

features:

  - id: #
    title: Lorem ipsum dolor sit amet consectetur
    description: Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolorem sequi quos, minima corporis harum eius modi reiciendis ipsam natus ex maiores explicabo voluptatibus fugit impedit itaque. Fugit, sequi vero impedit nam expedita quibusdam exercitationem esse voluptatum cumque, quam veritatis reprehenderit inventore vitae officiis laborum omnis ratione error ut, autem consectetur.

  - id: #
    title: Lorem ipsum dolor sit amet consectetur
    description: Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolorem sequi quos, minima corporis harum eius modi reiciendis ipsam natus ex maiores explicabo voluptatibus fugit impedit itaque. Fugit, sequi vero impedit nam expedita quibusdam exercitationem esse voluptatum cumque, quam veritatis reprehenderit inventore vitae officiis laborum omnis ratione error ut, autem consectetur.

  - id: #
    title: Lorem ipsum dolor sit amet consectetur
    description: Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolorem sequi quos, minima corporis harum eius modi reiciendis ipsam natus ex maiores explicabo voluptatibus fugit impedit itaque. Fugit, sequi vero impedit nam expedita quibusdam exercitationem esse voluptatum cumque, quam veritatis reprehenderit inventore vitae officiis laborum omnis ratione error ut, autem consectetur.
---

<div class="container vpad--xxl">
  <div class="width width--xl text--center">
    <p class="text--xxl">{{page.intro}}</p>
    <div class="space--sm"></div>
    <a href="{{site.client.link}}" class="btn btn--outline btn--outline-orange">See all products</a>
  </div>
  <div class="space--xxxl">
    {% for item in page.features %}
      <div class="bob{% cycle '', ' bob--swap' %}">
        <div class="bob__img">
          <div class="bg-img bg-img--4-3" style="background-image: url('{{site.img}}/img.jpg');">
            <a href="{{site.client.link}}" class="bg-img__link"></a>
          </div>
        </div>
        <div class="bob__text">
          <h2 class="title title--sm">{{item.title}}</h2>
          <p class="text--xl">{{item.description | truncatewords: 35}}</p>
          <div class="space--sm"></div>
          <a href="{{site.client.link}}" class="btn btn--sm btn--outline btn--outline-orange">Find out more</a>
        </div>
      </div>
    {% endfor %}
  </div>
  <div class="text--center">
    <div class="space--xxl"></div>
    <a href="{{site.client.link}}" class="btn btn--lg btn--outline btn--outline-orange">See all products</a>
  </div>
</div>