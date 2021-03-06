---
layout: page
title: "JavaScript hexdec function"
comments: true
sharing: true
footer: true
alias:
- /functions/view/hexdec:423
- /functions/view/hexdec
- /functions/view/423
- /functions/hexdec:423
- /functions/423
---
<!-- Generated by Rakefile:build -->
A JavaScript equivalent of PHP's hexdec

{% codeblock math/hexdec.js lang:js https://raw.github.com/kvz/phpjs/master/functions/math/hexdec.js raw on github %}
function hexdec(hex_string) {
  //  discuss at: http://phpjs.org/functions/hexdec/
  // original by: Philippe Baumann
  //   example 1: hexdec('that');
  //   returns 1: 10
  //   example 2: hexdec('a0');
  //   returns 2: 160

  hex_string = (hex_string + '')
    .replace(/[^a-f0-9]/gi, '');
  return parseInt(hex_string, 16);
}
{% endcodeblock %}

 - [Raw function on GitHub](https://github.com/kvz/phpjs/blob/master/functions/math/hexdec.js)

Please note that php.js uses JavaScript objects as substitutes for PHP arrays, they are 
the closest match to this hashtable-like data structure. 

Please also note that php.js offers community built functions and goes by the 
[McDonald's Theory](https://medium.com/what-i-learned-building/9216e1c9da7d). We'll put online 
functions that are far from perfect, in the hopes to spark better contributions. 
Do you have one? Then please just: 

 - [Edit on GitHub](https://github.com/kvz/phpjs/edit/master/functions/math/hexdec.js)


### Other PHP functions in the math extension
{% render_partial _includes/custom/math.html %}
