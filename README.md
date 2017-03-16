## Website Performance Optimization

Website optimization using [Google PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) score to evaluate page speed. The second part of the project is the optimization of Frames per Second(fps) in pizza.html. 

####Part 1: Optimize PageSpeed Insights score for index.html of the portfolio

PageSpeed Insights Score Before Optimization: Mobile: 27/100 Desktop: 29/100

1. Compress images. Images have a huge impact on page speed.
2. Use a font loader. "After images, fonts are the normally the largest assets in your web page."(See #1 under resources).
3. Concatenate, minify and inline css.
4. Move google analytics code from the head to right before the closing body tag.

PageSpeed Insights Score After Optimization: Mobile: 97/100 Desktop: 97/100

####Part 2: Optimize Frames per Second in pizza.html

To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or higher. You will find instructive comments in main.js. 

You might find the FPS Counter/HUD Display useful in Chrome developer tools described here: [Chrome Dev Tools tips-and-tricks](https://developer.chrome.com/devtools/docs/tips-and-tricks).

#### Resources

1. [How to Improve Page Performance with a Font Loader](https://www.sitepoint.com/improve-page-performance-font-loader/)
2. [Loading Web Fonts with the Web Font Loader](https://css-tricks.com/loading-web-fonts-with-the-web-font-loader/)


