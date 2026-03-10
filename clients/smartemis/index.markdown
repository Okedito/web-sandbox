---
title: Smartemis
layout: page
logo: yes
language: en
hs_region: eu1
#hs_portalId: 147529884 #Sandbox
hs_portalId: 25027870 #Production
brand_domain: smartemis.com
main_domains:
#- name: Website pages	
#  type: CNAME
#  host: website-page
#  value: 45847199.group49.sites.hubspot.net
#- name: Blog
#  type: CNAME
#  host: blog
#  value: 45847199.group49.sites.hubspot.net 
- name: Landing pages	
  type: CNAME
  host: info
  value: 25027870.group0.sites.hscoscdn-eu1.net
- name: Landing pages - domain validation entry
  type: TXT
  host: _cf-custom-hostname.info
  value: 9a2ed781-b21f-4961-95ef-6247afe74854
- name: Marketing email (web version)
  type: CNAME
  host: email
  value: 25027870.group0.sites.hscoscdn-eu1.net
- name: Marketing email (web version) - domain validation entry
  type: TXT
  host: _cf-custom-hostname.email
  value: eb47b72f-336d-4568-96de-6987d95eeffd
#- name: Sales & service email (tracking)
#  type: CNAME
#  host: ???
#  value: 45847199.group49.sites.hubspot.net
#- name: Knowledge base
#  type: CNAME
#  host: ???
#  value: 45847199.group49.sites.hubspot.net
#- name: Customer portal
#  type: CNAME
#  host: ???
#  value: 45847199.group49.sites.hubspot.net
#- name: Podcast
#  type: CNAME
#  host: ???
#  value: 45847199.group49.sites.hubspot.net
#- name: Quotes
#  type: CNAME
#  host: quotes
#  value: 45847199.group49.sites.hubspot.net
- name: Meetings scheduler
  type: CNAME
  host: meetings
  value: 25027870.group0.sites.hscoscdn-eu1.net
- name: Meetings scheduler - domain validation entry
  type: TXT
  host: _cf-custom-hostname.meetings
  value: ce4d6dd5-42c4-4962-b04d-04a3e7232da0
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
- name: DE - Kontaktformular
  id: 518f1791-e6f7-4edb-a553-fd5f56249ad8
- name: DE - Bewerberformular
  id: d1842234-7b20-4889-b59f-5efac7200ad1
new_forms:
- name: FR - Gated content form proof of concept - landing page
  id: 8f8f3e12-70dd-4295-8c47-2c327126addd
- name: FR - Gated content form proof of concept - thank-you page
  id: d483c791-9712-44aa-9072-30d4d43f6881
- name: FR - Newsletter registration form
  id: eefdfcc8-8a24-444e-b4ed-471fdd9bdff7
- name: DE - Newsletter registration form
  id: 5a034d43-36c1-4228-b745-104ea79c3a59
- name: FR - Lead form
  id: 70b4ffb2-3b16-4906-910d-5384d86272e9
- name: DE - Lead form
  id: 77a13db8-5f0f-454a-a928-7cc74a904a95
- name: FR - MQL form
  id: c9707624-c9c7-4aed-aca9-7b5f38d35619
- name: DE - MQL form
  id: d0ad15dc-a10b-4575-81ab-896bb4ea1dcc
- name: FR - SQL form
  id: ce6598d3-e0fc-45fd-9295-7f3eb3e53942
- name: DE - SQL form
  id: 7aceb99a-2cf3-4fde-8047-82a3b758b639
- name: FR - Contact form
  id: ca378315-0a88-48d1-a561-5ab234e6bf72
- name: DE - Contact form
  id: 2cc38f96-7384-4ec7-a565-43bddcc4d556
- name: EN - Request Investor Material
  id: 6885c739-a161-4038-9996-75d0c7275f47
- name: DE - Submit Your Application
  id: 725ea039-5137-4632-b776-418b58bcadcc
- name: FR - Submit Your Application
  id: ef6439bf-c17c-4d8d-a898-9754743e04d0
