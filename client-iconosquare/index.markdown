---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Iconosquare
layout: page
logo: yes
hs_region: eu1
hs_portalId: 143669362
ctas:
- name:
  occurence: first
  script:
forms:
- name:
  id:
  onFormReady:
  onFormSubmit:
  onFormSubmitted:
---

{%- include section-introduction.html -%}

{% if page.hs_portalId %}
    {%- include section-tracking-code.html -%}
{% endif %}
