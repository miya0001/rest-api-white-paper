# Case Study: ustwo

*[ustwo](http://ustwo.com) wanted a decoupled website with a WordPress backend and a frontend built with React.*
Daniel Demmel, ustwo

![a diagram showing the ustwo architecture](images/ustwo-architecture.png)

The ustwo website is a single-page application: the frontend is built using React and WordPress manages the content. React was used because it allows for
isomorphic rendering (pages can be rendered on the server or by the client). There is a Node.js server that enables server-side rendering.

On the WordPress side, a [custom page builder plugin](https://github.com/mattheu/modular-page-builder) gets authors to enter content in a modular fashion. This ensures that the content is modular and portable to different contexts.
The infrastructure for the REST API is used along with a bespoke API comprising custom endpoints that deliver content in JSON format to the frontend.