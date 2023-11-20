# Sass Basics

Welcome to the Sass Basics repository! This repository is designed to help you understand the fundamentals of Sass (Syntactically Awesome Style Sheets). With Sass, you can write more maintainable and powerful CSS using its features like variables, nesting, mixins, and more.

## Table of Contents

- [Introduction to Sass](#introduction-to-sass)
- [Installation](#installation)
- [Basic Usage](#basic-usage)
- [Variables](#variables)
- [Nesting](#nesting)
- [Mixins](#mixins)
- [Import](#import)
- [Resources](#resources)
- [Contributing](#contributing)
- [License](#license)

## Introduction to Sass

Sass is a CSS preprocessor that enhances the capabilities of standard CSS. It introduces features that make writing and maintaining stylesheets more efficient and organized.

## Installation

To start using Sass, you need to install it on your system. Follow these steps:

1. Install [Node.js](https://nodejs.org/) (if not already installed).

2. Open your terminal or command prompt.

3. Install Sass globally using Node Package Manager (npm):

`npm install -g sass`

## Basic Usage

Sass files have the `.scss` extension and can be compiled into standard CSS files. Here's how you can compile a Sass file:

1. Navigate to the directory containing your Sass file.

2. Open your terminal or command prompt.

3. Run the following command to compile the Sass file into CSS:

sass input.scss output.css

## Variables

Sass allows you to use variables to store values that you can reuse throughout your stylesheets. This makes it easier to maintain consistency.

Example:

```
$primary-color: #007bff;
$link-color: $primary-color;

a {
color: $link-color;
}

   ```

## Nesting

Sass enables you to nest selectors inside one another, improving readability and reducing repetition.
Example :

```
nav {
  ul {
    margin: 0;
    padding: 0;

    li {
      list-style: none;
    }
  }
}

   ```

## Mixins

Mixins in Sass are reusable sets of CSS declarations. They can take arguments, allowing you to create dynamic styles.

Example:

```
@mixin border-radius($radius) {
  border-radius: $radius;
}

.button {
  @include border-radius(5px);
}
  ```

## Import

Sass allows you to split your styles into multiple files and import them where needed.

Example:

```
// _variables.scss
$primary-color: #007bff;

// main.scss
@import 'variables';

body {
  background-color: $primary-color;
} 
  ```

## Resources

Sass Official Documentation [https://sass-lang.com/documentation]
Sass Guidelines [https://sass-guidelin.es/]

## Contributing

Contributions are welcome! If you find any issues or want to add enhancements to this repository, feel free to open a pull request.

## License
This project is licensed under the MIT License.