ctas:
- name: EN - Download Whitepaper
  occurence: first
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-374430355663\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"374430355663\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLInQD1Dk2EQPcu4Ktd4AZx2zc%2BSArO7tTSsU5RUnXe6lnusVJe9SPnKZQCU4nSSln2UtZZc2B5Zr5rHi%2F3wgrEphMZVr%2BkGziaDDQUl2ZifEdbQO5kKITawCM39qLDXJLeD1YXNLKSIHo%2F3e3SFMKLR6IoLD4mz2RO82mk%3D&webInteractiveContentId=374430355663&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Download&amp;nbsp;Whitepaper\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-374430355663.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: FR - Download Whitepaper
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375162943725\"
  style=\"max-width:100%; max-height:100%; width:240px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375162943725\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLKVCuA05oVCYqVdwtPhtlcwbDzsb6Wdccb5Ojw8k0oh6DBdryThBBiidKCzaKTrzy3YoUaxTL85CSC0N7Wq7080kvLBdcFffo1oSNGNmBt38uA%3D&webInteractiveContentId=375162943725&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"T&eacute;l&eacute;charger&amp;nbsp;le&amp;nbsp;livre&amp;nbsp;blanc\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375162943725.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: DE - Download Whitepaper
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375163004111\"
  style=\"max-width:100%; max-height:100%; width:250px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375163004111\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLLoSEGTav3jt7DSkiBwXxK2vPhHpfmt9BXpsci%2BlhKOuiFP0gQ6CpuSaDpTBfL2fXCxQPugbI7GFCWkwX6JSSq3d840CSPC3%2FfCyaDdB4HRnZ0%3D&webInteractiveContentId=375163004111&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Whitepaper&amp;nbsp;herunterladen\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375163004111.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: EN - Download Case Study
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-374643795190\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"374643795190\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLIkagu1AngfCO7LHG%2B%2F%2BzBVe9SHjfmLFvm%2BXrErK2LJcuJ0hekZy2hhAXPIpJ0t50%2BXS6AE%2B1M1%2FtrhFGYsLJByoPBOW223RFROnYkm%2F0CMk%2BI%3D&webInteractiveContentId=374643795190&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Download&amp;nbsp;Case&amp;nbsp;Study\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-374643795190.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: FR - Download Case Study
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375163003109\"
  style=\"max-width:100%; max-height:100%; width:260px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375163003109\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLLi1XxstcJ8jd8Ny%2BNUHcKARR4xqWdw5dtahsdfj9DL%2F0K%2FMzI3FSIQsWy1AKUuVqyHChE2nPd94eD8YRHYq%2Fgv7euEpevwUzERHhEBtAq%2FFtE%3D&webInteractiveContentId=375163003109&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"T&eacute;l&eacute;charger&amp;nbsp;l'&eacute;tude&amp;nbsp;de&amp;nbsp;cas\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375163003109.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: DE - Download Case Study
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375163004129\"
  style=\"max-width:100%; max-height:100%; width:240px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375163004129\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLKAV8qs6wRb8KsZxh2tEfQMOfTr%2FUSJEnthyj7ruIaCbfDvRzdz%2BOLiHroq%2B%2B288JLwZ4%2FA0j63XLI9kurkzxw%2B7VCtb4GAKVcaNkwQ6UzLQH8%3D&webInteractiveContentId=375163004129&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Fallstudie&amp;nbsp;herunterladen\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375163004129.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: EN - View Video
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-374463867095\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"374463867095\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLIWqdKj%2Bngaq24pK1jvGmeYKR0mHCRZALh4zqFqc%2FvY4yQjOihiaSIsLMzoyBQ2TLgypUu0G%2BggBA9FNWu%2Bv0CgP%2FefVmVT%2F2Tjxu6letXC5so%3D&webInteractiveContentId=374463867095&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"View&amp;nbsp;Video\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-374463867095.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: FR - View Video
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375162945768\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375162945768\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLL89dqvC7eFDoN%2B9Bu%2Fv2Y1mtVTSh4dqmBEA%2BwMtly52YrJ1H%2FdSuE0Jy6FMA%2FT%2BOZZp2OhQr0yXD%2B9h0gpy%2BO44%2FCnRRrlZw6OqjHAcp3IW8iWSIFSnrwHrHcXuBgH826sFkyS7SMWpidTHiO4%2BXzOEGsKZja25NV%2BHqg%3D&webInteractiveContentId=375162945768&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Regarder&amp;nbsp;la&amp;nbsp;vid&eacute;o\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375162945768.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: DE - View Video
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375163075810\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375163075810\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLJ%2B6sySKmk8vCG9Uv1l65BE%2F6B%2BU9aHVZdn8DvYkmXrUKTBx4qxprTnFWjlClb75DNzCxjDCw6ukw8eWSENZ1XGmPb8xh6Tj13unga0HOV4g5f3kj8S0jAAfOghGHVyTw85AU3gfHodMliErexeKYwyi8Bax9vaO%2BbpK6A%3D&webInteractiveContentId=375163075810&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Video&amp;nbsp;ansehen\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375163075810.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: EN - Contact Us
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-374643796174\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"374643796174\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLL30SGUuOftNZsKvbkysdFY5rFH8nXPoSHC8pMoDGiD9MJoJVFOtvTY29znB%2FpOGB4AyxXktEVqQKW164D8UdX6UDXIcsap3CAFNmsCudWR56kW3IPu7gtTdwPDwzyVZX3Rdd0q7358%2BLsjyzgLMpFHlfXK79Ac8nVD5QI%3D&webInteractiveContentId=374643796174&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Contact&amp;nbsp;Us\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-374643796174.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: FR - Contact Us
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375162943716\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375162943716\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLIILs%2B4gge8jzg5k%2FBKZFlNkcO0d0C%2FqNb5nB7XJYrd%2Bx1GhWZDkczj4gFzkVLy2%2BneZHg7UbXxyxWJyufeUVGUq%2FkW8tR2hEAPZQv%2BgRX32IE%3D&webInteractiveContentId=375162943716&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Contactez-nous\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375162943716.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: DE - Contact Us
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375163075827\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375163075827\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLL4MmIkR8pgI7SUmiJSNzh0Dla%2FdYTbmwCq8Q%2BYc10QCbloNaG0JMyBPB%2FzfRkcZbSEMkmDL2F49sc7Gx2Fc%2FqmPOPXoq8%2FRg4BN3rv%2F3s9TgU%3D&webInteractiveContentId=375163075827&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Kontakt\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375163075827.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: EN - Book an appointment
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-374773128426\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"374773128426\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLKeruf0sBf7mnSU%2FrxoD%2FB7Mox9LFb2%2BxCLuCYsTSKRMk4rM8T1WyWomfy0VwPJmsZe4D1lG9M%2FSkQhhNq3UpTH8pADZL8T31120oLKoDfNCC0%3D&webInteractiveContentId=374773128426&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Book&amp;nbsp;an&amp;nbsp;appointment\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-374773128426.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: FR - Book an appointment
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375162943690\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375162943690\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLIu7xMDlXUq3tpbugpElhf4ZERdtgwpk%2FUoESXCIZwaggZladx1LaO78zfh5rwIs1FVU7PP9Ms5ZTJoDdW88n7O7LL%2BT%2B%2BHViqZuLjPspnKVTc0ylV3iqTXQCaGty6ha9lkfAwIdpU0cjmEpXPfTF7SYGYnZnGETTqAC4o%3D&webInteractiveContentId=375162943690&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Prendre&amp;nbsp;rendez-vous\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375162943690.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
- name: DE - Book an appointment
  occurence: 
  script: "<div class=\"hs-cta-embed hs-cta-simple-placeholder hs-cta-embed-375163409644\"
  style=\"max-width:100%; max-height:100%; width:226px;height:50.390625px\" data-hubspot-wrapper-cta-id=\"375163409644\">
  <a href=\"https://cta-eu1.hubspot.com/web-interactives/public/v1/track/redirect?encryptedPayload=AVxigLJhosfJVjYO1e9dPt3zMIOQFg1sDOqpm6TssYEXc3xLX4VpwWMpoSVuDwo5BB%2F6ESX61XnPLiIFUGJHI0iE9csIaXionY4Jzp6AsLPu4fQ7ms0%3D&webInteractiveContentId=375163409644&portalId=25027870\" target=\"_blank\" rel=\"noopener\" crossorigin=\"anonymous\">
    <img alt=\"Termin&amp;nbsp;vereinbaren\" loading=\"lazy\" src=\"https://hubspot-no-cache-eu1-prod.s3.amazonaws.com/cta/default/25027870/interactive-375163409644.png\" style=\"height: 100%; width: 100%; object-fit: fill\"
      onerror=\"this.style.display='none'\" />
  </a>
</div>"
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

{% if page.new_forms %}
    {%- include section-new-forms-v1.html -%}
{% endif%}

{% if page.forms %}
    {%- include section-forms-v2.html -%}
{% endif %}

{% if page.ctas %}
    {%- include section-ctas-v2.html -%}
{% endif %}

<!-- Start of HubSpot Embed Code
<script type="text/javascript" id="hs-script-loader" async defer src="//js-eu1.hs-scripts.com/147529884.js"></script>
End of HubSpot Embed Code -->