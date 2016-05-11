Uninstall Delivery Date time
=============================



Delete the following files, folders::

	app/etc/modules/Magecheckout_DeliveryTime.xml
	app/code/local/Magecheckout/DeliveryTime
	app/design/adminhtml/default/default/layout/magecheckout/DeliveryTime.xml
	app/design/adminhtml/default/default/template/magecheckout/DeliveryTime
	app/design/frontend/base/default/layout/magecheckout
	app/design/frontend/base/default/template/magecheckout/DeliveryTime
	js/magecheckout/DeliveryTime
	skin/frontend/base/default/css/magecheckout/DeliveryTime
	skin/frontend/base/default/js/magecheckout/DeliveryTime

Run the following SQL::

	DROP TABLE magecheckout_deliverytime
	DROP TABLE magecheckout_deliverytime_rule
	DELETE FROM core_resource WHERE `code` LIKE 'magecheckout_deliverytime_setup'



