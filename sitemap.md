---
permalink: "sitemap.xml"
---

<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  {%- for item in collections.all %}
    {%- unless item.data.ignore == true %}
      <url>
        <loc>https://www.mattakumar.com/thought{{ item.url }}</loc>
        <lastmod>{{ item.date | date: '%Y-%m-%d' }}</lastmod>
      </url>
    {%- endunless %}
  {%- endfor %}
</urlset>
