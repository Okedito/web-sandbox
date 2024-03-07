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
- name: Support form - English
  id: 6af8285d-1ab2-4815-b03f-ce97fde5d4bb
  onFormReady:
  onFormSubmit:
  onFormSubmitted:
- name: Support form - Français
  id: 6945ba29c-238a-418c-b946-13a0eff1ad35
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
