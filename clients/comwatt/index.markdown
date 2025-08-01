---
title: Comwatt
layout: page
logo: yes
hs_region: eu1
hs_portalId: 146117604
brand_domain: ca-monenergie.fr
main_domains: 
#- name: Pages de site web
#  type: CNAME
#  host: 
#  value: 
- name: Pages de destination
  type: CNAME
  host: info
  value: 146117604.group0.sites.hscoscdn-eu1.net
- name: E-mail marketing (version web)
  type: CNAME
  host: courriel
  value: 146117604.group0.sites.hscoscdn-eu1.net
- name: E-mail de vente et de service client (suivi)
  type: CNAME
  host: courriel
  value: 146117604.group0.sites.hscoscdn-eu1.net
- name: Base de connaissances
  type: CNAME
  host: support
  value: 146117604.group0.sites.hscoscdn-eu1.net
#- name: Portail client
#  type: CNAME
#  host: 
#  value: 
- name: Planficateur de réunions
  type: CNAME
  host: rdv
  value: 146117604.group0.sites.hscoscdn-eu1.net
redirected_domains:
- domain : 
  name : comwatt.com
  type_1: CNAME
  host_1: support
  value_1: 146117604.group0.sites.hscoscdn-eu1.net
  type_2: TXT
  host_2: _cf-custom-hostname.support
  value_2: 6e7c83d9-fcf4-42b5-bfd2-8ba41677b074
sending_domains:
- domain:
  name: ca-monenergie.fr
  dkim_main_type: CNAME
  dkim_main_host: hs1-146117604._domainkey
  dkim_main_value: hs-ca--monenergie-fr.hs06a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-146117604._domainkey
  dkim_secondary_value: hs-ca--monenergie-fr.hs06b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:146117604.spf06.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
- domain:
  name: comwatt.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-146117604._domainkey
  dkim_main_value: comwatt-com.hs06a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-146117604._domainkey
  dkim_secondary_value: comwatt-com.hs06b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:146117604.spf06.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name: CTA - Obtenir un prix
#  occurence: first
#  script: ""
#forms:
#- name: Formulaire contact - demande de rdv
#  id: e5ea87d6-9d98-493a-b5fa-ac625a025942
#  onFormReady: 
#  onFormSubmit:
#  onFormSubmitted:
#- name: Formulaire Gated Content
#  id: 58dce789-e226-4380-b2e2-e5395321d006
#  onFormReady: "function($form) {
#      var DOCUMENT = 'Nom du document';
#      $('[name=\"derniere_demande_de_documentation\"]').val(DOCUMENT).change();
#      }"
#  onFormSubmit:
#  onFormSubmitted:
#- name: Formulaire Landing Page
#  comment: Code à utiliser pour l'insertion du formulaire sur des pages hors HubSpot. Pour l'insertion de ce formulaire sur une landing page HubSpot, utiliser le module natif adapté. La variable "THANK_YOU_PAGE_URL" est à modifier en fonction de l'url de la page de remerciements choisie (page sur laquelle le formulaire de surqualification sera insérée).
#  id: ea549c26-75c6-445d-bed4-469851b463bf
#  onFormReady: 
#  onFormSubmit:
#  onFormSubmitted: "function($form, data) {
#    var THANK_YOU_PAGE_URL = 'https://danialu.fr/';
#    let submission = data.submissionValues; 
#    window.location.href = THANK_YOU_PAGE_URL + \"?email=\" + encodeURIComponent(submission.email);
#    }"
#- name: Formulaire Thank You Page
#  id: c58e9873-40b9-4789-bff2-e93199423dc9
#  onFormReady: 
#  onFormSubmit:
#  onFormSubmitted:
#- name: Formulaire Newsletter
#  id: 20d28a87-02f1-48a9-9b41-cbdd62c4387d
#  onFormReady: 
#  onFormSubmit:
#  onFormSubmitted:
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

{% if page.redirected_domains %}
    {%- include section-domains-redirected.html -%}
{% endif%}

{% if page.ctas %}
    {%- include section-ctas.html -%}
{% endif %}

{% if page.forms %}
    {%- include section-forms-v2.html -%}
{% endif %}