# OC
my opencart2
шаблон - KINGSTORE Lite
https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=22604&filter_license=free&filter_download_id=41

удалено поле Fax и Company  
/theme/kingstorepro/template/checkout/guest.tpl
/theme/kingstorepro/template/checkout/register.tpl 
строчки:
<label class="control-label" for="input-payment-fax"><?php echo $entry_fax; ?></label>
<input type="text" name="fax" value="" placeholder="<?php echo $entry_fax; ?>" id="input-payment-fax" class="form-control"/>

Убрать поддержку нескольких языков и валют
решил сделать через изменение в контроллере, передавая в массив data только один язык или одну валюту, хотя лучше наверно изменить в базе данных колонку status
место if ($result['status']) теперь if($result['code']=="USD").



Убрать поддержку пользователей:
Скрыл в footer"е блок Customer Service, поскольку их стало 5 горизонтально, подключил дополнительный bootstrap-файл и растянул 5 по длинне.


Вывести на главной страницу график посещений
