# com480-week-4-intro-to-d3js-solved
**TO GET THIS SOLUTION VISIT:** [COM480 Week 4-Intro to D3JS Solved](https://www.ankitcodinghub.com/product/com480-week-4-intro-to-d3js-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96768&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COM480 Week 4-Intro to D3JS Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<h1 id="intro-to-d3js">Intro to D3JS</h1>
In this lab, we are going to build basic charts with D3. We will start with a scatter plot and then create a bar chart. Weather data is a suitable dataset for this exercise. Fetch some weather forecast for this week and get started.

<h2 id="preparing-the-data">Preparing the data</h2>
D3 needs data in the form of an array of objects, such as&nbsp;<code>[{'x': 1, 'y': 2}, {'x': 2, 'y': 5}</code>.

We provide the example data in the variables&nbsp;<code>TEST_TEMPERATURES</code>&nbsp;and&nbsp;<code>DAYS</code>. Please convert this data into an array where each element is&nbsp;<code>{'y': temperature, 'x': number_of_day, 'name': day_name}</code>.

<h2 id="initialize-d3js">Initialize D3JS</h2>
To use D3 funcitons, first, you need to add the latest version of D3 library to your project. It is included in the exercise files, so one way to do this is to add it as a script to your HTML file.

<pre><code>&lt;script src="lib/d3.min.js"&gt;&lt;/script&gt;</code></pre>
Alternatively you can use the CDN:&nbsp;<code>&lt;script src="https://d3js.org/d3.v5.min.js"&gt;&lt;/script&gt;</code>

<h2 id="scatter-plot">Scatter plot</h2>
First task is to create a simple full-screen scatter plot. Before you get started, we strongly encourage you to read this&nbsp;<a href="https://bost.ocks.org/mike/join/">blog post</a>&nbsp;by&nbsp;<a href="https://bost.ocks.org/mike/">Mike Bostock</a>, creator of D3. It explains a very basic, yet very important, concept of the library. You will be using it in all D3 projects. Also, it will tell you exactly how to build your first scatter plot.

Please use the tutorial to add the circles for the data you have converted.

<h2 id="scales">Scales</h2>
If you used the&nbsp;<code>x</code>&nbsp;and&nbsp;<code>y</code>&nbsp;of the datapoints directly as SVG coordinates, you may notice that the points don’t cover the whole plot. We should rescale them.

The SVG diagram has an internal coordinate space – it is in this space that we place our elements by specifying their&nbsp;<code>x</code>&nbsp;and&nbsp;<code>y</code>. The origin and size of that space is determined by the&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/viewBox">viewBox</a>&nbsp;property. For convenience, we used&nbsp;<code>viewBox="-10 -10 220 120"</code>&nbsp;which means that the internal coordinate space of the SVG starts at&nbsp;<code>[-10, -10]</code>&nbsp;and its size is&nbsp;<code>[220, 120]</code>.

Therefore the space is from&nbsp;<code>[-10, -10]</code>&nbsp;to&nbsp;<code>[210, 110]</code>. We will use the space from&nbsp;<code>[0, 0]</code>&nbsp;to&nbsp;<code>[200, 100]</code>&nbsp;for our plot, while the remaining space are the margins. In the bottom and left margins&nbsp;<code>(x=-10 to 0, y=100 to 110)</code>&nbsp;we will also place the labels.

Please use&nbsp;<a href="https://github.com/d3/d3-scale/blob/master/README.md">D3 scales</a>&nbsp;to map between the range of our values to the space of the plot. The functions&nbsp;<a href="https://github.com/d3/d3-array#max"><code>d3.min</code>&nbsp;and&nbsp;<code>d3.max</code></a>&nbsp;can be helpful as well.

Please remember that the SVG Y is 0 at top of the diagram, but scatter plots usually have 0 at the bottom.

<img data-recalc-dims="1" decoding="async" data-src="https://i0.wp.com/mdn.mozillademos.org/files/224/Canvas_default_grid.png?w=320&amp;ssl=1" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==" class="lazyload">

<h2 id="colors">Colors</h2>
Like in the previous exercise, please change the color of the points according to the temperature (17 and below is blue, 23 and above is red, default is white).

<h2 id="labels">Labels</h2>
You have learned how to place elements with D3. If you feel confident, try creating text labels for the plot, as seen in the reference solution:

<img decoding="async" data-src="task_images/scatter_plot_final.png" width="640" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==" class="lazyload">

<h2 id="bar-chart-optional">Bar chart (optional)</h2>
Now, create a bar chart. The scatter plot that we have just created only takes a part of the screen. When you resize the browser window, the bar chart should adjust accordingly. Adjust the coordinates with scales to fill the viewport. Once you have done this, feel free to experiment with scales in console.
