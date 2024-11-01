---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Comité interprofessionnel du vin de Champagne
layout: page
logo: yes
hs_region: eu1
hs_portalId: 144550957
brand_domain: champagne.education
main_domains:
- name: Blog	
  type: CNAME
  host: blog
  value: 144550957.group0.sites.hscoscdn-eu1.net
- name: Pages de destination	
  type: CNAME
  host: info
  value: 144550957.group0.sites.hscoscdn-eu1.net
- name: E-mail marketing (version web)
  type: CNAME
  host: email
  value: 144550957.group0.sites.hscoscdn-eu1.net
- name: Base de connaissances
  type: CNAME
  host: support
  value: 144550957.group0.sites.hscoscdn-eu1.net
- name: Portail client
  type: CNAME
  host: support
  value: 144550957.group0.sites.hscoscdn-eu1.net
sending_domains:
- domain:
  name: champagne.education
  dkim_main_type: CNAME
  dkim_main_host: hs1-144550957._domainkey
  dkim_main_value: champagne-education.hs04a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-144550957._domainkey
  dkim_secondary_value: champagne-education.hs04b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:144550957.spf03.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name:
#  occurence: first
#  script:
forms:
- name: Formulaire Ticket | FR
  id: b61c9578-bd97-48e9-81f0-2ec835d3acb0
#  onFormReady:
#  onFormSubmit:
#  onFormSubmitted:
- name: Formulaire Contact | FR
  id: c9df1441-813b-41d9-94b2-e6f547ed3d50
#  onFormReady:
#  onFormSubmit:
#  onFormSubmitted:
- name: Formulaire Newsletter | FR
  id: 72222813-344d-4d47-bc02-72393f839321
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