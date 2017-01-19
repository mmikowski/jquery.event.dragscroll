# jquery.event.dragscroll

## Summary
Use this plugin to add scrolling to touch enabled web pages.
It is compatible with jQuery 1.7.0+ and passes JSLint.

Code style is as presented in 
**Single Page Web Applications - JavaScript end-to-end**
which is available from [Amazon][1] and directly from [Manning][2].
The standard was last updated in [December 2016][3].

## Browser Support
Works with iOS5+ (Stock browser) and Android 3.2+ (Chrome) and of course
all modern desktop browsers (IE9+ and later version of
Chrome, Safari, and Firefox.

IE9 may require edge settings in the **head** section:

```html
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
```

## Examples

### Basic use
```js
  $(function (){
    var scroll_obj = $.makeDragScrollObj({ _$scroll_box_ : $( 'body' ) });
 
    $( 'body' )
      .on( 'udragend',   scroll_obj._onendHandler_   )
      .on( 'udragmove',  scroll_obj._onmoveHandler_  )
      .on( 'udragstart', scroll_obj._onstartHandler_ )
      ;
  });
```

### Option `_prop_key_`
Set this property to determine how the drag event propagates.

```js
`_stop_now_`: Prevent default behavior and stop drag event from
  propagating immediately.
      event_obj.preventDefault();
      event_obj.stopImmediatePropagation();

'_stop_all_': Prevent default behavior and stop drag event from
  propagating.
      event_obj.preventDefault();
      event_obj.stopPropagation();

'_stop_default_': Prevent default behavior.

default : Does not affect event behavior.

```

### Option `_do_scroll_x_`
Support x scrolling. Default `false`.

### Option `_do_scroll_y_`
Support y scrolling. Default `true`.

### Option `_drag_ratio_`
Affects scroll "friction."  Default is 0.001.

### Option `_on_stop_fn_`
Function executed when scrolling stops.  The function receives the
`_$scroll_box_` as the argument.

## Release Notes
### Copyright (c)
2015-2017 Michael S. Mikowski (mike[dot]mikowski[at]gmail[dotcom])

### License
Dual licensed under the MIT or GPL Version 2
http://jquery.org/license

### Version 0.9.0
First public npm release. 

### Version 0.9.1
Added the `_on_stop_fn_` callback which is fired after
scroll animation stops.

### Version 0.9.3
Updated docs.

### Version 1.0.0
Added support for the `body` element, update docs, README, and demo.

## Contribute!
If you want to help out, like all jQuery plugins this is hosted at
GitHub.  Any improvements or suggestions are welcome!
You can reach me at mike[dot]mikowski[at]gmail[dotcom].

If you are considering replacing jQuery with a "framwork", please consider
[if you really want an SPA framework][0]. 

## End
[0]:http://mmikowski.github.io/no-frameworks
[1]:http://www.amazon.com/dp/1617290750
[2]:http://manning.com/mikowski
[3]:https://github.com/mmikowski/spa/blob/master/js-code-std-2016.pdf
