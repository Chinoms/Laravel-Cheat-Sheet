# Laravel-Cheat-Sheet
A place where I dump all the Laravel snippets I always forget but always need.

### Inserting 'active' Class in a URL
The following example check for either of two conditions using the Terneary operator.  

```<li class="nav-item  {{ (request()->is('profile')) || request()->is('edit-profile') ? 'active' : '' }}">```  


The next example checks for a single condition  

```<li class="{{ (request()->is('profile')) ? 'active' : '' }}">```


### Send email
``` Mail::to($request->email)->send(new PatientRegistered);```
