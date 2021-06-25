**LOGIC OF THE CODE**

**FIRST** in **Line 5**-The Script element- The script HTML element is
used to embed executable code or data; this is typically used to embed
or refer to JavaScript code.What I used inside script was that its for
calling the javascript library jQuery.src is the name of the attribute
and the jQuery library calling thing is the value,this attribute is
basically used to contain the url of several things,can be that of a
file,a library calling,a set of images in other website.Here it is used
for calling the jQuery library of JavaScript so that its functions can
be used to extract informations from the json file.I could also have
written this line inside the script tag of the body of the code other
than the head of the code.If this line is not coded,the code won't run
as the compiler would recognise the functions of jQuery library.

**SECOND** in **Line 10**-ul tag is used for creating an unordered list
and then id is used for an identifier to be used uniquely in the entire
code.Here I want to display the images extracted form the json file as a
list.

**THIRD** in **Line 13**-I used the function
\$.getJSON(url,function(success) which is a function of the jQuery
library of JavaScript.The url is a string containing the URL to which
the request is sent.The success is an object that represents key/value
pairs that will be sent to the server.We could also have writtwn the
name of a .json file in place of the url if stored locally.This function
is used for requesting access or calling the url of .json file.

**FOURTH** in **Lines 14 and 15**-I declared the array variables
childrens and urls-childrens is used to access the data inside children
object of the json file inside data.And urls is an **undefined** or
dynamic array variable which will be used for storing the urls of all
the images onr by one as they are extracted.

**FIFTH** in **Line 16-23**-The **for..of** command is used in
JavaScript to iterate a loop over iterable objects,in this case an array
variable childrens and inside one for loop is another(nested).From the
.json file, I came to know that the urls of images are located in this
navigation data-children-data-preview-data-source-url.The urls inside
this needed to be extracted so I used urls.push function.This function
will add the urls one by one at te end of the array urls and will give
the length each time.

**SIXTH** in **Line 26-29**-**each** function is a function used in
jQuery of JavaScript for calling any function used in the code for each
element of the array.Here I called the function in Line 13 for each
element in array image giving its index location. and finally the urls
are getting stored and now we need to display it in the form of a
list.The append keyword is used to add images one by one.This new
AnythingSlider is an attempt at bringing together the functionality of
all of those previous sliders and adding new features.

**This was the logic of the code I used**
