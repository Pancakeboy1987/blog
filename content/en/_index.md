---
title: ""
date: 2022-10-24
type: landing

content:
  - block: hero  # Добавьте этот блок для заголовка
    content:
      title: "Добро пожаловать на мой сайт"
      image:
        filename: hero-academic.png
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true

  - block: about.avatar
    id: about
    content:
      username: admin  # Обязательно создайте этого автора
      text: |-
        Здесь напишите вашу биографию...
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      background:
        color: black
        image:
          filename: stacked-peaks.svg
          size: cover
          position: center

  - block: features  # Добавьте блок с вашими навыками
    content:
      title: Навыки
      items:
        - name: Python
          description: 90%
          icon: python
          icon_pack: fab
        - name: Data Science
          description: 100%
          icon: chart-line
          icon_pack: fas
        - name: Photography
          description: 10%
          icon: camera-retro
          icon_pack: fas

  - block: experience  # Добавьте блок с опытом работы
    content:
      title: Опыт работы
      items:
        - title: Профессор
          company: Университет X
          location: Калифорния
          date_start: '2018-01-01'
          date_end: ''
          description: |2-
              Обязанности:

              * Преподавание
              * Исследования
              * Публикации

        - title: Доцент
          company: Университет Y
          location: Орегон
          date_start: '2016-01-01'
          date_end: '2017-12-31'
    design:
      columns: '2'

  - block: collection  # Публикации
    id: featured
    content:
      title: Избранные публикации
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: card
      columns: '2'

  # Остальные блоки из вашего исходного файла...
  - block: collection
    content:
      title: Последние публикации
      filters:
        folders:
          - publication
    design:
      view: citation
      columns: '2'

  - block: collection
    id: talks
    content:
      title: Доклады и выступления
      filters:
        folders:
          - event
    design:
      view: compact
      columns: '2'

  - block: contact  # Добавьте блок контактов
    id: contact
    content:
      title: Контакты
      email: your-email@example.com
      phone: 888 888 88 88
      address:
        street: 450 Serra Mall
        city: Stanford
        region: CA
        postcode: '94305'
        country: United States
        country_code: US
    design:
      columns: '2'
---
