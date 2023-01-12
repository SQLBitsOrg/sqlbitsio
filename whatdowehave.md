---
layout: home
title: What Do We Have
---  

<table class="tg">
<thead>
  <tr>
    <th class="tg-lhfm">Short Link</th>
    <th class="tg-lhfm">Short Link Name</th>
    <th class="tg-lhfm">Redirects To</th>
  </tr>
</thead>
<tbody>
  <tr>
      {% for post in site.pages %}
          {% if post.redirect.from  %} 
            <tr>
                <td class="tg-0lax">
                    <a href="https://sqlbits.io/{{ post.redirect.from }}">
                        sqlbits.io/{{ post.redirect.from }}
                    </a>
                </td>
                <td class="tg-0lax">
                    {{ post.redirect.from }}
                </td>
                <td class="tg-0lax">
                    <a href="{{ post.redirect.to }}">
                        {{ post.redirect.to }}
                    </a>
                </td>
              </tr>
        {% endif %}
    {% endfor %}
  </tr>
</tbody>
</table>

