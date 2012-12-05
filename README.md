jCount
======

jquery plugin counter with number formatting

NOTICE:
------

The jCount plugin was originally created and generously shared by [Matt Huggins](https://github.com/mhuggins/jquery-countTo).  

Matt is awesome.

I have added a function to Matt's plugin that formats the numbers (adds commas).  Some people think that's awesome too.

For the whole story, read this blog post: [http://johnmclaughlin.info/introducing-jcount-a-jquery-countup-plugin-with-output-number-formatting/](http://johnmclaughlin.info/introducing-jcount-a-jquery-countup-plugin-with-output-number-formatting/)

Requirements:
-------------
[jCount](https://github.com/jmaclabs/jCount) requires the latest version of [jQuery](http://jquery.com).

Usage:
------
The most basic usage of this plugin is to create a DOM element, and apply the `countTo` method to it in your JS.

    <script type="text/javascript"><!--
        $('.timer').countTo({from: 0, to: 500});
    //--></script>
    
    <span class="timer"></span>

A more detailed example that demonstrates all possible options being used is as follows.

    <script type="text/javascript"><!--
        $('.timer').countTo({
            from: 50,
            to: 2500,
            speed: 1000,
            refreshInterval: 50,
            onComplete: function(value) {
                console.debug(this);
            }
        });
    //--></script>
    
    <span class="timer"></span>

Options:
--------
A complete listing of the options that can be passed to the `countTo` method is below.

<table>
  <tr>
    <th>Option</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><i>from</i></td>
    <td>The number to start counting from.</td>
  </tr>
  <tr>
    <td><i>to</i></td>
    <td>The number to stop counting at.</td>
  </tr>
  <tr>
    <td><i>speed</i></td>
    <td>The number of milliseconds it should take to finish counting.</td>
  </tr>
  <tr>
    <td><i>refreshInterval</i></td>
    <td>The number of milliseconds updating the count.</td>
  </tr>
  <tr>
    <td><i>onComplete</i></td>
    <td>A callback function the is triggered when counting finishes.  The final value is
        passed to the function, and it is run in the context of the DOM element</td>
  </tr>
</table>

Created By:
-----------
[Matt Huggins](http://www.matthuggins.com)

License:
--------
jCount and jQuery-countTo are released under the [MIT license](http://www.opensource.org/licenses/MIT).
