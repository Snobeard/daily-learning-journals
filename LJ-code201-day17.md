# LJ Code 201 - Day 17

#### Creating / Adding Elements
- var myForm= document.getElementById('form');
- myForm.insertBefore(<i>element</i>, myForm.childNodes[0]); - adds an element as the first child element, or respective numeric value

#### Accent lines (adjacent to text element)

###### HTML

< section id="title" >   
  < h1>< span > Your Title < /span >< /h1 >    
< /section >

###### CSS

\#title span {    
  position: relative;   
}

\#title span::before,     
\#title span::after {   
  content: '';    
  position: absolute;   
  border-top: 1px solid white;    
  top: 50%;     
  width: 200px;   
}

\#title span::before {     
  right: 100%;    
  margin-right: 15px;   
}

\#title span::after {   
  left: 100%;   
  margin-left: 15px;    
}
