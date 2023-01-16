# getting started with css
#### status: 
#### created: 2022-07-01
---
#### The box model
the *css* language consider all of the *html* elements as **boxes**, so it's modeling all the elements to boxes, this modeling feature make it easy to applies styles and manipulate those elements.

##### properties 
it's consistence from 4 parts or area:
1. **the content**
2. **the padding**
3. **the border**
4. **the margin**
<img src="https://cdncontribute.geeksforgeeks.org/wp-content/uploads/box-model-1.png">

a good *analogy* to understand this model is :
<img src="https://web-dev.imgix.net/image/VbAJIREinuYvovrBzzvEyZOpw5w1/FBaaJXdnuSkvOx1nB0CB.jpg?auto=format&w=845">
- *the content* is the **artwork** 
- *padding* is the white space between the frame and the artwork 
- the *border* is the frame 
- the *margin* is the space between each frame 

==the browser will calc the area of the box according to the value of *box-sizing* property the default for most is *content-box* which will add the padding and the border to the box area==
###### content
1. we can controll the sizing a content by *width* and *height*generally when the content is larger than the box dimension the default behavior of the box is to grow with its content and this due to the default value of *width* and *height* which is *min-content*	we can also provide *min|max-width* and *min|max height* 
2. when the box dimension are setting and content goes far than the box size , here the content will **overflowing**, we can prevent this behavior by setting the *overflow* property to auto which is the default and this will add a X or Y or both scroll bar to the box 

###### padding
1. the padding area surround the content and we can control it by the *padding* property .
2. the padding area get affected by the *background* property because it is inside the box 
3. if we have a scrollbar, then it occupied the padding 

###### border
 the border is the area that surround the padding area and we use the *border* property to manipulate it , **the border edge** is the limit where we can visually see.

###### margin
 is the last area . we define it by the *margin* property 

---
### referances
-[[@BoxModel]] 
