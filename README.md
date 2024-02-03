# Submission for Take Home Task
## Languages Used
1. HTML
2. CSS
3. Javascript

## Contents
1. live website [link](https://www.example.com)
2. test.html - the main file containing website
3. assets folder - containing images used

## Discussion
1. There were two possible ways in which I have inserted the image. One is by using the normal &lt;img&gt; tag and other by using &lt;picture&gt;.
2. Pros of &lt;img&gt; observed here include that the image seems to cover the entire whitespace in the various devices it checked for while Cons observed are the skewing of image due to it remaining in its original dimensions when tried over various devices
3. Pros of &lt;picture&gt; observed are that it shows better resolution of the source image for the conditions handled whereas Cons observed are that it leaves whitespaces for device dimensions that are not covered.

## Testing both options
1. To test the image using &lt;img&gt; option view the live website.
2. To test the image using  &lt;picture&gt; option do as follows: 2. 1. Uncomment the following segment of code in the file.
  ```
        <!-- <picture>
            <source srcset="assets\testimg_xl.jpeg" media="all and (min-width: 1200px)" type="image/jpeg" width="1600" height="1200" class="">
            <source srcset="assets\testimg_lg.jpeg" media="all and (min-width: 992px)" type="image/jpeg" width="1200" height="1440" class="">
            <source srcset="assets\testimg_md.jpeg" media="all and (min-width: 768px)" type="image/jpeg" width="992" height="992" class="">
            <source srcset="assets\testimg_sm.jpeg" media="all and (min-width: 576px)" type="image/jpeg" width="768" height="600" class="">
            <source srcset="assets\testimg_xs.jpeg" media="all and (min-width: 0)" type="image/jpeg" width="576" height="1500" class=""> 
            <img src="assets\testimg_sm.jpeg" alt="Homepage Img">
        </picture>  -->
  ```
  2. 2.  Comment the following segment of code in the file.
  ```
        <img src="assets\testimg.jpeg" alt="img">
  ```
   2. 3.  Save the file and view the refreshed html page.
