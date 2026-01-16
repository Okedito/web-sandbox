---
title: Smartemis
layout: page
logo: yes
language: en
hs_region: eu1
hs_portalId: 147529884 #Sandbox
brand_domain: smartemis.com
#main_domains:
#- name: Website pages	
#  type: CNAME
#  host: website-page
#  value: 45847199.group49.sites.hubspot.net
#- name: Blog
#  type: CNAME
#  host: blog
#  value: 45847199.group49.sites.hubspot.net 
#- name: Landing pages	
#  type: CNAME
#  host: page
#  value: 45847199.group49.sites.hubspot.net
#- name: Marketing email (web version)
#  type: CNAME
#  host: email
#  value: 147202787.group0.sites.hscoscdn-eu1.net
#- name: Domain validation entry
#  type: TXT
#  host: _cf-custom-hostname.email
#  value: e7363864-7b3b-4ac1-97e4-4ea60de0e596
#- name: Sales & service email (tracking)
#  type: CNAME
#  host: ???
#  value: 45847199.group49.sites.hubspot.net
#- name: Knowledge base
#  type: CNAME
#  host: ???
#  value: 45847199.group49.sites.hubspot.net
#- name: Customer portal
#  type: CNAME
#  host: ???
#  value: 45847199.group49.sites.hubspot.net
#- name: Podcast
#  type: CNAME
#  host: ???
#  value: 45847199.group49.sites.hubspot.net
#- name: Quotes
#  type: CNAME
#  host: quotes
#  value: 45847199.group49.sites.hubspot.net
#- name: Meetings scheduler
#  type: CNAME
#  host: meetings
#  value: 45847199.group49.sites.hubspot.net
#sending_domains:
#- domain:
#  name: tradelios.com
#  dkim_main_type: CNAME
#  dkim_main_host: hs1-147202787._domainkey
#  dkim_main_value: tradelios-com.hs04a.dkim.hubspotemail.net.
#  dkim_secondary_type: CNAME
#  dkim_secondary_host: hs2-147202787._domainkey
#  dkim_secondary_value: tradelios-com.hs04b.dkim.hubspotemail.net.
#  spf_type: TXT
#  spf_host: "@"
#  spf_value: include:147202787.spf04.hubspotemail.net
#  dmarc_type: TXT
#  dmarc_host: _dmarc
#  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name: 
#  occurence: first
#  script: ""
forms:
- name: Germany - Kontaktformular
  id: 518f1791-e6f7-4edb-a553-fd5f56249ad8
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