## Website Performance Optimization

Website optimization using [Google PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) score to evaluate page speed. The second part of the project is the optimization of Frames per Second(fps) in pizza.html. 

####Part 1: Optimize PageSpeed Insights score for index.html of the portfolio

PageSpeed Insights Score Before Optimization: Mobile: 27/100 Desktop: 29/100

1. Compress images. Images have a huge impact on page speed.
2. Use a font loader. "After images, fonts are the normally the largest assets in your web page."(See #1, Resources).
3. Concatenate, minify and inline css.
4. Move google analytics code from the head to right before the closing body tag.

PageSpeed Insights Score After Optimization: Mobile: 97/100 Desktop: 97/100

####Part 2: Optimize Frames per Second in pizza.html

1. Change querySelector to getElementById (See #3, Resources)
2. Use class, not style. (See #4, Resources)
3. Put operations outside of loops when possible.



#### Resources

1. [How to Improve Page Performance with a Font Loader](https://www.sitepoint.com/improve-page-performance-font-loader/)
2. [Loading Web Fonts with the Web Font Loader](https://css-tricks.com/loading-web-fonts-with-the-web-font-loader/)
3. [Performance: getElementById vs. querySelector](https://jsperf.com/getelementbyid-vs-queryselector)
4. [Performance: Class vs. Style](https://jsperf.com/class-vs-style)
5. Significant changes in course content and current DevTools prompting: "Hey, Where'd it go?" [Where did rendering go in Chrome DevTools](http://stackoverflow.com/questions/33292084/where-did-rendering-go-in-chrome-devtools)