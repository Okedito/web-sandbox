---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Cimalpes
layout: page
logo: yes
hs_region: eu1
hs_portalId: 139708350
ctas:
- name: CTA 1 - Download Android
  occurence: first
  script: <span class="hs-cta-wrapper" id="hs-cta-wrapper-4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4"><span class="hs-cta-node hs-cta-4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4" id="hs-cta-4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4"><!--[if lte IE 8]><div id="hs-cta-ie-element"></div><![endif]--><a href="https://hubspot-cta-redirect-eu1-prod.s3.amazonaws.com/cta/redirect/25969719/4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4" ><img class="hs-cta-img" id="hs-cta-img-4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4" style="border-width:0px;" src="https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25969719/4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4.png"  alt="Get it on Google Play"/></a></span><script charset="utf-8" src="https://js-eu1.hscta.net/cta/current.js"></script><script type="text/javascript"> hbspt.cta.load(25969719, '4d2a9b8e-e9fe-4ca5-816b-946ec9716dd4', {"useNewLoader":"true","region":"eu1"}); </script></span>
forms:
- name: Formulaire Newsletter FR
  id: 9712940e-20c2-44c4-bc38-1c7603ceaf7e
  onFormReady:
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Newsletter EN
  id: 2ee93fc6-e7d1-4fba-88ca-876706770fc1
  onFormReady:
  onFormSubmit:
  onFormSubmitted:
- name: Formulaire Livret Expérience FR
  id: 951dfa9e-a879-4375-9e80-061b0aadd668
  onFormReady: yes
  onFormSubmit: yes
  onFormSubmitted: yes
- name: Formulaire Livret Expérience EN
  id: 6dc1ec6b-f123-4d3d-a1e1-07f1a7e78df0
  onFormReady: yes
  onFormSubmit: yes
  onFormSubmitted: yes
- name: Formulaire Brochure FR
  id: e7d70d74-fd1c-4097-a214-b1f1da737ad0
  onFormReady: yes
  onFormSubmit: yes
  onFormSubmitted: yes
- name: Formulaire Brochure EN
  id: 1a1b1e71-085d-459f-b21f-083ad4c40c0e
  onFormReady: yes
  onFormSubmit: yes
  onFormSubmitted: yes
---

{%- include section-introduction.html -%}

{% if page.hs_portalId %}
    {%- include section-tracking-code.html -%}
{% endif %}

{% comment %}
{% if page.ctas %}
    {%- include section-ctas.html -%}
{% endif %}
{% endcomment %}

{% if page.forms %}
    {%- include section-forms-cimalpes.html -%}
{% endif %}

<h2>Formulaire Plan | FR</h2>
<button onclick="CopyToClipboard('bc21f15a-117b-4106-a0b2-4bc43be772c9')">Copier le code</button>

    <script charset="utf-8" type="text/javascript" src="//js-eu1.hsforms.net/forms/embed/v2.js"></script>
    <script>
      hbspt.forms.create({
        portalId: "139708350",
        formId: "bc21f15a-117b-4106-a0b2-4bc43be772c9",
        onFormReady: function($form) {
          console.log(window.location.href);
        },
        onFormSubmit function($form) {
          $('[name="doc_request_form"]').val(window.location.href).change();
        }
      });
    </script>
  {: id="A{{ form.id }}"}

<script charset="utf-8" type="text/javascript" src="//js-eu1.hsforms.net/forms/embed/v2.js"></script>
<script>
  hbspt.forms.create({
  portalId: "139708350",
  formId: "bc21f15a-117b-4106-a0b2-4bc43be772c9",
  onFormReady: function($form) {
    console.log(window.location.href);
  },
  onFormSubmit: function($form) {
    $('[name="doc_request_form"]').val(window.location.href).change();
  }
  });
</script>