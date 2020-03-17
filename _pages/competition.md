---
layout: competition
id: competition
permalink: /competition/
nav: true
nav-order: 3

banner:
  image: bg.jpg

title: Compet&shy;ition
long-title: Win a delicious escape to Belgium
intro: Win a grand two-night getaway to Brussels, staying in the well-appointed, five-star Steigenberger Wiltcher's. Located in the heart of the city, wake up for breakfast before strolling the magnificent boulevards of this stylish destination, unpicking the medieval old town, the boutiques and cultural curiosities that hide within. On your return, enjoy a sumptuous evening in the hotel’s esteemed restaurant, indulging in exceptional cooking. If that wasn’t sweet enough, you’ll also be treated to a hamper bursting with a choice selection of Godiva’s gorgeous chocolates. Enter now for a truly delicious getaway.

enter-cta: Enter Now

competition-form:
  id: comp
  post-url: https://getform.io/f/45369df2-96d3-40d0-8ba1-2b871d001844
  expiry-date: 2020-04-16
  fields:
    - id: name
      type: text
      label: Name
      required: true
    - id: email
      type: email
      label: Email
      required: true
    - id: qualify
      type: radio
      label: Are you a UK resident and over the age of 18?
      required: true
      options:
        - id: qualify-true
          label: 'Yes'
          value: 'yes'
        - id: qualify-false
          label: 'No'
          value: 'no'
          invalid: true
    - id: opt-in
      type: radio
      label: Would you like to receive emails from Godiva?
      required: true
      options:
        - id: opt-in-true
          label: 'Yes'
          value: 'yes'
        - id: opt-in-false
          label: 'No'
          value: 'no'
  submit: Submit Entry
  terms: >
    By submitting your entry, you agree to the <a href="#" class="js-open-modal link--underlined" data-open-modal="competition-terms">terms and conditions</a> of this competition
---