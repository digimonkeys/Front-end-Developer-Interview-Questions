
* When creating a directive, it can be used in several different ways in the view. Which ways for using a directive do you know? How do you define the way your directive will be used?  
When you create a directive, it can be used as an attribute, element or class name. To define which way to use, you need to set the restrict option in your directive declaration.  
The restrict option is typically set to:  
‘A’ – only matches attribute name  
‘E’ – only matches element name  
‘C’ – only matches class name  
'M' - only matches comment  
These restrictions can all be combined as needed:  
‘AEC’ – matches either attribute or element or class name  
