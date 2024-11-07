---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Intuiti
layout: page
logo: yes
hs_region: eu1
hs_portalId: 145014391
brand_domain: groupe-iteractii.com
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
- name: Intuiti | Téléchargement
  id: 6ce224ba-0259-44bc-ab0d-9d8319ac66f2
  onFormReady: "function($form) {
      var DOCUMENT = 'Nom du document téléchargeable';
      $('#hsForm_6ce224ba-0259-44bc-ab0d-9d8319ac66f2 > div.hs_doc_request_form.hs-doc_request_form.hs-fieldtype-text.field.hs-form-field > div > input').val(DOCUMENT).change();
      }"
  onFormSubmit: "function($form) {
      sessionStorage.setItem(\"mail\", $(\"#email-6ce224ba-0259-44bc-ab0d-9d8319ac66f2\")[0].value);
    }"
  onFormSubmitted: "function($form) {
      window.addEventListener('message', event => {
        if(event.data.type === 'hsFormCallback' && event.data.eventName === 'onFormSubmitted') {
          document.querySelector(\".submitted-message a\").href += \"?email=\"+ sessionStorage.getItem(\"mail\");
        }
      });
    }"
- name: Intuiti | Demande de contact
  id: a7f4b350-566a-4308-920b-1145553e1ec5
- name: Intuiti | Inscription Decriiipt
  id: 79aaa8bb-a9eb-427f-873e-168dd26d2ba1
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