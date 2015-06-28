---
layout: post
title: Adding Reading Time 
date: 2015-06-28 10:40:42
---

To add a reading time to your Jekyll post just add this code in your post layout:


{% highlight html %}
{% raw %}
{% if page.minutes %}
  {% assign minutes = page.minutes %}
{% else %}
  {% assign minutes = content | number_of_words | divided_by: 180 %}
  {% if minutes == 0 %}{% assign minutes = 1 %}{% endif %}
{% endif %}

{% if minutes == 1 %}
 <span class="post-meta small">{{ minutes }} minute read</span>
 {% else %}
 <span class="post-meta small">{{ minutes }} minutes read</span>
 {% endif %}
{% endraw %}
 {% endhighlight %}
}

Lorem ipsum Nostrud sed commodo sed quis id eu dolor ea laborum nisi laboris occaecat ullamco enim aliquip pariatur nisi tempor et id consectetur aliquip fugiat adipisicing dolore voluptate anim reprehenderit eiusmod ut mollit quis velit eiusmod Duis id eiusmod exercitation esse laborum et exercitation est tempor tempor mollit dolor aute mollit ea voluptate tempor eiusmod deserunt dolore nisi veniam fugiat consequat dolor pariatur aliquip elit Duis et aliqua id ex qui minim esse ut deserunt ea in in incididunt Ut dolor ea do enim pariatur dolor exercitation sed mollit consectetur reprehenderit ea sint eiusmod laboris incididunt reprehenderit in nostrud qui mollit occaecat nulla consectetur incididunt laborum fugiat nostrud ut esse proident magna dolore irure dolore deserunt velit ut ut sint cillum consectetur mollit ea aute nisi officia in sint qui aute nostrud id mollit sunt dolore cillum aliquip amet aute labore veniam ea occaecat tempor dolore mollit ullamco eu tempor ut pariatur et velit elit dolore veniam reprehenderit do aliquip velit consectetur velit aute velit elit Ut dolore cupidatat quis labore velit id sed pariatur laboris commodo commodo deserunt laboris exercitation voluptate aliquip cupidatat elit reprehenderit occaecat est veniam cupidatat voluptate est consectetur ullamco consequat dolor pariatur nulla est in sint aute velit cillum dolor laborum tempor esse deserunt sed irure commodo nulla labore ex in aliquip non aute ad ut Excepteur cupidatat do incididunt ullamco nisi nulla amet consequat anim.

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo. Nullam dictum felis eu pede mollis pretium.

Lorem ipsum Dolor consectetur ad in laboris velit nostrud do fugiat enim officia sit in aliquip Duis cillum nulla Ut ex amet culpa aute ullamco nostrud incididunt occaecat cupidatat elit in qui amet ad esse occaecat qui adipisicing Duis velit consectetur mollit deserunt laborum incididunt dolor anim veniam ullamco ut elit ullamco proident dolor proident nostrud in in nulla amet in proident proident velit velit aute enim dolor in cupidatat in veniam cupidatat fugiat do sit dolor tempor reprehenderit nostrud aliquip veniam consectetur qui cupidatat adipisicing sunt in esse consectetur consequat cupidatat quis in consequat id est in commodo enim officia qui deserunt velit Excepteur Duis ut proident cupidatat in laboris consequat dolore do ex est dolor in eiusmod in eiusmod deserunt minim laboris cillum sint sed labore dolor aute dolore enim reprehenderit adipisicing adipisicing dolore aliquip enim tempor commodo ad sint est et aliqua enim reprehenderit dolore dolor ad exercitation ut consectetur sit ex consequat laboris labore ad voluptate aliquip magna consectetur magna minim proident officia officia dolore ullamco laborum ad qui proident nostrud sit occaecat pariatur sit Excepteur proident et ullamco dolore mollit anim.