---
title: Les Chalets Covarel
layout: page
logo: yes
sandbox: no
language: fr
hs_region: eu1
hs_portalId: 148534280 #Production
brand_domain: chalets-de-valdisere.com
main_domains:
#- name: Website pages	
#  type: CNAME
#  host: website-page
#  value: 
#- name: Blog
#  type: CNAME
#  host: blog
#  value: 
#- name: Landing pages	
#  type: CNAME
#  host: 
#  value: 
#- name: Landing pages - validation du sous-domaine
#  type: TXT
#  host: 
#  value: 
#- name: Marketing email (web version)
#  type: CNAME
#  host: mail
#  value: 
#- name: Marketing email (web version) - validation du sous-domaine
#  type: TXT
#  host: 
#  value: 
#- name: Sales & service email (tracking)
#  type: CNAME
#  host: ???
#  value: 
#- name: Knowledge base
#  type: CNAME
#  host: ???
#  value: 
#- name: Customer portal
#  type: CNAME
#  host: ???
#  value: 
#- name: Podcast
#  type: CNAME
#  host: ???
#  value: 
#- name: Quotes
#  type: CNAME
#  host: quotes
#  value: 
#- name: Meetings scheduler
#  type: CNAME
#  host: meetings
#  value: 25027870.group0.sites.hscoscdn-eu1.net
#- name: Meetings scheduler - validation du sous-domaine
#  type: TXT
#  host: _cf-custom-hostname.meetings
#  value: ce4d6dd5-42c4-4962-b04d-04a3e7232da0
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
#  spf_host: 
#  spf_value: 
#  dmarc_type: TXT
#  dmarc_host: _dmarc
#  dmarc_value: v=DMARC1; p=none;
forms:
- name: Formulaire de contact (legacy)
  id: 665aa003-75dc-472a-9456-d278a400d3d4
#  onFormReady: function($form) { XYZ }
#  onFormSubmit: function($form) { XYZ }
#  onFormSubmitted: function($form) { XYZ }
new_forms:
- name: Formulaire de contact
  id: f692b62d-807d-49e5-a42e-dfb00918f485
#ctas:
#- name: EN - Download Whitepaper
#  occurence: first
#  script: ""
---
{%- include section-introduction.html -%}

{% if page.hs_portalId %}
    {%- include section-tracking-code-v2.html -%}
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

{% if page.new_forms %}
    {%- include section-new-forms-v1.html -%}
{% endif%}

{% if page.forms %}
    {%- include section-forms-v2.html -%}
{% endif %}

{% if page.ctas %}
    {%- include section-ctas-v2.html -%}
{% endif %}