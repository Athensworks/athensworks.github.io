---
layout: page
title: Internal Membership
date: 2013-04-08 14:00
comments: true
sharing: false
footer: true
plans:
  # For profit - monthly
  - name: Day Pass
    paypal_button_id: M3WHKTLWRJ8UQ
    cost: 20
  - name: Flex Monthly Membership
    paypal_button_id: 2XLCVVGGEUQ26
    cost: 75
  - name: Full-time Monthly Membership
    paypal_button_id: Q4U5GM8UVUUDY
    cost: 120
  - name: Full-time Dedicated Monthly Membership
    paypal_button_id: 6FHGPKLCBJF68
    cost: 150

  # For profit - annual
  - name: Flex Annual Membership (with 10% Discount)
    paypal_button_id: WEEQP2TCCR6YL
    cost: 810
  - name: Full-time Annual Membership (with 10% Discount)
    paypal_button_id: JKEZVU9C9U6EJ
    cost: 1290
  - name: Full-time Dedicated Annual Membership (with 10% Discount)
    paypal_button_id: XE23RHT27VUX6
    cost: 1620

  # Nonprofit - monthly
  - name: Day Pass [Nonprofit]
    paypal_button_id: Y4FNF6DPF5C82
    cost: 15
  - name: Flex Monthly Membership [Nonprofit]
    paypal_button_id: QG6AQNHFBJPMA
    cost: 50
  - name: Full-time Monthly Membership [Nonprofit]
    paypal_button_id: 7AFT2LZV38B38
    cost: 80
  - name: Full-time Dedicated Monthly Membership [Nonprofit]
    paypal_button_id: BLDUABCEEVCCY
    cost: 100
---

*Select a membership level below. Your previous membership has already been canceled.*

{% for plan in page.plans %}
  <h4>{{ plan.name }} - ${{ plan.cost }}</h4>
  <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
    <input type="hidden" name="cmd" value="_s-xclick">
    <input type="hidden" name="hosted_button_id" value="{{ plan.paypal_button_id }}">
    <table>
    <tr><td><input type="hidden" name="on0" value="Your Name / Company Name">Your Name / Company Name</td></tr><tr><td><input type="text" name="os0" maxlength="200"></td></tr>
    <tr><td><input type="hidden" name="on1" value="Email Address">Email Address</td></tr><tr><td><input type="text" name="os1" maxlength="200"></td></tr>
    </table>
    <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_buynowCC_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
    <img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
  </form>
  <br />
{% endfor %}