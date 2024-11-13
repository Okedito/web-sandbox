---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Delahaye Studios
layout: page
logo: yes
hs_region: eu1
hs_portalId: 143362522
brand_domain: delahayestudio.com
main_domains:
- name: Pages de destination	
  type: CNAME
  host: image
  value: 
- name: E-mail marketing (version web)
  type: CNAME
  host: email
  value: 
- name: Devis
  type: CNAME
  host: devis
  value: 
sending_domains:
- domain:
  name: delahayestudio.com
  dkim_main_type: CNAME
  dkim_main_host: 
  dkim_main_value: 
  dkim_secondary_type: CNAME
  dkim_secondary_host: 
  dkim_secondary_value: 
  spf_type: TXT
  spf_host: "@"
  spf_value: 
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
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