# Refactor Goals and Report

## Goals and Reqs

The goal was to refactor the webpage of Horiseon webpage to become more accesible by implementing more intuitve and structured elements within the codebase of the site and create a cleaner codebase with best practices to allow further development

### Therefore,

the acceptance criteria is as follows
~~~
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
~~~

## The Process

### Inspection & Review

Upon looking at the site and the codebase,
we can find many different issues.

* On the site we can find links in the header that navigate user to sections of the page, with the subsquent "SEO" link broken.

* The HTML file separates all portions into 'div' instead of semantic elements .

* The CSS files have redundant classes that repeat the same functions and declarations.

* Lack of alt img text for accessibility users.


### Refactoring

Knowing these issues we begin to improve the code

#### CSS File

To make a more efficent CSS file we look through all the classes and see which ones have identical declarations within them. Once we identify them we can take one of them to rename into a class that represents the function of the class to apply to the similar elements in the HTML file. Once we rename and remove the redundant code we head back to the HTML file and apply the class to all nescessary HTML elements.

#### HTML File

Looking over the HTML file practically all of the webpage was sections into 'div's instead of descriptive semantic elements. We implemented a header, main, an aside, nav and a footer. We also had to add descriptive alt text of the associated image to provide information to those that need the accessibility features. It is worth mentioning again that the classes used within the HTML file had to be redirected to the appropriate classes after being renamed in the CSS file for efficecy. The broken "SEO" navigation link was due to a missing id tag in the appropriate section to be called on.

### Conclusion

Implementing the changes, the site looks practically the same, but behind the scenes it has been improved upon in the codebase to ease future development of the sight and includes mores accessibility features for those that use such applications. The navigation bar is currently fully functional and has no issues.

#### Future Improvements

Possible to improve the sizing and layout of the website through diffrent aspects and dimensions to avoid issues of viewing on different windows and devices.


Link to webpage : https://jaketnguyen.github.io/refactor-horiseon-webpage/