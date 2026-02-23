---
title: Smartemis
layout: page
logo: yes
language: en
hs_region: eu1
#hs_portalId: 147529884 #Sandbox
hs_portalId: 25027870 #Production
brand_domain: smartemis.com
main_domains:
#- name: Website pages	
#  type: CNAME
#  host: website-page
#  value: 45847199.group49.sites.hubspot.net
#- name: Blog
#  type: CNAME
#  host: blog
#  value: 45847199.group49.sites.hubspot.net 
- name: Landing pages	
  type: CNAME
  host: info
  value: 25027870.group0.sites.hscoscdn-eu1.net
- name: Landing pages - domain validation entry
  type: TXT
  host: _cf-custom-hostname.info
  value: 9a2ed781-b21f-4961-95ef-6247afe74854
- name: Marketing email (web version)
  type: CNAME
  host: email
  value: 25027870.group0.sites.hscoscdn-eu1.net
- name: Marketing email (web version) - domain validation entry
  type: TXT
  host: _cf-custom-hostname.email
  value: eb47b72f-336d-4568-96de-6987d95eeffd
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
- name: Meetings scheduler
  type: CNAME
  host: meetings
  value: To be confirmed, once main domains have been configured
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
- name: German - Bewerberformular
  id: d1842234-7b20-4889-b59f-5efac7200ad1
#- name: French - Dummy form - Thank-you page (legacy)
#  id: 61e71be8-30ef-48fd-a208-ea29928a3635
  #onFormReady: ""
  #onFormSubmit: ""
  #onFormSubmitted: ""
new_forms:
- name: French - Gated content form proof of concept - landing page
  id: 8f8f3e12-70dd-4295-8c47-2c327126addd
- name: French - Gated content form proof of concept - thank-you page
  id: d483c791-9712-44aa-9072-30d4d43f6881
- name: French - Newsletter registration form
  id: eefdfcc8-8a24-444e-b4ed-471fdd9bdff7
- name: German - Newsletter registration form
  id: 5a034d43-36c1-4228-b745-104ea79c3a59
- name: German - Lead form
  id: 77a13db8-5f0f-454a-a928-7cc74a904a95
- name: French - Lead form
  id: 70b4ffb2-3b16-4906-910d-5384d86272e9
- name: French - MQL form
  id: c9707624-c9c7-4aed-aca9-7b5f38d35619
- name: German - MQL form
  id: d0ad15dc-a10b-4575-81ab-896bb4ea1dcc
- name: French - SQL form
  id: ce6598d3-e0fc-45fd-9295-7f3eb3e53942
- name: German - SQL form
  id: 7aceb99a-2cf3-4fde-8047-82a3b758b639
- name: French - Contact form
  id: ca378315-0a88-48d1-a561-5ab234e6bf72
- name: German - Contact form
  id: 2cc38f96-7384-4ec7-a565-43bddcc4d556
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

{% if page.new_forms %}
    {%- include section-new-forms-v1.html -%}
{% endif%}

{% if page.forms %}
    {%- include section-forms-v2.html -%}
{% endif %}

<!-- Start of HubSpot Embed Code
<script type="text/javascript" id="hs-script-loader" async defer src="//js-eu1.hs-scripts.com/147529884.js"></script>
End of HubSpot Embed Code -->