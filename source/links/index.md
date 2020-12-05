---
title:
date: 2020-11-23 17:46:11
type: "links"
---
# How to request a link exchange
1.Add a link on your site for my blog.
2.Email to <admin@kamisu66.com> with you name, avatar, site, info.
For example:
name: Miracles, Magic. They are real.
avatar: https://www.kamisu66.com/images/kashiwada_agadgqadvjaniq.png
site: https://www.kamisu66.com/
info: 一切价值源于生命给予的定义，生命本身为最高价值。
I am developing the feature of optimising for the SEO of any exchanged links in this site but it will take sometime!
*****
<div id="links">
<div class="links-content">
<div class="link-navigation">
{% for link in site.data.links %}
<div class="card">
  <a href="{{ link.site }}" target="_blank">
  <img class="ava" src="{{ link.avatar }}"/></a>
  <div class="card-header">
  <div><a href="{{ link.site }}" target="_blank">{{ link.name }}</a>
  <a href="{{ link.site }}"></a></div>
  <div class="info" title="{{ link.info }}">{{ link.info }}</div>
  </div>
</div>
{% endfor %}
</div>
</div>
</div>