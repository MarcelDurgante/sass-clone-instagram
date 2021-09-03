`#sass` `#css` `#html` `#master-in-software-engineering`

# SASS - Clone Instagram <!-- omit in toc -->

<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0-blue.svg?cacheSeconds=2592000" />
</p>

> Sass (which stands for 'Syntactically awesome style sheets) is an extension of CSS that enables you to use things like variables, nested rules, inline imports and more
>
> The purpose of this project is to learn the basics of SASS and put them into practice by building a visual replica of Instagram

## Index <!-- omit in toc -->

- [Requirements](#requirements)
- [Repository](#repository)
- [Technologies used](#technologies-used)
- [Project delivery](#project-delivery)
- [Resources](#resources)

## Requirements

- You must use variables at least once in the project.
- You must use nesting.
- You must use inheritance at least once in the project.
- You cannot use third party libraries for the development of this pill

## Repository

First of all you must fork this project into your GitHub account.

To create a fork on GitHub is as easy as clicking the “fork” button on the repository page.

<img src="https://docs.github.com/assets/images/help/repository/fork_button.jpg" alt="Fork on GitHub" width='450'>

### Installing

In this project you must use the VSCode SASS extension in order to compile SASS into CSS.

First of all you will need to install the extension:

- [Live SASS Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)

When the extension is installed correctly, having a SASS file open, you must click on "Watch Sass":

<img src="https://raw.githubusercontent.com/ritwickdey/vscode-live-sass-compiler/master/images/Screenshot/AnimatedPreview.gif" width="600px">

If you want to change some configuration of "Live SASS Compiler" you can check this official resource:

- [Live SASS Compiler Settings](https://github.com/ritwickdey/vscode-live-sass-compiler/blob/master/docs/settings.md)

## Technologies used

\* SASS

\* CSS

\* HTML

## Project delivery

To deliver this project you must follow the steps indicated in the document:

- [Submitting a solution](https://www.notion.so/Submitting-a-solution-524dab1a71dd4b96903f26385e24cdb6)

## Resources

- [SASS documentation](https://sass-lang.com/)
- [W3S SASS](https://www.w3schools.com/sass/)
- [SASS Guidelines](https://sass-guidelin.es/es/)
- [Organizing SASS Projects](https://blog.prototypr.io/how-i-organize-sass-projects-e2d7760df86f)
- [Why don't use @import](https://www.youtube.com/watch?v=CR-a8upNjJ0)

## 1.1. Theory Questions Answered

#### What is SASS? What does SASS stand for?

"CSS with superpowers". As they say about themselves in their website:

> Sass is the most mature, stable, and powerful professional grade CSS extension language in the world (according to what themselves say in their website). 

Sass stands for ***syntactically awesome stylesheets*** and it is a scripting language that is compiled into regular CSS and was created to help writing CSS easier and more efficient.

Sass can create **variables** for _colors, font-sizes_, and any other value. You can then use that variable throughout your styles to make global changes without having to find and replace to make a change.

With Sass you can break up your stylesheet into subfiles like _\_nav.scss_, _\_typography.scss_ and then merge them together into one file named _styles.css_.

You can create and use **mixins** which are essentially a block of styles you can insert to your rules. One way I use mixins is for _fonts_. Often fonts have a font-family, color, font-weight, etc that when I declare a font I want all of those properties to be applied. This saves you time maintaining all of the properties throughout your stylesheet.

#### What is a CSS pre-processor?

CSS preprocessors are scripting languages that extend the default capabilities of CSS. They enable us to use logic in our CSS code, such as _variables, nesting, inheritance, mixins, functions,_ and _mathematical operations_. CSS preprocessors make it easy to automate repetitive tasks, reduce the number of errors and code bloat, create reusable code snippets, and ensure backward compatibility.

Each CSS preprocessor has its own syntax that they compile into regular CSS so that browsers can render it on the client side. Currently, the three most popular and stable CSS preprocessors are **Sass, LESS,** and **Stylus**, however there are many smaller ones as well. CSS preprocessors all do similar things but in a different way and with their own syntaxes. Each of them has some advanced features unique to them and their own ecosystem (tools, frameworks, libraries) as well.

#### What does a pre-processor have to do with SASS?

In short, Sass is a CSS preprocessor, which adds special features such as _variables, nested rules and mixins_ (sometimes referred to as syntactic sugar) into regular CSS. **The aim is to make the coding process simpler and more efficient.**

#### Why use SASS?

Sass (and other CSS preprocessors) can be a powerful ally — a tool that any style-crafter can easily insert into their daily work.

A browser can only understand CSS, as the styling technique for any DOM element being rendered. CSS, as a language has its own feature set, which at times might not be enough to create a clean and reusable chunk of rules. Eg. Not being able to reuse a collection of rules in multiple selectors, unavailability of variables which may lead to ambiguous pieces of data across the stylesheet.

To overcome most of these limitations, the concept of a preprocessor was born — offering an advanced way of writing CSS, which extends the basic functionalities. This advanced code is later compiled as normal CSS code using respective compilers (which depends on what preprocessor you are using), which the browser will understand.

As our web pages and apps get more complex our style sheets get larger and harder to maintain. CSS preprocessors like Sass help by keeping our style sheets concise and allowing us to modularize our code while offering a whole slew of features not yet available in regular CSS.

#### SASS has disadvantages? Which are?

- Sass disadvantages
- The developer must have enough time to learn new features present in this preprocessor before using it.
- Using Sass may cause losing benefits of browser’s built-in element inspector.
- Code has to be compiled
- Difficult  Troubleshooting
 
#### What is a SASS Variable? Explain why are useful

Sass variables are used to store information that can be reused throughout the stylesheet when you need. Thet are useful because you can store things like colors, font stacks, or any CSS value according to your future reusability.

#### Explain the SASS variables property with an example.

A variable allows you us store a value or a set of values (information/informations) inside given variables (like strings, numbers, etc). With Sass you can reuse these variables throughout our SASS files as many times we want and wherever we want. Easy, powerful, and useful.

#### What is a mixin? Why is it important? Give an example

Mixins allow you to define styles that can be re-used throughout your stylesheet. They make it easy to avoid using non-semantic classes like .float-left, and to distribute collections of styles in libraries.

Mixins are defined using the **@mixin** at-rule, which is written **@mixin \<name> { ... }** or **@mixin name(<arguments...>) \{ ... }**. A mixin’s name can be any Sass _identifier_, and it can contain any statement other than _top-level statements_. They can be used to encapsulate styles that can be dropped into a single style rule; they can contain style rules of their own that can be nested in other rules or included at the top level of the stylesheet; or they can just serve to _modify variables_.

Mixins are included into the current context using the **@include** at-rule, which is written @include <name> or @include <name>(<arguments...>), with the name of the mixin being included.
  
To summarize: The **\@mixin** lets you create CSS code that is to be reused throughout the website. The @include directive is created to let you use (include) the mixin.

#### What is SCSS? Give an example
#### What is SASS? Give an example
#### What is the difference between .scss and .sass syntax.
#### In which cases would we use SCSS? And in which cases would we use SASS?
#### Explain how traditional CSS and Preprocessed CSS workflows are different.
#### Can we create functions with SASS? If it is true, give an example.
#### What is nesting? Is it useful? Give an example of nesting
#### Difference between @use & @import? Give an example
#### How can we import other CSS/SASS files in SASS? Give an example
#### Explain the concept of inheritance in SASS.
#### Why use @extend? Give an example

