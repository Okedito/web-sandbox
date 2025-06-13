---
title: Memmert
layout: page
logo: yes
language: en
hs_region: eu1
hs_portalId: 145850363
brand_domain: memmert.com
main_domains:
- name: All marketing content types
  type: CNAME
  host: info.frmce
  value: 145850363.group0.sites.hscoscdn-eu1.net
- name: Quotes
  type: CNAME
  host: quotes.frmce
  value: 145850363.group0.sites.hscoscdn-eu1.net
- name: Meetings
  type: CNAME
  host: meetings.frmce
  value: 145850363.group0.sites.hscoscdn-eu1.net
- name: Email
  type: CNAME
  host: email.frmce
  value: 145850363.group0.sites.hscoscdn-eu1.net
sending_domains:
- domain:
  name: memmert.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-145850363._domainkey
  dkim_main_value: memmert-com.hs19a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-145850363._domainkey
  dkim_secondary_value: memmert-com.hs19b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:145850363.spf07.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name: 
#  occurence: first
#  script: ""
forms:
- name: Basic contact form
  id: 3407db41-e4ec-46ec-a6ea-a61757d9d6e4
#  onFormReady: ""
#  onFormSubmit: ""
#  onFormSubmitted: ""
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

{% if page.ctas %}
    {%- include section-ctas.html -%}
{% endif %}

{% if page.forms %}
    {%- include section-forms-v2.html -%}
{% endif %}