# validation-for-prototypes
 Validation plugin for GOVUK Prototypes, based on abbott567 version:

 https://github.com/abbott567/validation-for-prototypes#validation-plugin-for-govuk-prototypes

 **Currently works only for radio and checkboxes.

 ###WARNING: For prototypes only. Do not use in production under any circumstances


### How does it work?

The plugin uses jQuery to check any `<fieldset>` tags you have applied the data attribute of `data-required` to. It then checks you have made a selection or entered some characters. If the validation fails, the browser scrolls to the top of the page and shows the error message.

Custom error messages can be passed in with `data-error="custom error message text"`.

### Installation

1) Download the file validation.js and put it into the directory `app/assets/javascripts`.

2) In your `scripts.html` file, which is located in the `app/views/includes` directory, paste the following code at the end:

``` javascript
  <script src="/public/javascripts/validation.js"></script>
```

Add the following to any radio or checkboxes `<fieldset>`
```HTML
data-required data-error="Custom error message text here"
```

Check the `validation-example.html` to see examples. 

That's it! Happy validating.

### Markup examples

In order to make the validation work, your HTML markup must be correct.
