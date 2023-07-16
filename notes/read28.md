# Q1. How do Django Forms facilitate user input handling, and what are some key components of creating a form using the Django framework?

Display the default form the first time it is requested by the user<br>

Receive data from a submit request and bind it to the form<br>

Clean and validate the data<br>
If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.<br>

If all data is valid, perform required actions (such as save the data, send an email, return the result of a search, upload a file, and so on).<br>

Once all actions are complete, redirect the user to another page.<br>

# Q2. Explain the purpose of Django Templates in web development and describe how template inheritance can be utilized to improve code reusability and maintainability.

A template is a text file that defines the structure or layout of a file (such as an HTML page), it uses placeholders to represent actual content.<br>

A Django application created using startapp (like the skeleton of this example) will look for templates in a subdirectory named 'templates' of your applications. For example, in the index view that we just added, the render() function will expect to find the file index.html in /locallibrary/catalog/templates/ and will raise an error if the file is not present.

# Q3. Describe the function of Django Views in handling HTTP requests, and outline the differences between function-based views and class-based views.
Function Based Views<br>
Pros<br>
Simple to implement<br>
Easy to read<br>
Explicit code flow<br>
Straightforward usage of decorators<br>
good for one-off or specialized functionality<br>
Cons<br>
Hard to extend and reuse the code<br>
Handling of HTTP methods via conditional branching<br>

Class Based Views<br>
Class-based views provide an alternative way to implement views as Python objects instead of functions. They do not replace function-based views, but have certain differences and advantages when compared to function-based views.<br>

Pros<br>
Code reuseability — In CBV, a view class can be inherited by another view class and modified for a different use case.<br>
DRY — Using CBVs help to reduce code duplication<br>
Code extendability — CBV can be extended to include more functionalities using Mixins<br>
Code structuring — In CBVs A class based view helps you respond to different http request with different class instance methods instead of conditional branching statements inside a single function based view.<br>
Built-in generic class-based views<br>
Cons<br>
Harder to read<br>
Implicit code flow<br>
Use of view decorators require extra import, or method override<br>
