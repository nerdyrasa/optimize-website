## Website Performance Optimization

Website optimization using [Google PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) score to evaluate page speed. The second part of the project is the optimization of Frames per Second(fps) in pizza.html. 

[Click here for the live index.html for PageSpeed Insights evaluation](https://nerdyrasa.github.io/optimize-website/)

[Click here for the live pizza.html for frames per second evaluation](https://nerdyrasa.github.io/optimize-website/views/pizza.html) Open the console window to review statistics.
___

#### Part 1: Optimize PageSpeed Insights score for index.html of the portfolio

PageSpeed Insights Score *Before* Optimization: 

**Mobile: 27/100**

**Desktop: 29/100**

1. Compress images. Images have a huge impact on page speed.
2. Use a font loader. "After images, fonts are the normally the largest assets in your web page."(See #1, Resources).
3. Concatenate, minify and inline css.
4. Move google analytics code from the head to right before the closing body tag.

PageSpeed Insights Score *After* Optimization: 

**Mobile: 97/100** :smiley:

**Desktop: 97/100** :smiley:
___

#### Part 2: Optimize Frames per Second in pizza.html

1. Change querySelector to getElementById (See #3, Resources)
2. Use class, not style. (See #4, Resources)
3. Put operations outside of loops when possible.
___

#### Resources

1. [How to Improve Page Performance with a Font Loader](https://www.sitepoint.com/improve-page-performance-font-loader/)
2. [Loading Web Fonts with the Web Font Loader](https://css-tricks.com/loading-web-fonts-with-the-web-font-loader/)
3. [Performance: getElementById vs. querySelector](https://jsperf.com/getelementbyid-vs-queryselector)
4. [Performance: Class vs. Style](https://jsperf.com/class-vs-style)
5. [Where did rendering go in Chrome DevTools](http://stackoverflow.com/questions/33292084/where-did-rendering-go-in-chrome-devtools)
6. [Markdown Cheat Sheet](https://beegit.com/markdown-cheat-sheet)
7. [Photo Resizer](http://webresizer.com/resizer/)
8. [Photo Compressor](https://compressor.io/compress)
9. [Timeline Profiling with Chrome DevTools](http://blog.librato.com/posts/chrome-devtools)
10. [Interesting perspective from a Chromium Developer](https://medium.com/@egraether/why-working-on-chrome-made-me-develop-a-tool-for-reading-source-code-7111ba21a6f0#.6mgo252tp)
11. [document.createDocumentFragment()](https://developer.mozilla.org/en-US/docs/Web/API/Document/createDocumentFragment)

#### Reviewer Suggestions

Scrolling speed may not be 60 fps on more modest devices.  For those devices, enabling hardware accelerated composition makes a huge difference. You could use translateX instead of style.left in the main.js file, or, a little trick to make it simpler. Add these properties to .mover in the css file. 
   ```
   -webkit-backface-visibility: hidden; /* Chrome, Safari, Opera */
   backface-visibility: hidden;
   ```
   
    