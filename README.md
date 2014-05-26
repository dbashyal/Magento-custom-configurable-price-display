Magento Display Custom Configurable Price on product options
============================================================

[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=dbashyal&url=https://github.com/dbashyal&title=Github Repos&language=&tags=github&category=software)

I am playing around price.phtml to display 'from' on the configurable products.

for more information visit: http://dltr.org/blog/magento/254/Magento-show-FROM-price-on-configurable-products

if you want to use skin...js/varien/configurable.js

you need to update catalog.xml

find
```xml
	<action method="addJs"><script>varien/configurable.js</script></action>
```

and replace with
```xml
	<!--<action method="addJs"><script>varien/configurable.js</script></action>-->
	<action method="addItem"><type>skin_js</type><name>js/varien/configurable.js</name></action>
```
