=== Easy Digital Downloads - Dropbox Sync ===

Contributors: Kevin Michael Gray
Contributors Website: www.wp-e-signature.com
Tags: Easy Digital Downloads, Dropbox Sync
Extension URL: https://easydigitaldownloads.com/extensions/dropbox-sync?ref=1065
Documentation: https://easydigitaldownloads.com/docs/dropbox-sync-setup-documentation?ref=1065
License: GPLv2

== Description ==

Dropbox Sync allows you to sync in real-time a PDF purchase receipt with your Dropbox account. When a successful order is triggered from your store, Dropbox sync will automatically create a PDF using the template that you created (yes you can use shortcodes, html, and more in the template), Dropbox Sync then stores the generated PDF in real-time in your Dropbox account.

Dropbox Sync is extremely useful for accounting purposes, you can easily store PDF exports in real-time of purchase orders and purchase receipts.

== THE TEMPLATE ==

We created this helpful html template for you to paste into the “Dropbox Sync” template page.  WordPress requires the css to be passed inline the html using style=“” tags in order to properly format the pdf receipt that is exported when a user makes a purchase using your Easy Digital Downloads plugin and WordPress website.

== INSTRUCTIONS ==

1. Install Easy Digital Downloads

2. Install Dropbox Sync

3. Enter License key for Dropbox Sync

4. Sync/Authenticate your Dropbox Account with EDD Dropbox Sync

5. Copy and paste the html below into the text editor which is displayed once you have successfully synced your Dropbox account with Easy Digital Downloads.

6. Customize content/information in the html text editor to taste.


== COPY THE HTML BELOW INTO TEXT EDTIOR ==


<div style="font-family: Arial;">
<div style="z-index: 10; position: relative; margin-left: 0.5in; min-height: 90px;">
<div style="font-family: Arial;float: left; width: 300px; margin-bottom: 20px;">{sitename}<br />555 My Street Blvd<br />Suite #249<br />Portland OR  97232</div>
<div style="width: 250px; height: 90px; float: right;">
<div style="text-align: center; font-size: 11px; line-height: 12px;"><a href="http://www.rockstaridea.com"><img alt="" src="http://rockstaridea.com/assets/images/rsi-logo-transparent.png" width="167" height="80" /></a></div>
</div>
</div>
<div style="clear: both; margin-top: 54px; margin-left: 0.5in; min-height: 126px;">
<div style="font-family: Arial;float: left; width: 300px; padding-bottom: 20px;">Customer Username: {username}<br />Customer Full Name: {fullname}<br />Customer email: {user_email}<br />Customer Address: {billing_address}<br />Payment method: {payment_method}</div>
<div style="font-family: Arial;float: right; width: 290px; padding-bottom: 20px;">
<table cellspacing="0">
<tbody>
<tr><th style="text-align: left;"><span>Payment ID</span></th>
<td>#{payment_id}</td>
</tr>
<tr><th style="text-align: left;"><span>Purchase Date</span></th>
<td>{date}</td>
</tr>
<tr><th style="text-align: left;"><span>Tax Charged</span></th>
<td>${tax}</td>
</tr>
<tr class="invheader-invoicedetails-balance"><th>
<div style="text-align: left;"><span>Order Total</span></div>
</th>
<td>
<div>${price}</div>
</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
<div style="width: 800px;height: 43px;border-color: gray;background: #8b8a87;margin-left: 44px;padding-top: 16px;color: #fff;font-family: Arial;"><span style="margin-left: 12px; margin-top: 5px; font-weight: bold; font-size: 22px;">Items Purchased</span></div>
<div style="margin-left: 44px;">
<p style="font-family: Arial;">{download_list} <br /><br /><a href="{receipt_link}">View Actual Purchase Receipt</a></p>
</div>
