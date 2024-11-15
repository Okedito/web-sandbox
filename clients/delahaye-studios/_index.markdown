---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Delahaye Studios
layout: page
logo: yes
hs_region: eu1
hs_portalId: 143362522
brand_domain: delahayestudio.com
#ctas:
#- name:
#  occurence: first
#  script:
#forms:
#- name: 
#  id: 
#  onFormReady:
#  onFormSubmit:
#  onFormSubmitted:
---

{%- include section-introduction.html -%}

{% if page.hs_portalId %}
    {%- include section-tracking-code.html -%}
{% endif %}

{% if page.main_domains %}
    {%- include section-domains-main.html -%}
{% endif %}

{% if page.sending_domains %}
    {%- include section-domains-sending.html -%}
{% endif %}

{% comment %}
{% if page.ctas %}
    {%- include section-ctas.html -%}
{% endif %}
{% endcomment %}

{% if page.forms %}
    {%- include section-forms-v2.html -%}
{% endif %}