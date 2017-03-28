# Learning-Technology-Ecosystem
## [Atomic Design](http://atomicdesign.bradfrost.com/)
* **Atoms** of our interfaces serve as the foundational building blocks that comprise all our user interfaces.
* **Molecules** are relatively simple groups of UI elements functioning together as a unit. 
* **Organisms** are relatively complex UI components composed of groups of molecules and/or atoms and/or other organisms. 
* **Templates** are page-level objects that place components into a layout and articulate the design’s underlying content structure.
* **Pages** are specific instances of templates that show what a UI looks like with real representative content in place.
* **Microservices** are pages and services that represent a single business capability or domain
* **Monoliths** are applications that combine a multitude of microservices and/or business capabilities
* **Ecosystems** are compilations of microservices and monoliths 

###Examples
A form label atom, search input atom, and button atom can join together to create a search form molecule.

A logo atom, search form molecule, and navigation molecule can be joined together to create a header organism.

A header organism, billboard organism, sidebar organism, and footer organism can be joined together to create a homepage template.

Data can be provided to a homepage template to create a home page.

Multiple pages and APIs can be joined together to offer a service or microservice.

Multitudes of services joined together in one application architecture create a monolith.

Microservices and monolithes offered as a portfolio of services to the university community is the learning technology ecosystem.


## Design for the edges
The majority of faculty will use the LMS monolith, and usually, only a few features. 

Design intuitive solutions for innovative and laggard faculty and students.

Design is just the application of a structure. Theme is on top of that.