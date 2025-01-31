---
title: KOOB
layout: page
logo: yes
hs_region: eu1
hs_portalId: 48499538
brand_domain: koob.tech
#main_domains:
#- name: Pages de destination - Global
#  type: CNAME
#  host: 
#  value: 
#- name: E-mail marketing (version web) - Global
#  type: CNAME
#  host: 
#  value: 
#sending_domains:
#- domain:
#  name: 
#  dkim_main_type: CNAME
#  dkim_main_host: 
#  dkim_main_value: 
#  dkim_secondary_type: CNAME
#  dkim_secondary_host: 
#  dkim_secondary_value: 
#  spf_type: TXT
#  spf_host: "@"
#  spf_value: 
#  dmarc_type: TXT
#  dmarc_host: _dmarc
#  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name:
#  occurence: first
#  script:
#forms:
#- name: XXX
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

{% if page.secondary_domains %}
    {%- include section-domains-secondary.html -%}
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