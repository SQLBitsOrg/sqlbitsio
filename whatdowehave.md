---
layout: home
title: What Do We Have
---  

<div class="container">
    <table table cellspacing=0 class="table table-striped table-hover mt-3" id="pasteventlist" width="100%">
      <thead>
        <tr>
          <th scope="col">Short Link</th>
          <th scope="col">Short Link Name</th>
          <th scope="col">Redirects To</th>
        </tr>
      </thead>
      <tbody>

        {% for post in site.posts %}
            <!-- post content here -->
        <tr>
            <td>
                <a href="https://sqlbits.io{{ post.permalink }}">
                    https://sqlbits.io{{ post.permalink }}
                </a>
            </td>
            <td>
                {{ post.permalink }}
            </td>
            <td>
                <a href="{{ post.redirect_to }}">
                    { post.redirect_to }}
                </a>
            </td>
          </tr>
        {% endfor %}
      </tbody>
    </table>
