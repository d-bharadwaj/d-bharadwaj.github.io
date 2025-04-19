---
title: Superscalar RISC-V Processor
template: page
summary: Out-of-Order Design with Advanced Caching and Branch Prediction
cv_pdf: pdf/Dhanvi_Bharadwaj_Resume.pdf
img: images/image.png
importance: 1
category: courses
related_publications:
---
<!-- 
    Every project has a beautiful feature showcase page
    It's easy to include images in a flexible 3-column grid format.
    Make your photos 1/3, 2/3, or full width

    To give your project a background in the portfolio page, just add the img tag to the front matter like so:

        ---
        layout: page
        title: project
        description: a project with a background image
        img: /assets/img/12.jpg
        ---

    !TEMPLATE!
    <div class="row">
        <div class="col-sm mt-3 mt-md-0">
            {{ figure(path="images/1.jpg",title="example image", class="img-fluid rounded z-depth-1") }}
        </div>
        <div class="col-sm mt-3 mt-md-0">
            {{ figure(path="images/3.jpg",title="example image", class="img-fluid rounded z-depth-1") }}
        </div>
        <div class="col-sm mt-3 mt-md-0">
            {{ figure(path="images/5.jpg",title="example image", class="img-fluid rounded z-depth-1") }}

        </div>
    </div>
    <div class="caption">
        Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
    </div>
    <div class="row">
        <div class="col-sm mt-3 mt-md-0">
            {{ figure(path="images/5.jpg",title="example image", class="img-fluid rounded z-depth-1") }}
        </div>
    </div>
    <div class="caption">
        This image can also have a caption. It's like magic.
    </div>
    !TEMPLATE!

    You can also put regular text between your rows of images.
    Say you wanted to write a little bit about your project before you posted the rest of the images.
    You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.

    !TEMPLATE!
    <div class="row justify-content-sm-center">
        <div class="col-sm-8 mt-3 mt-md-0">
            {{ figure(path="images/6.jpg",title="example image", class="img-fluid rounded z-depth-1") }}
        </div>
        <div class="col-sm-4 mt-3 mt-md-0">
            {{ figure(path="images/11.jpg",title="example image", class="img-fluid rounded z-depth-1") }}
        </div>
    </div>
    <div class="caption">
        You can also have artistically styled 2/3 + 1/3 images, like these.
    </div>
    !TEMPLATE!

    The code is simple.
    Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
    To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
    Here's the code for the last row of images above:

    ```html
    !TEMPLATE!
    <div class="row justify-content-sm-center">
        <div class="col-sm-8 mt-3 mt-md-0">
            {{ figure(path="images/6.jpg",title="example image", class="img-fluid rounded z-depth-1") }}
        </div>
        <div class="col-sm-4 mt-3 mt-md-0">
            {{ figure(path="images/11.jpg",title="example image", class="img-fluid rounded z-depth-1") }}
        </div>
    </div>
    !TEMPLATE!
    ``` -->

Our team designed, implemented, and analyzed an N-way superscalar, out-of-order RISC-V processor. Our design includes a G-Share branch predictor, return address stack, instruction prefetching, variably-associative non-blocking caches, and a victim cache. Following the MIPS R10K architecture, we used a reorder buffer, and reservation station to achieve high instruction-level parallelism.

<div style="border: 1px solid #ccc; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
  <iframe 
    src="/pdf/EECS_470_Final_Report.pdf#toolbar=0&navpanes=0&view=FitH  " 
    style="width: 100%; height: 1000px; border: none;" 
    title="EECS 470 Final Report"
  >
    Your browser does not support iframes. 
    <a href="/pdf/EECS_470_Final_Report.pdf" target="_blank">Download the PDF</a> instead.
  </iframe>
</div>
