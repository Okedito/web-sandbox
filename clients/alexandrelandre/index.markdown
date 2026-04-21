---
title: Alexandre Landre
layout: page
logo: yes
sandbox: no
language: fr
hs_region: eu1
hs_portalId: 146711514
brand_domain: alexandrelandre.com
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
#  host: info
#  value: 
#- name: Landing pages - domain validation entry
#  type: TXT
#  host: _cf-custom-hostname.info
#  value: 
#- name: Marketing email (web version)
#  type: CNAME
#  host: email
#  value: 
#- name: Marketing email (web version) - domain validation entry
#  type: TXT
#  host: _cf-custom-hostname.email
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
#- name: Meetings scheduler - domain validation entry
#  type: TXT
#  host: _cf-custom-hostname.meetings
#  value: ce4d6dd5-42c4-4962-b04d-04a3e7232da0
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
#- name: 
#  id: 
#  type: pop-up
#- name: 
#  id: 
#  type: embedded
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

<!-- Start of HubSpot Embed Code -->
<script type="text/javascript" id="hs-script-loader" async defer src="//js-eu1.hs-scripts.com/146711514.js"></script>
<!-- End of HubSpot Embed Code -->