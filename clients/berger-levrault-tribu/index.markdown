---
title: Berger-Levrault TriBU
layout: page
logo: yes
sandbox: no
language: fr
hs_region: eu1
hs_portalId: 146037277 #Production
brand_domain: berger-levrault.com
main_domains:
#- name: Website pages	
#  type: CNAME
#  host: website-page
#  value: 
#- name: Blog
#  type: CNAME
#  host: blog
#  value: 
- name: Landing pages	
  type: CNAME
  host: collectivites
  value: 146037277.group0.sites.hscoscdn-eu1.net
- name: Landing pages - validation du sous-domaine
  type: TXT
  host: _cf-custom-hostname.collectivites
  value: c4d08e27-de1a-45bf-a540-74a7673146c6
- name: Landing pages	
  type: CNAME
  host: sante
  value: 146037277.group0.sites.hscoscdn-eu1.net
- name: Landing pages - validation du sous-domaine
  type: TXT
  host: _cf-custom-hostname.sante
  value: 7eac2c65-c644-4e21-ad3d-f6a4dcf0c64e
- name: Landing pages	
  type: CNAME
  host: edition
  value: 146037277.group0.sites.hscoscdn-eu1.net
- name: Landing pages - validation du sous-domaine
  type: TXT
  host: _cf-custom-hostname.edition
  value: c98f35ab-9a15-4cf5-bcef-623008320d1a
- name: Marketing email (web version)
  type: CNAME
  host: email
  value: 146037277.group0.sites.hscoscdn-eu1.net
- name: Marketing email (web version) - validation du sous-domaine
  type: TXT
  host: _cf-custom-hostname.email
  value: 78e837cb-e5d6-4f52-a747-7631706fb0da
- name: Marketing email (web version)
  type: CNAME
  host: mail
  value: 146037277.group0.sites.hscoscdn-eu1.net
- name: Marketing email (web version) - validation du sous-domaine
  type: TXT
  host: _cf-custom-hostname.mail
  value: c85a4c5b-ae7a-401f-8e04-c7a71cd70632
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
sending_domains:
- domain:
  name: berger-levrault.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-146037277._domainkey
  dkim_main_value: berger--levrault-com.hs11a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-146037277._domainkey
  dkim_secondary_value: berger--levrault-com.hs11b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:146037277.spf08.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
#forms:
#- name: 
#  id: 
#  onFormReady: function($form) { XYZ }
#  onFormSubmit: function($form) { XYZ }
#  onFormSubmitted: function($form) { XYZ }
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