==========================================
 Real Multi Website (eCommerce extension)
==========================================

Installation
============

* `Install <https://odoo-development.readthedocs.io/en/latest/odoo/usage/install-module.html>`__ this module in a usual way

Configuration
=============

Follow instruction of the base module `Real Multi Website <https://www.odoo.com/apps/modules/10.0/website_multi_company/>`__.

Multi-categories
----------------
* Open menu ``[[ Website Admin ]] >> Configuration >> eCommerce >> Website Product Categories``
* Only for top-level (i.e. without ``parent_id``) categories: specify **Websites** field

Multi-products
--------------
* Open menu ``[[ Sales ]] >> Sales >> Products``
* Specify **Allowed websites** for your products
* Websites company and product company should be equal. But if you want different company websites then leave the **Company** field empty in your product - in such case you can specify any websites


Usage
=====

Multi-categories
----------------

* Open shop at some of your websites
* Login as Administrator
* In ``Customize`` section activate ``[x] Product Categories``
* RESULT: parent categories for current website and categories without value at **Websites** fields are shown only. **Websites** value of child categories are ignored.

Multi-cart
----------

* Login as portal or internal user at some of your websites
* Add some products to the cart
* Open another website that belongs to another company
* Login as the same user
* RESULT: you have empty cart, rather than one from previous website

Multi-products
--------------

* Open website shop
* RESULT: you should only see products allowed for this website or products with no websites specified
