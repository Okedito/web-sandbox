---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Wedia
layout: page
logo: yes
hs_region: eu1
hs_portalId: 144852889
brand_domain: wedia-group.com
main_domains:
- name: Pages de destination	
  type: CNAME
  host: go
  value: 144852889.sites.hscoscdn-eu1.net
- name: E-mail marketing (version web)
  type: CNAME
  host: email
  value: 144852889.sites.hscoscdn-eu1.net
sending_domains:
- domain:
  name: wedia-group.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-144852889._domainkey
  dkim_main_value: wedia--group-com.hs07a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-144852889._domainkey
  dkim_secondary_value: wedia--group-com.hs07b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:144852889.spf06.hubspotemail.net
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
    {%- include section-forms-cimalpes.html -%}
{% endif %}