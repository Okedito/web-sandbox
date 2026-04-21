---
title: Berger-Levrault TriBU - Sandbox
layout: page
logo: yes
sandbox: yes
language: fr
hs_region: eu1
hs_portalId: 147990385 #Sandbox
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
forms:
- name: TEST - Exemple de formulaire de contact (legacy)
  id: 236bfb72-c0c6-498e-85d7-7e4f6e0107c7
#  onFormReady: function($form) { XYZ }
#  onFormSubmit: function($form) { XYZ }
#  onFormSubmitted: function($form) { XYZ }
new_forms:
- name: TEST - Exemple de formulaire de contact
  id: ba3b534f-fd28-4f66-8ba5-4a42a5d2364e
ctas:
- name: TEST - CTA pop-up Découvrir les solutions
  id: 394638614759
  type: pop-up
- name: TEST - CTA embedded Découvrir les solutions
  id: 394667419879
  type: embedded
  occurence: first
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-394667419879\"
  style=\"max-width:100%; max-height:100%; width:700px;height:315.8984375px\" data-hubspot-wrapper-cta-id=\"394667419879\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLJttuoHGKtSZd9RgKiG974xx4ePKIzRhfZjnR3kvd%2FigaFwo2Gw04odNPIKxQjdQU5mYc2Uc8sFgSwkmwbFtamIzhmYu1wBFaj3QVXMzKFezcdmByTmCzuIAHDaGFIS5bhOEhEdNUzBWhbNWuWXq7G7nPVAaZZFFm2AHwZ0NbcjtlQzimXSlzGSMlL2mp1WBP8owh%2BS8LfQEjCGlj%2Bw3ATr9BV0QtVGy3VZ1gFm4z2W5GkT%2Bc4g5gu3zPutsc1DI53yEn4tHzTiyCBxnrFvCzf3GL456bTbso7p7bGXZeHX9Q%3D%3D&webInteractiveContentId=394667419879&portalId=147990385\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"FREE KIT DOWNLOAD Community Management 3 templates to help you build, grow and connect with your community. &nbsp;\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/147990385/interactive-394667419879.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
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
<script type="text/javascript" id="hs-script-loader" async defer src="//js-eu1.hs-scripts.com/147990385.js"></script>
<!-- End of HubSpot Embed Code -->