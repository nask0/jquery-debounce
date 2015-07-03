# Debounce and throttle function's decorator plugin
## Simple debounce and throttle implementations

### Usage: 
```
debouncedFn = $.debounce(fn, timeout, [invokeAsap], [ctx]);
throttledFn = $.throttle(fn, timeout, [ctx]);
```

### Example of debouncing
```
$('input[name=suggest]').keyup($.debounce(onKeyUp, 300));
// or
$('input').bind('keyup blur', $.debounce(process, 300));
```

### Example of throttling
```
$(window).resize($.throttle(doComplexСomputation, 300));
```
