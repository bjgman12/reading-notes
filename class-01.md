# HTML 
[Home](README.md)
- Hyper Text Markup Language
- **Semantic HTML** name implies function nav = navigation
  - body
    - **Content** -- goes inside of elements
    - header 
    - footer 
    - nav 
    - div
- tags - opening and closing `<p>` content `</p>`
- attributes -- examples: language,style(not advised),id,class,src,rel
- .
- Meta
- Personas -- user demographicsgit 
- Structure vs Presentation


HTML is the bones of the site


## HTML Reading NOTES

### Process and Design

### Who is the site for?

##### Target Audience

- age range
- country of access
- gender demo
- average level of education
- occupation
- hours of work week

### Why are people visiting?

- to achieve a specific goal
- entertainment
- general information
- information on a specific product or service

### What information do visitors need?

- are visitors familiar with information or will they need to be introduced to it?
- important features of site
- what differentiates your site

<is the site you are building one that will need to be updated often by nature ?>

### Site Maps

- important to think about what your visitors might aswsume about the sites layout


### Wireframes

- a simple sketch of the key elements of your site

<img src="tplate.PNG" alt="wireframe exapmle" width="550" height="350">


### Chapter 17 notes

#### Articles

- can be used to encapsulate any section of a page that could stand alone as content
- can nest images headers paragraphs and mroe

#### Asides

- are used primarily for complementary content such as pullquotes on an article

### Chapter 8

- `<!-- this is comment syntax HTML-->`
- IDs can be used for single out a single portion of your page
- iframes are small windows in you page in which you can veiw a seperate page
- ` <iframe width= height= src=></iframe>`
- conditionals
  - if
  - else
- operators ( + - = *)
- data types
  - string
  - boolean
  - number
- variable` var` `x = 42`, `UserName = Brandon`

## Objects and methods

- the document object represents the entire page
- write() method allows new conent wherever the `<Script>` element sits
- parameters go inside methods

<img src ="js example.jpg">

- java script will run where it is found in the html
- comment are done like C++ with a `//`
- store variable into strings bye using  ' string here'

``` 
var today = new Date();
var hourNow = today.getHours();
var greeting;


if (hourNow > 18) {
    greeting = 'Good Evening G!';
} else if ( hourNow > 12){
    greeting = 'Good Afternoon Playa!';
} else if (hourNow > 0){
    greeting = ' Good Morning Sunshine!';
} else {
    gretting = ' Welcome Sir ...';
}

document.write('<h3>'+ greeting + '</h3>')
```