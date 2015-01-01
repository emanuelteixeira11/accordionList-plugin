AccordionList-plugin
====================
This plugin has the functionality to organize several sections, arranged by title and their respective content. It was written in **Javascript** using the **jQuery** library.

**Demo:** [Website demo](http://emanuelteixeira.16mb.com/plugin/demo/)

![alt text](http://emanuelteixeira.16mb.com/plugin/img/list.png "Logo Title Text 1")
![alt text](http://emanuelteixeira.16mb.com/plugin/img/list-open.png "Logo Title Text 1")
Installation
-------------
**Call the jquery library**

*From web:*
```javascript
<script src="//ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
```
*From local path:*
```javascript
<script src="js/jquery.min.js"></script>
```

**Call acordionList script**

*From web:*
```javascript
<script src="http://emanuelteixeira.16mb.com/plugin/js/accordion.js"></script>
```
*From local path:*
```javascript
<script src="js/accordion.js""></script>
```

**Call acordionList style sheet**
```javascript
<link href="css/style.css" rel="stylesheet" type="text/css">
```

**To add more resources add font awesome** 

*From web:*
```javascript
<link href="//maxcdn.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.min.css" rel="stylesheet">
```

Usage
-------
Create container section:
```javascript
<section id="accordion">
```

Create content section:
```javascript
<div data-type="accordion-section">
```
Create content title:
```javascript
<h3 data-type="accordion-section-title">Example</h3>
```
Create inside content:
```javascript
<div data-type="accordion-section-body">
```

####Extra Resources

Create search box:
```javascript
<input type="text" placeholder="search in list" name="search" id="search" data-type="accordion-search">
```
Important: For search into contents use *"keyword"*. If you search without *""* find on titles.

Create filter:
```javascript
<select data-type="accordion-filter">
    <option value="default">all</option>
    <option value="type1">Type 1</option>
    <option value="type2">Type 2</option>
</select>
```
Important: use *default* value for search *all*.

Create ordering buttons:
```javascript
<button data-type="accordion-ordering" ordering="asc"></button>
<button data-type="accordion-ordering" ordering="desc"></button>
```
Important: Only work with font awesome.

Call accordion funtion
---------------------
```javascript
<script>
    $(document).ready(function () {
        $("#accordion").accordion();
    });
</script>
```

Author
------
[Emanuel Teixeira](https://github.com/emanuelteixeira11)
