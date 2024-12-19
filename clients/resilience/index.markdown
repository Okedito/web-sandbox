---
title: Resilience
layout: page
logo: yes
hs_region: eu1
hs_portalId: 25122959
brand_domain: resilience.care
#main_domains:
#- name: Pages de destination	
#  type: CNAME
#  host: go
#  value: 144852889.sites.hscoscdn-eu1.net
#- name: E-mail marketing (version web)
#  type: CNAME
#  host: email
#  value: 144852889.sites.hscoscdn-eu1.net
#sending_domains:
#- domain:
#  name: wedia-group.com
#  dkim_main_type: CNAME
#  dkim_main_host: hs1-144852889._domainkey
#  dkim_main_value: wedia--group-com.hs07a.dkim.hubspotemail.net.
#  dkim_secondary_type: CNAME
#  dkim_secondary_host: hs2-144852889._domainkey
#  dkim_secondary_value: wedia--group-com.hs07b.dkim.hubspotemail.net.
#  spf_type: TXT
#  spf_host: "@"
#  spf_value: include:144852889.spf06.hubspotemail.net
#  dmarc_type: TXT
#  dmarc_host: _dmarc
#  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name:
#  occurence: first
#  script:
forms:
- name: Formulaire - Newsletter
  id: 1695dea6-174f-4ac3-9676-613c2b88c2bb
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire - Guides, livres blancs et posters
  id: b2e2306a-e9f2-4d6c-aca7-bde4fa769df2
  onFormReady: "function($form) {
      var DOCUMENT = 'Document name';
      $('[name=\"latest_request_for_documentation\"]').val(DOCUMENT).change();
      }"
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire - Démo
  id: d8f78a21-6e0b-4eff-9a68-cddbec7787e4
  onFormReady: 
  onFormSubmit:
  onFormSubmitted: "function($form) {
      var REDIRECT_URL = 'https://meet.okedito.com/meetings/daniele-lodola/30-minutes';
      window.location.href = REDIRECT_URL;
    }"
- name: Formulaire - Landing Page
  id: fe8dc68b-81b2-4bfd-afd6-b2ebf9398aac
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire - Thank You Page
  id: 222e3ab3-4eb0-4689-a2b0-48829358967a
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
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