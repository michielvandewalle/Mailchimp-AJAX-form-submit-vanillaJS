# Mailchimp AJAX form submit vanillaJS

Only 0.3KB 

Subscribe to a mailchimp newsletter list. Lightweight and easy to implement. Here is a [Codepen example](https://codepen.io/michielvandewalle/pen/oeoMXg "Codepen")

### HTML
The required form fields for mailchimp such as the email, need to be wrapped in the container with id `#js-form-inputs`

**Form fields markup**
```$html
<div id="js-form-inputs">
    <div>
        <label for="mce-EMAIL">Email Address<sup>*</sup></label>
        <input type="email" name="EMAIL" id="mce-EMAIL" value="">
    </div>
    <div>
        <label for="mce-FNAME">First Name </label>
        <input type="text" name="FNAME" id="mce-FNAME" value="">
    </div>
    <div>
        <label for="mce-LNAME">Last Name </label>
        <input type="text" name="LNAME" id="mce-LNAME" value="">
    </div>
</div>

```

### Form action markup
Change the endpoint of the form action to your mailchimp newsletter list. You can find this url in mailchimp under Signup forms > Embeded forms.

**important**
- form action starts with `http://`
- form action ends with `c=callback`

```$html
<form action="http://XXX-URL-XXX.XXX.list-manage.com/subscribe/post?u=XXXXXXXXXXXXXXXXXXXXXXXX&amp;id=XXXXXXXXXX&amp;c=callback"> ... </form>
```

### Example
Check out [Codepen example](https://codepen.io/michielvandewalle/pen/oeoMXg "Codepen")
![Mailchimp newsletter subscribe with](https://d26dzxoao6i3hh.cloudfront.net/items/3g0W0u0y0o2b0c2Q0l27/Screen%20Recording%202017-07-27%20at%2005.56%20PM.gif?v=0cae79bf "Mailchimp subscribe")
