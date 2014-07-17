jquery-mobile-pull-to-refresh---jqPTR
=====================================

This is good for HTML mobile developed apps using Phonegap or something similar.

Requirements
=====================================
 - jquery            http://jquery.com/download/
 - jquery mobile     http://jquerymobile.com/download/
 
How to:
=====================================
In the header you must include ptr.css and ptr.js. After that you will use the function like this:

jqPTR([target], [callback]);

jqPTR('ptr',function (){ 
	console.log('Done!'); 
	
	// usually you call just jqPTR_refresh(); 
	// I've added setTimeout because I do not have to wait for an ajax call response
	setTimeout(jqPTR_refresh, 1000); 
});
