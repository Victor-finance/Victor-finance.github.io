---
layout: page
permalink: /publications/
title: Research+
description: 
nav: true
nav_order: 2
---


{% include bib_search.liquid %}

## Peer-Reviewed Journal Articles

<div class="publications">
{% bibliography --query @article %}
</div>

---

## Working Papers

<div class="publications">
{% bibliography --query @unpublished %}
</div>

---

## Work in Progress

<div class="publications">
{% bibliography --query @misc %}
</div>

---

<script>
const authorUrls = {
  "Wang, Xingjian": "https://victor-finance.github.io",
  "Han, Haozhe": "https://come.tju.edu.cn/info/1091/7801.htm",
  "Yao, Chi": "https://www.suibe.edu.cn/finance/yc/list.htm",
  "Wang, Changyun": "http://sf.ruc.edu.cn/info/1269/8125.htm",
  "Gao, Haoyu": "https://haoyugao.top",
  "Wen, Huiyu": "https://glxy.gdut.edu.cn/info/1292/29774.htm",
  "Xu, Zelin": "https://jgxy.fzu.edu.cn/info/1043/22411.htm",
  "Ren, Xingzi": "https://jrx.cueb.edu.cn/szll/jsml/8be04f4f81144a9a926feb3e2d90aad7.htm",
  "Miao, Meng": "http://sf.ruc.edu.cn/jszy/mm/index.htm",
  "Tang, Huoqing": "https://cz.cueb.edu.cn/szdw/swx/146301.htm",
  "Zhu, Guangshun": "https://sbf.uibe.edu.cn/szdw/xyjs/jszc/4fea26058ab541eaa8d8795c05a8dfcd.htm",
  "Zhong, Teng": "https://sbf.uibe.edu.cn/szdw/xyjs/fjszc/a3139c035ed84961a9c3caa0d90eec3a.htm"
};

document.addEventListener('DOMContentLoaded', function() {
  document.querySelectorAll('.bibliography .author').forEach(function(authorDiv) {
    let html = authorDiv.innerHTML;
    Object.keys(authorUrls).forEach(function(author) {
      const regex = new RegExp(author.replace(/[.*+?^${}()|[\]\\]/g, '\\$&'), 'g');
      html = html.replace(regex, `<a href="${authorUrls[author]}" target="_blank" style="color: inherit; text-decoration: none; border-bottom: 1px dotted;">${author}</a>`);
    });
    authorDiv.innerHTML = html;
  });
});
</script>
