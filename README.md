# jquery.event.dragscroll #

## Summary ##

Use this jQuery plugin to create numerous inertia scrolling areas all 
with their own properties.  One does this by creating a drag-scroll-handler
object and then using the event handlers and methods from that object.

It is written in the style of presented in
[Single page web applications - JavaScript end-to-end][1]
and passes JSLint.  It is touch and desktop enabled.

Compatible with jQuery 1.7.0+.

## Browser Support ##

Works with iOS5+ (Stock browser) and Android 3.2+ (Chrome) and of course
all modern desktop browsers (IE9+ and later version of
Chrome, Safari, and Firefox.

IE9 may require edge settings:

    <html>
    <head>
      <meta http-equiv="X-UA-Compatible" content="IE=edge" />
      ....

## Examples ##

Coming soon!

## Avoid complex 'SPA framework' libraries ##

jQuery used with this and a few other well-chosen tools forms
a fantastic basis for a lean, easy to use SPA architecture
as detailed in [Single page web applications, JavaScript end-to-end][1].
Here are the recommended tools:

| Capability   | Tool                | Notes                             |
| ------------ | ------------------- | ----------------------------------|
| Websockets   | [Socket.io][6]      | Prefer websockets over AJAX.      |
| AJAX         | jQuery native       | Use jQuery AJAX methods.          |
| Promises     | jQuery native       | Use jQuery promise methods.       |
| Model Events | [Global Events][2]  | jQuery plugin eliminates having   |
|              |                     | to manage multiple event types.   |
| Touch        | [Unified events][3] | Unify desktop and touch events.   |
| Routing      | [uriAnchor][4]      | jQuery plugin for robust routing. |
|              |                     | Includes support for dependent    |
|              |                     | and independent query arguments.  |
| Data Model   | [taffyDB][5]        | A powerful and flexible SQL-like  |
|              |                     | client data management tool.      |
| SVG          | [D3][7]             | Great for easy graphs and charts  |
|              | [SVG][8]            | Low-level jQuery plugin           |
| Templates    | [Dust][9]           | Uses a powerful template DSL that |
|              |                     | minimizes chances to intemingle   |
|              |                     | business and display logic.       |

This suite of tools has all the capabilities of a bleeding-edge 
SPA "framework" library within the reliable and mature jQuery ecosystem.
It can provide an application that is significantly more flexible and
testable since display logic can easily be decoupled from business logic.
Finally, it leverages jQuery's maturity, performance, and excellent
tools instead of competing with them.

## Release Notes ##

### Copyright (c) ###
2015 Michael S. Mikowski (mike[dot]mikowski[at]gmail[dotcom])

### License ###
Dual licensed under the MIT or GPL Version 2
http://jquery.org/license

### Version 0.9.0 ###
First public npm release. 

### Testing ###

Works in Safari, Firefox, and Chrome.

## TODO ##
Coming soon!

## Contribute! ##

If you want to help out, like all jQuery plugins this is hosted at
GitHub.  Any improvements or suggestions are welcome!
You can reach me at mike[dot]mikowski[at]gmail[dotcom].

## END ##

[1]:http://manning.com/mikowski
[2]:https://github.com/mmikowski/jquery.event.gevent
[3]:https://github.com/mmikowski/jquery.event.ue
[4]:https://github.com/mmikowski/urianchor
[5]:https://github.com/typicaljoe/taffydb
[6]:http://socket.io
[7]:https://github.com/mbostock/d3
[8]:http://keith-wood.name/svg.html
[9]:http://linkedin.github.io/dustjs
