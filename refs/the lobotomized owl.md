
#### categories: #css
#### created: 2023-01-28
---
a way to fix margins for a page no matter how the page gets restructured.
Web designer Heydon Pickering once said margins are “like applying glue to one side of an object before you’ve determined whether you actually want to stick it to something or what that something might be.” 
`* + *` this is the *lobotomized owl selector*, it targets any element that immediately follows any other element. That is, it selects all elements on the page that aren’t the first child of their parent. 
it looks like this:
``` css
body * + * {
	margin-top:1.5em;
}

```

> [!note] 
> Using the lobotomized owl like this is a tradeoff. It simplifies many margins throughout your page, but you’ll have to override it in places where you don’t want it to apply.  








---
### references
- 
