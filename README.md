# magento2-featured-products

<h2>Composer Installation Instructions</h2>
edit composer.json file of the Magento 2 project
edit to the following in repositories section 
<pre>
"repositories": [
        {
            "type": "composer",
            "url": "https://repo.magento.com/"
        },
        {
            "type": "vcs",
            "url": "https://github.com/witiva/magento2-featured-products-widget"
        }
    ],
</pre>

Since this package is in a development stage, you will need to change the minimum-stability as well to the composer.json file: -
<pre>
"minimum-stability": "dev",
</pre>

After that, need to install this module as follows:
<pre>
  composer require magento/magento-composer-installer
  composer require witiva/featuredwidget
</pre>


<br/>
<h2> Mannual Installation Instructions</h2>
go to Magento2Project root dir 
create following Directory Structure :<br/>
<strong>/Magento2Project/app/code/Witiva/Featuredwidget</strong>
you can also create by following command:
<pre>
cd /Magento2Project
mkdir app/code/Witiva
mkdir app/code/Witiva/Featuredwidget
</pre>



<h3> Enable Witiva/Featuredwidget Module</h3>
to Enable this module you need to follow these steps:

<ul>
<li>
<strong>Enable the Module</strong>
<pre>bin/magento module:enable Witiva_Featuredwidget</pre></li>
<li>
<strong>Run Upgrade Setup</strong>
<pre>bin/magento setup:upgrade</pre></li>
<li>
<strong>Re-Compile (in-case you have compilation enabled)</strong>
	<pre>bin/magento setup:di:compile</pre>
</li>
</ul>
