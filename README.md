# Submission for Take Home Task
## Languages Used
1. HTML
2. CSS
3. Javascript

## Contents
1. live website [link](https://knchn08.github.io/travelopia-take-home-task)
2. index.html - the main file containing website
3. assets folder - containing images used

## Approach
1. The aim was to get the basic elements asked in the test case in the given time.
2. A prototype was created that satisfied the requirements at the lowest level of execution.
3. I laid each element in order as asked and then proceeded to style them in order to produce the base UI.
4. The website currently holds many issues which can be improved on if worked for longer time and with more guidance provided.

## Testing
The page was tested on the various dimensions provided under edge inspect and the following observations were made:
1. There were two possible ways in which I have inserted the image. One is by using the &lt;img&gt; tag and other by using &lt;picture&gt;.
2. Pros of &lt;img&gt; observed here include that the image seems to cover the entire whitespace in the various devices it checked for.
3. Cons of &lt;img&gt; observed are the skewing of image due to it remaining in its original dimensions when tried over various device dimensions.
4. Pros of &lt;picture&gt; observed are that it shows better resolution of the source image for the dimensions handled
5. Cons of &lt;picture&gt; observed are that it leaves whitespaces for device dimensions(iPad Mini, iPad Air, Surface Pro 7 - as tested through Edge inspect) that are not covered.

## How to test both options
1. To test the image using &lt;picture&gt; option view the live website.
2. To test the image using  &lt;img&gt;, firt clone the repository to your system.
3. Then carry out the following changes in the index.html file: i. Uncomment the following segment of code in the file.
  ```
        <!-- <img src="assets\testimg.jpeg" alt="img">-->
  ```
  3. 2.  Comment the following segment of code in the file.
  ```
        <picture>
            <source srcset="assets\testimg_xl.jpeg" media="all and (min-width: 1200px)" type="image/jpeg" width="1600" height="1200" class="">
            <source srcset="assets\testimg_lg.jpeg" media="all and (min-width: 992px)" type="image/jpeg" width="1200" height="1440" class="">
            <source srcset="assets\testimg_md.jpeg" media="all and (min-width: 768px)" type="image/jpeg" width="992" height="992" class="">
            <source srcset="assets\testimg_sm.jpeg" media="all and (min-width: 576px)" type="image/jpeg" width="768" height="600" class="">
            <source srcset="assets\testimg_xs.jpeg" media="all and (min-width: 0)" type="image/jpeg" width="576" height="1500" class=""> 
            <img src="assets\testimg_sm.jpeg" alt="Homepage Img">
        </picture>  
  ```
   3. 3.  Save the file and view the refreshed html page.
