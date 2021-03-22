# OC.
My OpenCart2.
Template - Kingstore Lite
https://www.opencart.com/index.php?Route=MarketPlace/extension/info&extension_id=22604&filter_license=free&filter_download_id=41

Removed FAX and Company field
/theme/kingstorepro/template/checkout/guest.tpl
/theme/kingstorepro/template/checkout/register.tpl
Line:
<label class = "Control-Label" for = "input-payment-fax"> <? php echo $ entry_fax; ?> </ label>
<input type = "text" name = "fax" value = "" placeholder = "<? php echo $ entry_fax;?> ID =" INPUT-payment-Fax "class =" Form-Control "/>

Remove the support of several languages ​​and currencies
I decided to do through the change in the controller, passing into the DATA array only one language or one currency, although it is better to change the STATUS column in the database
Place if ($ result [Status']) Now if ($ result ['Code'] == "USD").



Remove user support:
I hid in the Footer "E block Customer Service, because they were 5 horizontally, connected an additional bootstrap-file and stretched 5 in length.

Bring the schedule of visits on the main page
