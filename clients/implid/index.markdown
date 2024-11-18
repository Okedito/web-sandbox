---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Implid
layout: page
logo: yes
hs_region: eu1
#hs_portalId: 145537483
brand_domain: implid.com
main_domains:
- name: Base de connaissances / Portail Client / Pages de destination / E-mail de vente et de service client
  type: CNAME
  host: supportclients
  value: 145537483.group0.sites.hscoscdn-eu1.net
- name: Base de connaissances (Okédito)
  type: CNAME
  host: okedito.supportclients
  value: 145537483.group0.sites.hscoscdn-eu1.net
- name: Base de connaissances (Implid)
  type: CNAME
  host: implid.supportclients
  value: 145537483.group0.sites.hscoscdn-eu1.net
- name: Base de connaissances (ProBTP)
  type: CNAME
  host: probtp.supportclients
  value: 145537483.group0.sites.hscoscdn-eu1.net
#- name: Pages de destination	
#  type: CNAME
#  host: À confirmer
#  value: À confirmer
#- name: E-mail marketing (version web)
#  type: CNAME
#  host: À confirmer
#  value: À confirmer
sending_domains:
- domain:
  name: implid.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-145537483._domainkey
  dkim_main_value: implid-com.hs12a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-145537483._domainkey
  dkim_secondary_value: implid-com.hs12b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:145537483.spf01.hubspotemail.net
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