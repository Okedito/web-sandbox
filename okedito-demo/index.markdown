---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Okédito sandbox account 2
layout: page
hs_region: eu1
hs_portalId: 26174332
ctas:
#- name: CTA 1 - Download Android
#  occurence: first
#  script: <span class="hs-cta-wrapper" id="hs-cta-wrapper-4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4"><span class="hs-cta-node hs-cta-4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4" id="hs-cta-4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4"><!--[if lte IE 8]><div id="hs-cta-ie-element"></div><![endif]--><a href="https://hubspot-cta-redirect-eu1-prod.s3.amazonaws.com/cta/redirect/25969719/4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4" ><img class="hs-cta-img" id="hs-cta-img-4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4" style="border-width:0px;" src="https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25969719/4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4.png"  alt="Get it on Google Play"/></a></span><script charset="utf-8" src="https://js-eu1.hscta.net/cta/current.js"></script><script type="text/javascript"> hbspt.cta.load(25969719, '4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4', {"useNewLoader":"true","region":"eu1"}); </script></span>
#- name: CTA 2 - Download iOS
#  occurence: second
#  script: <span class="hs-cta-wrapper" id="hs-cta-wrapper-ebf02ff0-39c9-4eaf-a8e5-0e68ac2f582d"><span class="hs-cta-node hs-cta-ebf02ff0-39c9-4eaf-a8e5-0e68ac2f582d" id="hs-cta-ebf02ff0-39c9-4eaf-a8e5-0e68ac2f582d"><!--[if lte IE 8]><div id="hs-cta-ie-element"></div><![endif]--><a href="https://hubspot-cta-redirect-eu1-prod.s3.amazonaws.com/cta/redirect/25969719/ebf02ff0-39c9-4eaf-a8e5-0e68ac2f582d" ><img class="hs-cta-img" id="hs-cta-img-ebf02ff0-39c9-4eaf-a8e5-0e68ac2f582d" style="border-width:0px;" src="https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25969719/ebf02ff0-39c9-4eaf-a8e5-0e68ac2f582d.png"  alt="Download on the App Store"/></a></span><script charset="utf-8" src="https://js-eu1.hscta.net/cta/current.js"></script><script type="text/javascript"> hbspt.cta.load(25969719, 'ebf02ff0-39c9-4eaf-a8e5-0e68ac2f582d', {"useNewLoader":"true","region":"eu1"}); </script></span>
forms:
#- name: Formulaire 1 - Abonné newsletter
#  id: 5f5bca25-d613-4a56-9ead-8a37627f9023
- name: Formulaire de test 1
  id: 70f43189-80ac-4522-8fa6-4253d3bbbcbc
#- name: Formulaire 3 - MQL
#  id: d2daa079-e2b3-41a9-add3-419cb32d596c
#- name: Formulaire 4 - SQL
#  id: 0da360b8-da1f-4055-afc1-2e4f01f95110
#- name: Formulaire 5 - Qualification / Thank-you page
#  id: 4399e57c-8c7b-4847-97b3-a3136ea4f53d
---

{%- include section-introduction.html -%}

{% if page.hs_portalId %}
    {%- include section-tracking-code.html -%}
{% endif %}

{% if page.ctas %}
    {%- include section-ctas.html -%}
{% endif %}

{% if page.forms %}
    {%- include section-forms.html -%}
{% endif %}

<h2>HTML form</h2>

<form id="HTML form">
  <label for="firstname">First name:</label><br>
  <input type="text" id="firstname" name="firstname" value="John"><br>
  <label for="lastname">Last name:</label><br>
  <input type="text" id="lastname" name="lastname" value="Doe"><br>
  <label for="email">E-mail:</label><br>
  <input type="text" id="email" name="email" value="john.doe@email.com">
  <input type="submit" value="Submit">
</form>

<hr/>


<!-- Start of HubSpot Embed Code -->
<script type="text/javascript" id="hs-script-loader" async defer src="//js-eu1.hs-scripts.com/26174332.js"></script>
<!-- End of HubSpot Embed Code -->

