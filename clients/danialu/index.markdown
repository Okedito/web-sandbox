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
  id: e5ea87d6-9d98-493a-b5fa-ac625a025942
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Gated Content
  id: 58dce789-e226-4380-b2e2-e5395321d006
  onFormReady: "function($form) {
      var DOCUMENT = 'Nom du document';
      $('[name=\"derniere_demande_de_documentation\"]').val(DOCUMENT).change();
      }"
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Landing Page
  comment: Code à utiliser pour l'insertion du formulaire sur des pages hors HubSpot. Pour l'insertion de ce formulaire sur une landing page HubSpot, utiliser le module natif adapté. La variable "THANK_YOU_PAGE_URL" est à modifier en fonction de l'url de la page de remerciements choisie (page sur laquelle le formulaire de surqualification sera insérée).
  id: ea549c26-75c6-445d-bed4-469851b463bf
  onFormReady: 
  onFormSubmit:
  onFormSubmitted: "function($form, data) {
    var THANK_YOU_PAGE_URL = 'https://danialu.fr/';
    let submission = data.submissionValues; 
    window.location.href = THANK_YOU_PAGE_URL + \"?email=\" + encodeURIComponent(submission.email);
    }"
- name: Formulaire Thank You Page
  id: c58e9873-40b9-4789-bff2-e93199423dc9
  onFormReady: 
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Newsletter
  id: 20d28a87-02f1-48a9-9b41-cbdd62c4387d
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