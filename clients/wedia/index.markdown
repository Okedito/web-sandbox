---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Wedia
layout: page
logo: yes
hs_region: eu1
hs_portalId: 144852889
#ctas:
#- name:
#  occurence: first
#  script:
#forms:
#- name: Formulaire Contact - SAP
#  id: 89ffb57c-af22-4b9f-8b74-853bdf8bd911
#  onFormReady:
#  onFormSubmit:
#  onFormSubmitted:
---

{%- include section-introduction.html -%}

{% if page.hs_portalId %}
    {%- include section-tracking-code.html -%}
{% endif %}

{% comment %}
{% if page.ctas %}
    {%- include section-ctas.html -%}
{% endif %}
{% endcomment %}

{% if page.forms %}
    {%- include section-forms-cimalpes.html -%}
{% endif %}