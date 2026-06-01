---
title: Carl Software
layout: page
logo: yes
sandbox: yes
language: fr
hs_region: eu1
hs_portalId: 147990386
brand_domain: carl-software.com
#main_domains:
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
#  host: collectivites
#  value: 146037277.group0.sites.hscoscdn-eu1.net
#- name: Landing pages - validation du sous-domaine
#  type: TXT
#  host: _cf-custom-hostname.collectivites
#  value: c4d08e27-de1a-45bf-a540-74a7673146c6
#- name: Marketing email (web version)
#  type: CNAME
#  host: news
#  value: 147339785.group0.sites.hscoscdn-eu1.net
#- name: Marketing email (web version) - validation du sous-domaine
#  type: TXT
#  host: _cf-custom-hostname.news.carl-software
#  value: f165e541-d6ae-4f37-a346-45a0d477f048
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
#  name: carl-software.com
#  dkim_main_type: CNAME
#  dkim_main_host: hs1-147339785._domainkey
#  dkim_main_value: carl--software-com.hs12a.dkim.hubspotemail.net.
#  dkim_secondary_type: CNAME
#  dkim_secondary_host: hs2-147339785._domainkey
#  dkim_secondary_value: carl--software-com.hs12b.dkim.hubspotemail.net.
#  spf_type: TXT
#  spf_host: "@"
#  spf_value: include:147339785.spf05.hubspotemail.net
#  dmarc_type: TXT
#  dmarc_host: _dmarc
#  dmarc_value: v=DMARC1; p=none;
forms:
- name: Demande de contact
  id: 36a2a17b-bbc0-4280-9b11-2ba8a6b95691
#  onFormReady: function($form) { XYZ }
#  onFormSubmit: function($form) { XYZ }
#  onFormSubmitted: function($form) { XYZ }
- name: Demande de contact [CA]
  id: bc10d10e-b87c-4cbe-9e54-db883c3d5de7
- name: Deamnde de contact [EN]
  id: 4fdb914a-b15e-4f54-a1f4-1e49707e0c40
- name: Demande de contact [ES]
  id: 06631213-0455-4ca5-a82e-7df7370f99b0
- name: Demande de contact [DL]
  id: 25fcea12-5651-4e01-bcc4-9eb124b8337c
- name: Demande de contact [IT]
  id: 000403c5-f2cf-4edd-a2c9-750349c33668
- name: Demande de contact [NL]
  id: 6aad57e2-d18a-4daf-afa6-62d2d7fbf0bb
#new_forms:
#- name: 
#  id: 
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