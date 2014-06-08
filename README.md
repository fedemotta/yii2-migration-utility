Yii2 Migration Utility
===================

This is a simple utility that writes the create table statement for you.
The table(s) must already exist.

It automatically writes out all:

+ tables
+ columns
+ column types
+ column defaults
+ primary keys
+ foreign key
+ ***does not*** add indexes

***Note:*** Foreign keys default to CASCADE / DELETE so you may need to manually change these.

***Note:*** <span style="color:red;">$tableOptions</span> is added so make sure you have a var set.
Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist "c006/yii2-migration-utility" "dev-master"
```

or add

```
"c006/yii2-migration-utility": "dev-master"
```

to the require section of your `composer.json` file.


Required
--------

+ ***MySQL***

Currently this is only setup to MySQL.

Update either ***config/web.php*** (basic) or ***config/main.php*** (advanced)

>
        'modules'    => [
            ...
            ...
            ...
            'utility' => [
                'class' => 'c006\utility\migration\Module',
            ],
        ],



The tables must already exist in website schema.



Usage
-----

Demo: [http://demo.c006.us/index.php?r=demo/migration-utility](http://demo.c006.us/index.php?r=demo/migration-utility)

##http://<span style="color:red;">[Your_Domain]</span>/utility/index##

Workbench showing the user table:

![alt text](http://demo.c006.us/images/yii2-migration-utility/workbench.jpg)


Image of demo page:

![alt text](http://demo.c006.us/images/yii2-migration-utility/output.jpg)



To Do
------

Add table data insert statements

Comments / Suggestions
--------------------

Please provide any helpful feedback or requests.

Thanks.

































