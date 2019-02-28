---
title: Flexbox Responsive Layout - W3Schools How To Video 02
category: "W3Schools"
cover: flexbox.jpg
author: Zack
---

![Flex Responsive Layout](flexbox.jpg)

Today we are going to continue with our [W3Schools series](https://zacklive.com/w3schools-web-layout/) and learn how to create responsive layout with **Flexbox**. Using Flexbox for responsive design the a norm now at the beginning of 2019. If you are not familiar with Flexbox, check out the tutorial by W3Schools:

* [W3Schools Flexbox Tutorial](https://www.w3schools.com/css/css3_flexbox.asp)

The Flexbox Example of today:

* [Flexbox Responsive Layout Exxample](https://www.w3schools.com/howto/tryit.asp?filename=tryhow_make_a_website)

## Video link

## Flexbox Responsive Design

You can follow the following 3 steps to create a responsive layout with Flexbox:

1. Set the *display* of the container to *flex* and make it "*wrap*";
2. Set the *flex-basis* of each flex item in the flex container to a percentage;
3. Change the container's flex direction to *column* (*row* by default) in the **Media Query**.

In the W3Schools example, the Flex container is set as below:

```
.row {
  display: flex;
  flex-wrap: wrap;
}
```

The two columns in the container, a.k.a. the Flex items:

```
/* Sidebar/left column */
.side {
  flex: 30%;
  background-color: #f1f1f1;
  padding: 20px;
}

/* Main column */
.main {
  flex: 70%;
  background-color: white;
  padding: 20px;
}
```

Finally, the media query, the breakpoint is set to 700px:

```
@media screen and (max-width: 700px) {
  .row {
    flex-direction: column;
  }
}
```

## Improvement: Mobile first

Again, as an exercise, we can make this example mobile first.

The Flex container:

```
.row {
  display: flex;
  flex-direction: column
}
```

The Flex items:

```
.side {
  padding: 20px;
  background-color: #f1f1f1;
}

/* Main column */
.main {
  padding: 20px;
  background-color: white;
}
```

And the media query:

```
@media screen and (min-width: 700px) {
  .row {
    flex-direction: row;
  }
  .side {
    flex: 30%;
  }
  .main {
    flex: 70%;
  }
}
```

The code for the W3Schools series is on GitHub now: [W3Schools GitHub](https://github.com/ZacharyChim/W3Schools)

## W3Schools How-Tos Videos

W3Schools is a well-known web design/front-end development tutorial website, which not only provides detailed tutorials on HTML, CSS, JavaScript, etc., but also can be used as a reference, as it explains almost everything in the web design field. You probably have already visited this website as a frontend developer, because it often appears on the first page of many search results that are related to web design. And its How To section is really useful. It provides tutorials on, for example, how to make a SlideShow (picture carousel), a Lightbox, a Parallax effect and so on. So I want to do a series of videos dedicated to these How-Tos.

1. [Float Responsive Layout](https://atzack.com/w3schools-web-layout/)
2. [Flexbox Responsive Layout](https://atzack.com/w3schools-flex-layout/)