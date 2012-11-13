"Solitaire mit Backbone" - CologneJS, 13.11.2012 - Paul Wittmann
================================================================

* [paul@railslove.com](mailto:paul@railslove.com)
* [http://www.railslove.com/team/paul_wittmann](http://railslove.com/paul_wittmann)
* [@wakkahari](http://twitter.com/wakkahari)

Slides
------
[http://paulwittmann.github.com/colognejs-talk-2012-11/](http://paulwittmann.github.com/colognejs-talk-2012-11)<br>
source: [https://github.com/paulwittmann/colognejs-talk-2012-11](https://github.com/paulwittmann/colognejs-talk-2012-11)


Links aus Präsentation
----------------------
* Irmingard: [http://irmingard.herokuapp.com](http://irmingard.herokuapp.com)<br>
  code: [https://github.com/paulwittmann/irmingard-backbone](https://github.com/paulwittmann/irmingard-backbone)

* Simple Backbone Dummy App with Model-View syncing: [http://backbone-dummy.herokuapp.com](http://backbone-dummy.herokuapp.com)<br>
  code: [https://github.com/paulwittmann/backbone-dummy](https://github.com/paulwittmann/backbone-dummy)

* [HTML5 Drag and Drop tutorial](http://www.html5rocks.com/en/tutorials/dnd/basics)
* [DOMNodeInserted Hack](http://davidwalsh.name/detect-node-insertion)
* [RevealJS](http://lab.hakim.se/reveal-js)

* BDD Javascript Testing: [Jasmine](http://pivotal.github.com/jasmine)


Pro & Contra für Backbone
-------------------------

### The Gist of it all
1. Javascript MVC
  - provides structure for your Javascript code - less jQuery spaghetti code
  - cf. "Is it MVC, or what?" below
2. View Synching
  - update your views whenever your models' attributes change
3. Data Synching (not at all implemented in Irmingard)
  - offers painless synching of Backbone models to and from your server via Ajax and JSON

### Pros
+ active community &amp; widely used
+ mature (initial commit: Sep 30, 2010)
+ good documentation &amp; many great tutorials
+ lightweight (6kB, v0.9.2)
+ templating engine agnostic (HAMLc, underscore templates, handlebars, eco, jade etc.)
+ highly customizable (unlike many other JS MVC solutions)

### Cons
- rather barebone, lacking esp. View functionality and conventions for larger JS apps (that's why there are so many libraries built on top of it, Backbone core is intentionally being kept minimal)
- comparatively verbose to set up View behaviour
- lacks automatic Model-View bindings


Backbone Erweiterungen
----------------------
* [Backbone Marionette](https://github.com/derickbailey/backbone.marionette)
  Composite application architecture. Better view handling and unbinding. Alternative to 9elements' Chaplin but more mature.
  + [Backbone Geppetto](https://github.com/ModelN/backbone.geppetto)
    Setzt auf Marionette auf und fügt "scalable Controller architecture" hinzu.<br>

* [Backbone Relational](github.com/PaulUithol/Backbone-relational)
  Hierarchies of Backbone Models - 'has many'-relations etc.

* [Backbone Model Binder](github.com/theironcook/Backbone.ModelBinder)
  Provides Model-View bindings. Interesting to autosync from a view to a model via input fields etc. (plain Backbone only makes the other way around really easy).

* [HAML Coffee Assets](github.com/netzpirat/haml_coffee_assets)
  Backbone templates with HAML syntax. After '-' and '=' you'll be writing CoffeeScript instead of Ruby.


Resources
---------
* [www.backbonejs.org](http://www.backbonejs.org)

* [Annotated source](http://backbonejs.org/docs/backbone.html)

* Osmani, Addy. _Developing Backbone.js Applications_ (work in progress). [https://github.com/addyosmani/backbone-fundamentals](https://github.com/addyosmani/backbone-fundamentals).
  Probably the best single resource on Backbone so far.

* 3-part Peepcode screencast series: [https://peepcode.com/products/backbone-js](https://peepcode.com/products/backbone-js)
  Rather slow-going. You'll learn a lot more by playing around with your own project.

* Overview of Javascript MVC frameworks
  Osmani, Addy. 2012-07-27. "Journey Through The JavaScript MVC Jungle". [http://coding.smashingmagazine.com/2012/07/27/journey-through-the-javascript-mvc-jungle](http://coding.smashingmagazine.com/2012/07/27/journey-through-the-javascript-mvc-jungle)

* Overview of Backbone Architecture Libraries
  Schäfer, Mathias. 2012-05-10. "Application frameworks on top of Backbone.js. A birds-eye view of the similarities of Chaplin, Marionette and Thorax/Lumbar". [https://speakerdeck.com/u/molily/p/application-frameworks-on-top-of-backbonejs-talk-at-appsberlinjs](https://speakerdeck.com/u/molily/p/application-frameworks-on-top-of-backbonejs-talk-at-appsberlinjs)
  Mathias is one of the main programmers of moviepilot.com, one of the largest Backbone apps out there. He's also the maintainer of [Chaplin](https://github.com/chaplinjs/chaplin), a not yet production-ready alternative to Marionette.


Is it MVC, or what?
-------------------
In some regards, Backbone comes a lot closer to the original MVC architecture than, e.g., Rails.
MVC was designed by Trygve Reenskaug in 1979 while working on Smalltalk-80:
  - called it "Model-View-Controller-Editor"
  - View-Controller pair required for each element on the screen; no true separation
  - Controller’s role: handling user input
  - observer pattern: Views and Controllers subscribe to Models
  - the View is automatically updated whenever the Model changes
(for all of this cf. Addy Osmani's _Developing Backbone.js Applications_ above)

Nevertheless, Backbone's usually considered MV\* - it doesn't really follow the MVC pattern but has some important MVP features as well. Cf. [Backbone.js Is Not An MVC Framework](http://lostechies.com/derickbailey/2011/12/23/backbone-js-is-not-an-mvc-framework).


Kudos
-----
+ an [Tim Schneider](http://railslove.com/team/tim_schneider) für das fantastische Reveal.js Railslove template
