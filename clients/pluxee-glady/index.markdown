---
title: Pluxee (Glady)
layout: page
logo: yes
hs_region: eu1
hs_portalId: 146250427
brand_domain: pluxee.fr
main_domains:
- name: Emails marketing
  type: CNAME
  host: email
  value: 146250427.group0.sites.hscoscdn-eu1.net
sending_domains:
- domain:
  name: pluxee.fr
  dkim_main_type: CNAME
  dkim_main_host: hs1-146250427._domainkey
  dkim_main_value: pluxee-fr.hs19a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-146250427._domainkey
  dkim_secondary_value: pluxee-fr.hs19b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:146250427.spf05.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
- domain:
  name: glady.com
  dkim_main_type: CNAME
  dkim_main_host: hs1-146250427._domainkey
  dkim_main_value: glady-com.hs19a.dkim.hubspotemail.net.
  dkim_secondary_type: CNAME
  dkim_secondary_host: hs2-146250427._domainkey
  dkim_secondary_value: glady-com.hs19b.dkim.hubspotemail.net.
  spf_type: TXT
  spf_host: "@"
  spf_value: include:146250427.spf05.hubspotemail.net
  dmarc_type: TXT
  dmarc_host: _dmarc
  dmarc_value: v=DMARC1; p=none;
#ctas:
#- name: (Nom CTA)
#  occurence: first
#  script: ""
#forms:
#- name: Formulaire 1
#  id: 
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

{% if page.ctas %}
    {%- include section-ctas.html -%}
{% endif %}

{% if page.forms %}
    {%- include section-forms-v2.html -%}
{% endif %}