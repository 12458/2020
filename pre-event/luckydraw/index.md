---
layout: default
---


# Lucky draw

Are you feeling lucky? Participants earn chances to win in regular lucky dips by participating in the various BuildingBloCS activities such as Coursemology, DataCamp, games, workshops and more. The more you participate, the luckier you get! And it is not only about prizes, you learn Computing knowledge and skills while we conduct our lucky draws too!

>Lucky draws will take place every Friday at **12 20 pm**

Do visit [classdo.com](https://classdo.com) and witness the lucky draw unfold.


## Source code

To ensure the equalness for every participant, we have decided to share the source code of the 'lucky generator' with all of you.

<a class="btn" href="https://github.com/buildingblocs/2019/blob/master/luckydraw.py">View Code</a>

## Result
{% for week in site.data.awards %}
<h3>Lucky Draw {{ week.week }}</h3>
<a class="btn" href="{{ site.baseurl }}/pre-event/luckydraw/video#{{week.week}}">Video</a>
<table>
    {% for awards in week.awards %}
    <tr>
        <td width="40%">{{ awards.prize }}</td>
        <td width="60%">{{ awards.winner }}</td>
    </tr>
    {% endfor %}
</table>
{% endfor %}


