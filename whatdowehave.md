---
layout: home
title: What Do We Have
---  
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-lhfm{background-color:#cbcefb;border-color:#340096;color:#333333;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
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
                    <a href="https://sqlbits.io{{ post.redirect.from }}">
                        https://sqlbits.io{{ post.redirect.from }}
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

