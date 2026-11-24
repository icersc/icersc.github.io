---
title: Steering Committee
nav_order: 2
---

# Steering Committee

<table class="committee-table">
  <thead>
    <tr><th>Name</th><th>Role</th><th>Affiliation</th><th>Term</th></tr>
  </thead>
  <tbody>
  {% for m in site.data.committee %}
    <tr>
      <td>{{ m.name }}</td>
      <td>{{ m.role }}</td>
      <td>{{ m.affiliation }}</td>
      <td>{{ m.term }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>

To contact the committee, see [Contact](contact).
