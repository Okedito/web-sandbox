---
title: Dani Alu
layout: page
logo: yes
hs_region: eu1
hs_portalId: 145721206
brand_domain: danialu.fr
main_domains:
- name: Pages de destination
  type: CNAME
  host: info
  value: 145721206.group0.sites.hscoscdn-eu1.net
- name: E-mail marketing (version web)
  type: CNAME
  host: email
  value: 145721206.group0.sites.hscoscdn-eu1.net
sending_domains:
- domain:
  name: danialu.fr
  dkim_main_type: CNAME
  dkim_main_host: hs1-145721206._domainkey
  dkim_main_value: danialu-fr.hs05a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-145721206._domainkey
  dkim_secondary_value: danialu-fr.hs05b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:145721206.spf03.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name:
#  occurence: first
#  script:
forms:
- name: Formulaire contact - demande de rdv
  id: b0029179-5a9f-4776-b027-dd2ecc7abc1b
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Gated Content
  id: 51f12e37-c298-4d9e-a121-64ef0be6960f
  #onFormReady: "function($form) {
  #    var DOCUMENT = 'Document name';
  #    $('[name=\"latest_request_for_documentation\"]').val(DOCUMENT).change();
  #    }"
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Landing Page (progressif)
  #comment: Code à utiliser pour l'insertion du formulaire sur des pages hors HubSpot. Pour l'insertion de ce formulaire sur une landing page HubSpot, utiliser le module natif adapté. La variable "THANK_YOU_PAGE_URL" est à modifier en fonction de l'url de la page de remerciements choisie (page sur laquelle le formulaire de surqualification sera insérée).
  id: ea549c26-75c6-445d-bed4-469851b463bf
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Thank You Page (progressif)
  id: c58e9873-40b9-4789-bff2-e93199423dc9
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Newsletter
  id: 8d016ae3-9521-4611-8b12-f380f2ed5fdc
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