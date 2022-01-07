# Reading

## Django Forms

Django forms, just as in HTML, provide an obvious collection point for an user to submit information. Any of the expected HTML forms can
likewise be found in Django, such as text boxes, radio buttons, email fields, etc. The Django Admin page is full of forms.  

While the similarities between Django and HTML forms are plenty, Django walks away with some serious benefits. Here is a short list of the
work Django takes care of for you:

- Validating data
- Reposting with Error Message
- Responding with success messages
- Data handling upon submission

Now, let's look at how Django does it. 

### Form Handling

1. An untouched, or __unbound__ form is displayed the first time it is requested. 
2. The user data is bound to the form upon a submission. This information and any errors will be redisplayed when the time comes. 
3. The data is cleaned and validated. This means invalid characters are removed and converted to Python types. 
4. At this point, anything that is still invalid will cause the bound form to be re-rendered with the error messages. 
5. The user has a chance to make corrections and resubmit. 
6. If everything checks out, the ___actions___ are carried out and the user
is redirected. 

### Declaring a Form

The syntax may seem familiar to declaring a Model. See below.

```
from django import forms

class ReviewForm(forms.Form):
  review = forms.CharField(help_text="Leave your review here.", max_length=265)
```

### Validation

#### clean_<fieldname>()
  
Django provides a simple way to validate a single field. Using the example of the form above we could create a method...
```
  def clean_review(self):
    data = self.cleaned_data['review']
  
    return data
```
  
Note you always get the clean data using self.cleaned_data['<data_name>']
  
### View
  
  It is important for view to know if it is being called the first time or not so it can render the proper form. For forms that use POST, 
  the request method is evaluated. 


  ```
import datetime

from django.shortcuts import render, get_object_or_404
from django.http import HttpResponseRedirect
from django.urls import reverse

from catalog.forms import RenewBookForm

def renew_book_librarian(request, pk):
    book_instance = get_object_or_404(BookInstance, pk=pk)

    # If this is a POST request then process the Form data
    if request.method == 'POST':

        # Create a form instance and populate it with data from the request (binding):
        form = RenewBookForm(request.POST)

        # Check if the form is valid:
        if form.is_valid():
            # process the data in form.cleaned_data as required (here we just write it to the model due_back field)
            book_instance.due_back = form.cleaned_data['renewal_date']
            book_instance.save()

            # redirect to a new URL:
            return HttpResponseRedirect(reverse('all-borrowed') )

    # If this is a GET (or any other method) create the default form.
    else:
        proposed_renewal_date = datetime.date.today() + datetime.timedelta(weeks=3)
        form = RenewBookForm(initial={'renewal_date': proposed_renewal_date})

    context = {
        'form': form,
        'book_instance': book_instance,
    }

    return render(request, 'catalog/book_renew_librarian.html', context)
  ```
   source: https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms
  
  As we can see above, the first time the user visits the site, a GET request would retrieve the form, so the else block is fired, retrieving
  a default form. Once the user fills out the form, the submit button would be pressed, and the action would be a POST request, firing off 
  the first if block and it's nested code blocks. 
  

  
