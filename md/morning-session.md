## Logistics
1. Student Introductions
2. Self Introductions
3. Courseware
4. Internet Access
5. Phones on silent

-


## How you will Benefit
* Learn to build Hybrid apps for mobile devices
* Gain hands-on experience
	- Generous mixture of presentation and labs
* Access to expereinced intructors.
  
-

## Requirements - You!
* Experience
* Practical knowledge of Html, and Javascript

* Equipment
	* Your own laptop
	* Node and Ionic and course-material installed
	* IDE of your choice, we suggest Visual Studio Code
	* PDF Reader

-

## Course Agenda: Morning

### Ionic Basics
* Generating your first project
* Anatomy of an Ionic Project
* Ionic CLI Commands
* Decorators
* Classes

-

## Course Agenda: Afternoon
* Templates
* Styling & Theming
* Navigation
* User Input
* Saving Data
* Fetching Data, Observables and Promises

-

## Covered in this section

* Agenda
* Installation
* New Concepts
	* EMCAScript 6
	* TypeScript
	* Web Components
	
-
-

####Sample Ionic HTML Template

```
<ion-menu [content]="content">
			(click)="openPage(p)"></button>
</ion-menu>
```
-
-
####Sample Ionic TypeScript Template

```
import { Component } from '@angular/core';
```


-
-

# ECMAScript 6 (ES6)

-

### ECMAScript 6 (ES6)

* ECMAScript is a standard,

-

### ECMAScript 6 (ES6)

* In a similar way, HTML specifications (most recently HTML5) are defined by the organising body and are implemented by the browser vendors. Different browsers implement specifications in different

-

# Classes

-
### Classes in Javascript

You can now use and implement Classes as a part of the language, instead of having an approximation of them. 

-

### Classes in Javascript

```
class Shape {
		this.y = y
		
```
-

# Modules

-

### Modules

Modules allow you to modularise your code into packages that can be imported anywhere you need in

-

### Modules

```
// lib/math.js
```
```
```
```
```

-

# Promises

-

### Promises

Promises are something that have been made available by services like ngCordova previously, but now

```
doSomething().then((response) => {

```

-

# Block Scoping

-

### Block Scoping (let Keyword )

Currently, if you define a variable in Javascript it is available anywhere within the function that it was defined

```
for (let i = 0; i < a.length; i++) {
```

-

# Fat Arrow Functions

-

### Fat Arrow Functions

New Way ( Good )

```
someFunction((response) => {

```
Old way (Meh)

```
someFunction(function(response){
```

-

### Fat Arrow Functions

Old way (Meh)

To access the parent method we have to do some work 
```
var me = this;

someFunction(function(response){
```

-

### Fat Arrow Functions

New Way ( Good )

```
someFunction((response) => {

```

-

# TypeScript

-

### Typescript

A typed superset of JavaScript that compiles to plain JavaScript

```
function add(x: number, y :number):number {
// this function can only accept numerical input

```

-

# Transpiling

-

### Transpiling

Transpiling means converting from one language to another language. Why is this important to us? Basically,

-

### Transpiling

We use a transpiler to convert our ES6 code into ES5 code (i.e. the

-
### Transpiling

* Here’s how the process works:
	* You don’t need to worry about this process as it is all automatically handled by Ionic.

-

# Web Components

-

### Old way

```
<div id="slider">
		</div>
```

-

### Using Components

```
<img-slider>

```

-
-

# Ionic Basics

* (Live Walkthrough)

-
-


# Decorators

-

### Decorators

Each class (which we will talk about in the next section) you see in an Ionic application will have a decorator.

```
@Component({
```

-

### Decorators

* They definitely look a little weird, but they play an important role. 
* Provide some metadata about the class you are defining, and 
* They always sit directly above your class

```
@Decorator({
```

-

### Decorators

The decorator name itself is quite useful, here’s a few you might see in an Ionic application:

-

### @Component

* A @Component is not specific to Ionic, it is used generally in Angular 2. 
* A lot of the functionality provided by Ionic is done through using components. 
* In Ionic, for example, you might want to create a search bar,

```
<ion-searchbar></ion-searchbar>

```

-

### @Component

Ionic provides a lot of components but you can also

```
@Component({
```

-

### @Component

Which would then allow you to use it in your templates like this:

```
	<my-cool-component></my-cool-component>
```

-

# @Directive

-

### @Directive

The @Directive decorator allows you to create your own custom directives. Typically, the decorator would

```
@Directive({
```

-

### @Directive

Then in your template you could use that selector to trigger the behaviour of the directive you have created

```
<some-element my-selector></some-element>
```

-

### @Directive

* It might be a little confusing as to when to use **@Component** and **@Directive** , as they are both quite similar.

-

# @Pipe

-

### @Pipe
@Pipe allows you to create your own custom pipes to filter data that is displayed to the user, which can

```
@Pipe({
```
-

### @Pipe

Which would then allow you to implement it in your templates like this:

```
<p>{{someString | myPipe}}</p>
```
Now someString would be run through your custom myPipe before the value is output to the user.

-

# @Injectable

-

### @Injectable

* An @Injectable allows you to create a service for a class to use. A common example of a service created

-

### @Injectable

* Rather than doing this manually in your

-

# @IonicPage

-
### @IonicPage

* The @IonicPage decorator works in tandem with the NavController to help provide navigation, and “lazy
* It is included by default at the top of any “page” that is generated in your application, but
* Adding the @IonicPage

-

### @IonicPage 
```
@IonicPage()
```