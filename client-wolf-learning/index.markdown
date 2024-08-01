---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Wolf Learning Consulting
layout: page
logo: yes
hs_region: eu1
hs_portalId: 143984062
ctas:
- name:
  occurence: first
  script:
forms:
- name: Formulaire - Contact | EN
  id: d637367b-8d08-47af-b387-e5251c9b9084
  onFormReady:
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire - Contact | FR
  id: e7766694-93ef-4b85-9302-6bb1473b0462
  onFormReady:
  onFormSubmit:
  onFormSubmitted:
---

{%- include section-introduction.html -%}

{% if page.hs_portalId %}
    {%- include section-tracking-code.html -%}
{% endif %}

{% if page.forms %}
    {%- include section-forms-cimalpes.html -%}
{% endif %}