---
title: Global Foods Group
layout: page
logo: yes
hs_region: eu1
hs_portalId: 145033053
brand_domain: gf-group.fr
main_domains:
- name: Pages de destination - Global
  type: CNAME
  host: info
  value: 145033053.group0.sites.hscoscdn-eu1.net
- name: E-mail marketing (version web) - Global
  type: CNAME
  host: email
  value: 145033053.group0.sites.hscoscdn-eu1.net
secondary_domains:
- name: Pages de destination - GFS
  type: CNAME
  host: gfs
  value: 145033053.group0.sites.hscoscdn-eu1.net
- name: Pages de destination - GSI
  type: CNAME
  host: gsi
  value: 145033053.group0.sites.hscoscdn-eu1.net
- name: Pages de destination - Foods Company
  type: CNAME
  host: foods-company
  value: 145033053.group0.sites.hscoscdn-eu1.net
sending_domains:
- domain:
  name: gf-solutions.fr
  dkim_main_type: CNAME
  dkim_main_host: hs1-145033053._domainkey
  dkim_main_value: hs-gf--solutions-fr.hs13a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-145033053._domainkey
  dkim_secondary_value: hs-gf--solutions-fr.hs13b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:145033053.spf10.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
- domain:
  name: foods-company.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-145033053._domainkey
  dkim_main_value: foods--company-com.hs13a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-145033053._domainkey
  dkim_secondary_value: foods--company-com.hs13b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:145033053.spf10.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
- domain:
  name: gs-industrie.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-145033053._domainkey
  dkim_main_value: hs-gs--industrie-com.hs13a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-145033053._domainkey
  dkim_secondary_value: hs-gs--industrie-com.hs13b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:145033053.spf10.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name:
#  occurence: first
#  script:
forms:
- name: Global Solutions Industrie - Formulaire de Contact
  id: b6a0d062-e09a-4dc0-8c94-eb051ef73fbd
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Global Foods Solution - Formulaire de Contact
  id: aa9fa43e-1ed2-40d8-a99b-625792504970
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Foods Company - Formulaire de Contact
  id: d6ee1166-9fe6-4142-8fbd-1b4cc0ca8ebe
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Global Foods Group - Formulaire de Contact
  id: 3176f16d-694d-439e-aadc-193690def1ed
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Global Solutions Industrie - Newsletter
  id: 91087aa0-9583-4c6d-9384-61e1604f8b5e
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Global Foods Solution - Newsletter
  id: 869bc8a5-b5dd-47af-bd0e-89e04b3297ba
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Foods Company - Newsletter
  id: 8280aba6-d3e8-4416-9307-ba665227246e
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Gated content - Ressource
  id: ece96d68-361c-48f8-b24d-cfff4a334afe
  onFormReady: "function($form) {
      var DOCUMENT = 'Document name';
      $('[name=\"latest_request_for_documentation\"]').val(DOCUMENT).change();
      }"
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire - Landing Page
  comment: Code à utiliser pour l'insertion du formulaire sur des pages hors HubSpot. Pour l'insertion de ce formulaire sur une landing page HubSpot, utiliser le module natif adapté. La variable "THANK_YOU_PAGE_URL" est à modifier en fonction de l'url de la page de remerciements choisie (page sur laquelle le formulaire de surqualification sera insérée).
  id: 9be2577d-ff4f-4557-9dd6-190bf67f10e1
  onFormReady: 
  onFormSubmit:
  onFormSubmitted: "function($form, data) {
    var THANK_YOU_PAGE_URL = 'https://gf-group.fr/';
    let submission = data.submissionValues; 
    window.location.href = THANK_YOU_PAGE_URL + \"?email=\" + encodeURIComponent(submission.email);
    }"
- name: Formulaire de surqualification
  id: 8dc4ce2a-4063-4c2e-ad8c-b1d9184de66f
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

{% if page.secondary_domains %}
    {%- include section-domains-secondary.html -%}
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