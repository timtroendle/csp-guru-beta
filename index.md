---
layout: home
---

<table>
    <caption>This is the data</caption>
    <thead>
        <tr>
            <td>Country code</td>
            <td>electricity demand [TWh/a]</td>
        </tr>
    </thead>
    <tbody>
    {% for demand in site.data.demand %}
        <tr>
            <td>{{ demand.id }}</td>
            <td>{{ demand.demand_twh_per_year }}</td>
        </tr>
    {% endfor %}
    </tbody>
</table>
