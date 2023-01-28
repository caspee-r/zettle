
#### categories: #css 
#### created: 2023-01-27
---
- when a top and / or bottom margins are adjoining, they *overlap* and combining to form a single margin.
- the size of a collapsed margin is equal to the largest of the joined margins, for instance: 
  
```html 
<div> Some Shit </div>
<p> Another Shit </p>
```

``` css
div {
margin-bottom:1em;
}
p {
margin-top:2em;
}
```
**The collapsed margin will equals to 2em**
## collapsing multiple margins
element don’t have to be *adjacent siblings*  for their margin to collapse :
``` html
<div> The Same Shit </div>
<div><p>The Same another shit</p></div>
```
in this case there is 3 different margins collapsing together,
1. the bottom margin of the first div
2. the top margin of the second div
3. the top margin of the paragraph
==The collapsed margin between the elements only appears larger if the following element requires more space. 
> [!note] 
> Margin collapsing only occurs with top and bottom margins. Left and right margins don’t collapse.  

> [!success] 
> padding can solve this  collapse 

>  

---
### references
