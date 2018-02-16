# BEM (http://getbem.com/)
BEM (Block Element Modifier) 
- It's for naming rules in the CSS 
- Using proper naming will prepare you for the changes in design of the website.

##Block

- Use class name selector only
- No tag name or ids
- No dependency on other blocks/elements on a page

```
<div class="block">...</div>
```
```
.block { color: #042; }
```



##Element
- Use class name selector only
- No tag name or ids
- No dependency on other blocks/elements on a page
```
<div class="block">
	  ...
	  <span class="block__elem"></span>
	</div>
```
####Good
```
.block__elem { color: #042; }
```
####Bad
```
.block .block__elem { color: #042; }
	div.block__elem { color: #042; }
```



##Modifier
- .block--mod
- .block__elem--mod
- .block--color-black 
