<p align="center"><img src="https://user-images.githubusercontent.com/15963/61768669-f34e2900-ad9c-11e9-8831-8a7fb1975cd0.png" width="80" height="80" alt="AMP logo"></p>


# Simple AMP for Email Templates

* [Getting started with AMP for Email](https://htmlemail.io/blog/getting-started-amp-for-email)
* [HTML support](https://github.com/ampproject/amphtml/blob/master/spec/email/amp-email-html.md) for AMP emails
* [CSS support](https://github.com/ampproject/amphtml/blob/master/spec/email/amp-email-css.md) for AMP emails

## Getting Started

* Open the [Gmail AMP for Email Playground](https://amp.gmail.dev/playground/)
* Copy/paste one of the templates and you'll see it rendered
* Hit send and it will be sent to your email

![image](https://user-images.githubusercontent.com/15963/61768315-f5fc4e80-ad9b-11e9-969f-9df4208bacb0.png)

_Note: The starting template used was a clone of [this HTML template](https://github.com/leemunroe/responsive-html-email-template). You do not necessarily need all the markup included in these templates for AMP emails to work correctly._

## You will need to configure your Gmail to receive AMP emails

* Go to **Settings > General > Dynamic email**
* Check **Enable dynamic email**
* Click **Developer Settings**
* Add `amp@gmail.dev` as the Sender Email Address
* Save your changes

![img](https://htmlemail.io/img/post-amp/amp3.jpg)

# Examples

## Simple hello world with image

![image](https://user-images.githubusercontent.com/15963/61767788-3ce94480-ad9a-11e9-97c4-cf28eafed4bf.png)

```html
<amp-img src="https://i.imgur.com/3NmrJA1.png"
  alt="photo description"
  width="500"
  height="380">
</amp-img>
```

## AMP carousel

![carousel-gmail](https://user-images.githubusercontent.com/15963/61767879-7621b480-ad9a-11e9-97b9-8a964c9fdf67.gif)

```html
<script async custom-element="amp-carousel" src="https://cdn.ampproject.org/v0/amp-carousel-0.1.js"></script>
```
```html
<amp-carousel width="500"
  height="380"
  layout="responsive"
  type="slides"
  controls>
  <amp-img src="https://i.imgur.com/Its6yBO.png"
    alt="photo description"
    width="500"
    height="380">
  </amp-img>
  <amp-img src="https://i.imgur.com/hUYQ4bi.png"
    alt="photo description"
    width="500"
    height="380">
  </amp-img>
  <amp-img src="https://i.imgur.com/ULDCGZN.png"
    alt="photo description"
    width="500"
    height="380">
  </amp-img>
</amp-carousel>
```

## AMP form

![form-gmail](https://user-images.githubusercontent.com/15963/61767946-ae28f780-ad9a-11e9-9c6a-f36509d96e76.gif)

```html
<script async custom-element="amp-form" src="https://cdn.ampproject.org/v0/amp-form-0.1.js"></script>
```

## Credits

* Using [simple HTML email template](https://github.com/leemunroe/responsive-html-email-template) as a boilerplate
* Thanks to [paaatterns](https://github.com/leemunroe/responsive-html-email-template) for the nice images
