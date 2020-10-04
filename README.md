Skycons
=======

Skycons is a set of ten animated weather glyphs, procedurally generated by
JavaScript using the HTML5 canvas tag. They're easy to use, and pretty
lightweight, so they shouldn't rain on your parade:

    <canvas id="icon1" width="128" height="128"></canvas>
    <canvas id="icon2" width="128" height="128"></canvas>

    <script>
      var skycons = new Skycons({"color": "pink"});
      // on Android, a nasty hack is needed: {"resizeClear": true}

      // you can add a canvas by it's ID...
      skycons.add("icon1", Skycons.PARTLY_CLOUDY_DAY);

      // ...or by the canvas DOM element itself.
      skycons.add(document.getElementById("icon2"), Skycons.RAIN);

      // if you're using the Forecast API, you can also supply
      // strings: "partly-cloudy-day" or "rain".

      // start animation!
      skycons.play();

      // you can also halt animation with skycons.pause()

      // want to change the icon? no problem:
      skycons.set("icon1", Skycons.PARTLY_CLOUDY_NIGHT);

      // want to remove one altogether? no problem:
      skycons.remove("icon2");
    </script>

Skycons were designed for [Forecast](http://forecast.io/) by those wacky folks
at The Dark Sky Company, and were heavily inspired by Adam Whitcroft's
excellent [Climacons](http://adamwhitcroft.com/climacons/). The source code has
been [released into the public domain][cc0], so please do with it as you see
fit! ♡

[cc0]: http://creativecommons.org/publicdomain/zero/1.0/

Variants
--------

Dark Sky no longer actively maintains Skycons, but several kind folks have made
variants that you might be interested in:

*   [Color Skycons](https://github.com/maxdow/skycons) by Maxime Warnier.
*   [Skycons for Android](https://github.com/torryharris/Skycons) by Torry Harris..
<br>
<p align="center"><img src="https://user-images.githubusercontent.com/48045143/95022717-9df6f280-0696-11eb-816e-588bf4acb6f7.PNG"></p>
<br>



