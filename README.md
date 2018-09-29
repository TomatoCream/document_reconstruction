
# Table of Contents

1.  [Scan2Doc](#org3ac8f6c)
2.  [The plan](#org99af250)
3.  [Guidelines](#orgea59b9c)
4.  [Links](#org699126d)
5.  [Tasks](#org3158ad2)


<a id="org3ac8f6c"></a>

# Scan2Doc

-   we shall use the readme to track issues and split tasks


<a id="org99af250"></a>

# The plan

Since we cannot develop this in parallel, as in makes no sense for 6
people to write a neural network model.

we shall split the task.


<a id="orgea59b9c"></a>

# Guidelines

Ideally we should make it semi functional, i.e. reduce side effects
and global variables. therefore we can easily modularise each part
and switch around as quickly as possible.


<a id="org699126d"></a>

# Links

-   Neural Network Resources
    -   <http://course.fast.ai/lessons/lesson1.html>


<a id="org3158ad2"></a>

# Tasks

-   Preprocessing
    -   DONE YS Import images, surprisingly challenging since it is on
        collab had to upload it to Github
    -   DONE YS Cut images to shape, make a functional cutter to cut
        into shape
    -   NOTE possible improvements is we could somehow get random
        squares from a picture
-   Neural network
    -   DONE DF Simple Auto encoder model
    -   TODO maybe write simple function to iterate differing parameters
        of the model?
    -   NOTE After trying the performance on a simple model. We could
        try to use more complex models such as U-net. Its just a
        combination of Autoencoder and Resnet.
    -   NOTE we could combine a GAN and classifier to classify and
        process at the same time. This classifier would provide hints to
        the network and performance should be better. Might be hard to
        train given limited data.
-   Data 
    -   NOTE Since we only ripped out 217 images of data and this data
        is 3 years old, data might not be enough, we have not accounted
        for many different forms of variations. For example.
        
        -   Different font
        -   Different texts
        -   Pen Marks
        -   Different spacing between characters
        -   Different spacing between lines
        -   Varying intensity and lightness of fonts, e.g. light grey
        -   Pictures in documents
        
        It would be nice to have a script that will generate synthetic
        data for us.
        
        -   Solutions
            -   using template pictures(coffee stains&#x2026;) and overlaying it
            -   Generate fake ink marks
            -   Generate creases on paper

