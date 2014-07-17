jquery-mobile-pull-to-refresh---jqPTR
=====================================

This is good for HTML mobile developed apps using Phonegap or something similar.

Requirements
=====================================
 - jquery            http://jquery.com/download/
 - jquery mobile     http://jquerymobile.com/download/
 
How to:
=====================================
In the header you must include <strong>ptr.css</strong> and <strong>ptr.js</strong>. After that you will use the function like this:

<pre>jqPTR([target_id], [callback]);</pre>

<pre>
jqPTR('ptr',function (){ 
	console.log('Done!'); 
	
	// usually you call just jqPTR_refresh(); 
	// I've added setTimeout because I do not have to wait for an ajax call response
	setTimeout(jqPTR_refresh, 1000); 
});
</pre>

Demo:
=====================================
If you unzip the files you have a working demo. You can also check it out on http://dev.alurosu.com/ptr/.
