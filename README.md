# TableHeadFixer
### About
TableHeadFixer is a simple [jQuery](http:/jquery.com/ "jQuery") plugin for fixer HTML tables header, footer or columns.<br/>
This plugin will only add elements events and css attributes necessary for fix tables header, footer or columns, you can customize styles of your table, this plugin will not influence style of table (width, height, background, font color, etc...)

### Require (Importante!)
- [jQuery](http:/jquery.com/ "jQuery")

### Get Starting
For use <b>TableHeadFixer</b> plugin, is require include <b>jQuery</b> in your page.<br/>
After included <b>jQuery</b> in your page, just include <b>TableHeadFixer</b> plugin and call <b>.tableHeadFixer([param])</b> function after page rendered.

### Example:
#### Fix Table Header
    // get your table with jQuery selector
    $("#fixTable").tableHeadFixer();

### Fix First Left Column
By default, table header is fixed when <b>.tableHeadFixer()</b> function is called, if you need fix only footer or columns, is necessary disable head fix by parameter.

	$("#fixTable").tableHeadFixer({'left' : 1, 'head' : false});

### Fix Two Left Columns
	$("#fixTable").tableHeadFixer({'left' : 2, 'head' : false});

### Fix Table Header and First Right Column
	$("#fixTable").tableHeadFixer({'right' : 1});

### Fix Table Header and Footer
	$("#fixTable").tableHeadFixer({'foot' : true});

### Fix Multiple Rows in Header or Footer
For fix multiple rows in header or footer, is only add new <code>tr</code> in the header or footer, all <code>tr</code> is will be fixed.