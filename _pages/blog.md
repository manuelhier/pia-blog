---
layout: page 
title: Blog
permalink: /    # Make blog default page until index has been improved
heading: false
published: true
nav: false
---

## // Willkommen auf meinem Blog 🌏

Ich bin Pia und mache für 11 Monate einen **Internationalen Freiwilligendienst (IJFD)** auf den **Philippinen**. Gemeinsam mit sechs weiteren Freiwilligen arbeite ich bei **Christ for Asia**, einer christlichen Wohltätigkeitsorganisation, die sich für Kinder in Not einsetzt.

Unsere Aufgaben sind vielfältig – vom **Kinderheim** über die **Schule** bis hin zu **praktischen Projekten** im Alltag. Wenn du mehr über den Freiwilligendienst oder unser Leben hier erfahren möchtest, bist du hier genau richtig!

Ich werde versuchen, mich regelmäßig zu melden und über unsere Erlebnisse, Eindrücke und das Leben auf den Philippinen zu berichten. Schön, dass du vorbeischaust! 🇵🇭

## // Meine Beiträge

<ul class="post-list">
  {%- for post in site.posts -%}
    <li>
        {%- assign date_format = site.minima.date_format | default: "%d.%m.%Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
            <a class="post-link" href="{{ post.url | relative_url }}">
                {{ post.title | escape }}
            </a>
        </h3>
      {% if post.description | default: '' | strip != '' %}
        <p>{{ post.description }}</p>
      {% else %}
        <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
      {% endif %}
    </li>
  {%- endfor -%}
</ul>



