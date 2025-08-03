---
title: Easia Travel
layout: page
logo: yes
language: en
hs_region: na1
hs_portalId: 45847199
brand_domain: easia-travel.com
main_domains:
- name: Website pages	
  type: CNAME
  host: website-page
  value: 45847199.group49.sites.hubspot.net
- name: Blog
  type: CNAME
  host: blog
  value: 45847199.group49.sites.hubspot.net 
- name: Landing pages	
  type: CNAME
  host: page
  value: 45847199.group49.sites.hubspot.net
- name: Marketing email (web version)
  type: CNAME
  host: campaign
  value: 45847199.group49.sites.hubspot.net
- name: Sales & service email (tracking)
  type: CNAME
  host: ???
  value: 45847199.group49.sites.hubspot.net
- name: Knowledge base
  type: CNAME
  host: ???
  value: 45847199.group49.sites.hubspot.net
- name: Customer portal
  type: CNAME
  host: ???
  value: 45847199.group49.sites.hubspot.net
- name: Podcast
  type: CNAME
  host: ???
  value: 45847199.group49.sites.hubspot.net
- name: Quotes
  type: CNAME
  host: quotes
  value: 45847199.group49.sites.hubspot.net
- name: Meetings scheduler
  type: CNAME
  host: meetings
  value: 45847199.group49.sites.hubspot.net
sending_domains:
- domain:
  name: easia-active.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-45847199._domainkey
  dkim_main_value: easia--active-com.hs11a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-45847199._domainkey
  dkim_secondary_value: easia--active-com.hs11b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:45847199.spf10.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
- domain:
  name: easia-exclusive.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-45847199._domainkey
  dkim_main_value: easia--exclusive-com.hs11a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-45847199._domainkey
  dkim_secondary_value: easia--exclusive-com.hs11b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:45847199.spf10.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
- domain:
  name: easia-incentive.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-45847199._domainkey
  dkim_main_value: easia--incentive-com.hs11a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-45847199._domainkey
  dkim_secondary_value: easia--incentive-com.hs11b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:45847199.spf10.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
- domain:
  name: easia-travel.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-45847199._domainkey
  dkim_main_value: easia--travel-com.hs11a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-45847199._domainkey
  dkim_secondary_value: easia--travel-com.hs11b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:45847199.spf10.hubspotemail.net
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