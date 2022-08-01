# HTML Form Methods

## Learning Goals

- Define radio inputs
- Define checkbox inputs
- Define select inputs
- Define textarea

## Introduction

While text inputs and buttons alone are already powerful for collecting data from users, sometimes we want our forms to be more specific. Thankfully, HTML provides several different input types to help with that. Let's learn about a few more.

### Telephone Inputs

Creating an `input` tag with `type="tel"` behaves like a text field, but will
bring up the numeric keypad on supported mobile devices.

```html
<label for="tel">Where should E.T. &trade; Phone Home?</label>
<input id="tel" type="tel" name="phone" placeholder="Phone Number" />
```

### Radio Inputs

Radio inputs show users many options. But radio buttons allow users to select
only one. You will set different `value` attributes for each radio button, but
they _must_ have the same `name` attribute.

```html
<h3>Does your dog get along with other dogs?</h3>
<input type="radio" name="plays-well-with-others" value="high" /> The more dogs,
the better!<br />
<input type="radio" name="plays-well-with-others" value="medium" /> It depends
on the dog, but generally they are ok<br />
<input type="radio" name="plays-well-with-others" value="low" /> My dog prefers
their walkies solo<br />
```

Here's a screenshot:

![Image of radio input](https://curriculum-content.s3.amazonaws.com/web-development/fewds-html-forms/radio_input.png)

### Checkboxes

Checkboxes are like radio buttons...but you can choose more than one.

```html
<h3>What are your dogs favorite toys?</h3>
<input type="checkbox" name="toy-1" value="kong" /> Kong <br />
<input type="checkbox" name="toy-2" value="stuffed-animals" />Stuffed Animals<br />
<input type="checkbox" name="toy-3" value="rope-toys" />Rope Toys<br />
<input type="checkbox" name="toy-4" value="squeaky-toys" />Squeaky Toys<br />
<input type="checkbox" name="toy-5" value="balls" />Balls, Frisbees, anything a
dog can fetch!<br />
```

Here's a screenshot:

![Image of the checkbox input](https://curriculum-content.s3.amazonaws.com/web-development/fewds-html-forms/checkbox_input.png)

### Select Menus

This is pretty advanced!

Select menus create a drop-down menu. Inside the `select` tag you use `option`
tags to create a menu. Inside the `option` tag you say what will be shown in
the menu. In the `value` option you say what will be sent as part of the _Query
String_. For the example below the _Query String_ would contain `size="small"`.

```html
<h3>What size is your dog?</h3>
<select name="size">
  <option value="small" selected>Small(0-25 pounds)</option>
  <option value="medium">Medium (26-50 pounds)</option>
  <option value="large">Large (51-75 pounds)</option>
  <option value="x-large">Extra Large (over 75 pounds)</option>
</select>
```

Here's a screenshot:

![Image of select input](https://curriculum-content.s3.amazonaws.com/web-development/fewds-html-forms/select_input.png)

### Textarea

Textarea elements are useful if we want our users to be able to be able to write
multiple lines of text. For example, if we wish to allow our clients to write
special notes for their dogs, we can let them write as much or as little as they
like.

```html
<h3>Any other things we should know about your dog?</h3>
<textarea name="message"></textarea>
```

Here's a screenshot:

![Image of textarea input](https://curriculum-content.s3.amazonaws.com/web-development/fewds-html-forms/textarea_input.png)

## Conclusion

Where appropriate, having a variety of inputs can make your forms more clear to users when simple text inputs are just not enough. With these extra types, you'll be able to decide which `input` is best for the data you're reuqesting. 

## Resources

- [MDN - The HTML5 Input Types](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)
- [W3School - HTML Input Types](https://www.w3schools.com/html/html_form_input_types.asp)
