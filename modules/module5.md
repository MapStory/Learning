# StoryScapes101: Introduction to the StoryScapes platform
## Module 5 -  Composing StoryScapes 2.0

Document Version: 01/01/2019

---

This work is licensed under the Creative Commons Attribution 3.0 Unported License.  To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/ or send a letter to Creative Commons, 444 Castro Street, Suite 900, Mountain View, California, 94041, USA.

Also, credit to GeoAcademy for inspiring this open course format.

---

## Introduction

In this module, students will learn to compose StoryScapes that utilize advanced styling functions and StoryPins with media embeds. This Module builds upon Module 2 which introduced students to the StoryScapes composer.

This module includes the following lessons:

+	Lesson 1 – Using Choropleth and Graduated styling for StoryLayers
+	Lesson 2 – Using Icons Commons for point Storylayers
+	Lesson 3 – Adding StoryPins with Media

## Lesson 1: Using Choropleth and Graduated styling for StoryLayers

##### Objective

In this Lesson, students will learn to add Choropleth and Graduated styling to StoryLayers.

### Lecture

The StoryScape composer offers four different styling options: Simple, Unique, Choropleth and Graduated. In Module 2 you learned how to use Simple and Unique styling.

Choropleth and Graduated styling are special because they cannot be used with just any StoryLayer. Choropleth and Graduated styling require that a StoryLayer have at least one attribute that is _numerical_, such as the number of students in a school, or the number of people injured in a conflict. Additionally, the numerical attribute should also be _ordinal_, meaning that bigger numbers should indicate more than lesser numbers. Numbers that serve simply to identify a feature are not ordinal. Choropleth and Graduated styling uses these ordinal numerical figures to generate different styling based on the levels the feature has on the numerical attribute.

You can determine if a StoryLayer has numerical attributes by looking at the StoryLayer detail page on the Attributes tab.

##### Using Choropleth styling
Choropleth styling assigns color _hue_ to a feature based on its level on a particular numerical attribute. A color ramp or gradient specifies the color hue different features in the StoryLayer receive. For example, a choropleth color gradient based on _red_ might assign lighter hues of red to features with lower magnitudes on the attribute and darker hues of red for features with higher magnitudes on the attribute.

Below we show a chapter from a StoryScape that depicts the numbers of civilians killed in the Syrian Civil War by governorate (a subnational unit in Syria). As the number of civilians killed in a governorate increases, the shade of red used to color the governorate becomes a darker red, or even a purple.

![](images/Screen Shot 2019-01-27 at 1.50.10 PM.jpg)\

##### Using Graduated styling

Like the Choropleth style, Graduated styles are based on the numerical attributes of the StoryLayer features. While Choropleth styles the features using a range of colors from a gradient, Graduated style uses the size of the feature to express the magnitude of a particular attribute. In general, features with lower values are represented by smaller features while features with higher values are represented by bigger features.

Because polygon features have fixed geographic areas, Graduated styling is not available for StoryLayers that have polygons. Graduated styling is appropriate __only for points__ based Storylayers.

### Activity

The exact procedure for using Choropleth and Graduated styling will differ depending on the StoryLayer you are using and the data it contains, but the essential steps will be the same as those presented in this activity.

1. To use Choropleth styling when composing a StoryScape, first make sure you've added a StoryLayer to your StoryScape that has an ordinal numerical attribute. If you're not sure if a StoryLayer has a numerical attribute to use with Choropleth styling, you can exit composer and go to the StoryLayer's page and look at the table of its attributes.

 In this activity we will use a StoryLayer about Syrian governorates. If this StoryLayer is not already available in your StoryScapes platform, you can import it yourself by accessing the data from the Data folder: `data/Syrian_VDC_Governorates.zip`. You can see that this StoryLayer has several numerical attributes.

![](images/Screen Shot 2019-01-27 at 1.58.09 PM.jpg)\

2. Once you've confirmed your StoryLayer has numerical attributes, you will launch a new StoryScape in the composer, as you learned to do in Module 2. To review, you should:
  - Click `Create` and `Compose StoryScape` at the top of your screen.

  - Give your new StoryScape a Title, a Summary and a Category.

  - Begin working on Chapter 1. Give Chapter 1 a name and enter a brief description.

3. Now you are ready to add a StoryLayer. Click `Add a StoryLayer` and begin typing to trigger the auto-complete box for StoryLayer names. This example uses a StoryLayer named "Syrian VDC Governorates". When the StoryLayer you're looking for appears, select it and click `Add`.

![](images/Screen Shot 2019-01-27 at 2.16.30 PM.jpg)\

 In the left-hand sidebar of the composer, we see the name of the StoryLayer and green buttons where we can `Style` the StoryLayer, toggle its `Visibility` and `Delete` it from the StoryScape.

4. Click `Style` to open up the style editor. This should look familiar from your work with `Simple` and `Unique` styling from Module 2. This time, we want to select the `Choropleth` styling option. This will customize the set of tools in the style editor that are appropriate for a choropleth style:

![](images/Screen Shot 2019-01-27 at 2.21.20 PM.jpg)\

5. Under the `Classification` header, select the attribute `t_status`. This is the attribute with the number of civilians killed in the governorate

6. Under the `Classification` header, select the number 5. This will divide the data into five color bins.

7. Under the `Classification` header, select a color ramp. Here we select the red-blue color ramp. Lower numbers will be a lighter red. As numbers increase, they will appear as a darker red, purple and blue at the highest level.

8. Select the `Natural Breaks` method. This will divide the data into five equally sized groups (since I selected five bins earlier).
  - Note, StoryScapes offers five different `Methods` for organizing data into choropleth ramps:
    - _Natural Breaks_:
    - _Equal Interval_:
    - _Quantile_:
    - _Geometric Interval_:
    - _Standard Deviation_:


9. Under the `Stroke` header, select the way you want the line surrounding your features (the `Stroke`) to be depicted. StoryScapes supports strokes that are `Solid`, `Dashed`, or `Dotted`. Here dotted is selected.

10. Select the thickness (or `Weight`) for the stroke. Here a stroke weight of 1 is selected.

11. Select the `Color` for stroke. Here Black is selected.

12. Select the `Transparency` for the stroke. A 100 percent transparency will show the color in its fullest form. Lower numbered transparencies will show a lighter stroke that is easier to see through. Here the transparency is 100.

13. Under the `Label` header, select an attribute with text if you want that text to appear on the map as a label. In this example, we could select the attribute that has the governorates name so that that name appears on each governorate. In this example no attribute is selected for a label. If we had selected one, we could also customize the `Size`, `Font`, `Color` and `Style` of the font used by the label.

 Once all of the `Classification` options are specified, StoryScapes will automatically generate a colors for the number of group bins you specified. In this example we had five group bins using Natural Breaks, so five group bins are generated. StoryScapes allows you to alter and customize any of the pre-selected colors, but keep in mind that if you make changes, you should retain the core aspect of choropleth mapping - bigger numbers should correspond with darker colors.

At this point, our choropleth style for the StoryLayer looks like this:

![](images/Screen Shot 2019-01-27 at 2.47.17 PM.jpg)\

As the StoryLayer plays, governorates with higher casualties appear in darker red, purple and even blue colors as the casualties increase.

15. To use Graduated styling when composing a StoryScape, first make sure you've added a StoryLayer with points. Second, make sure you've added a StoryLayer that has a numerical attribute.

This example uses a StoryLayer that depicts terrorist attacks claimed by ISIS from around the world in recent years. If this StoryLayer is not already in your StoryScapes platform and you want to complete the exercise with this data, you can access it from the Data Folder: `data/external_attacks_through_march2016_6b89155d.zip`

This StoryLayer happens to have an attribute for `Casualties` that lists the number of casualties suffered from each ISIS attack. We can see that ISIS attacks in this StoryLayer have an average of 30 casualties and a median of five.

![](images/Screen Shot 2019-01-27 at 3.49.44 PM.jpg)\

16. In the StoryScapes composer, add this StoryLayer to a StoryScape.

17. Select the `Graduated` styling option in order to show visually which ISIS attacks resulted in greater numbers of casualties.

18. Under the Classification header, find the attribute you want to use graduated styling on. Here we use the "Casualties" attribute.

19. Select the number of bin groups you want to divide the data into. In this example we've used five.

20. Select the `Method` you want to use to divide the data. Here were again using Natural Breaks.

21. Under the `Symbol` header, select a `Marker` type. In this example we used a circle.

22. Select a `Color` for the symbol. In this example we use Black.

23. Select a `Transparency` level. In this example were using 70 to provide a bit of transparency.

24. Under the `Stroke` header, select a solid, dotted or dashed stroke. In this example we use solid.

25. Select a weight for the thickness of the stroke. In this example we use 1.

26. Select a color for the stroke. In this example we use orange.

27. Select a transparency for the stroke. In this example we use 70.

28. Finally, under the `Rules` section, StoryScapes will automatically generate a feature size for each of the group bins you selected. In this example, we have five group bins that have been naturally broken up. Bin 1 includes ISIS attacks with 0-19 casualties. Bin 2 includes ISIS attacks with 19-59 casualties. And so forth. As a user, I can manually change the preset feature sizes. In this example, we the feature sizes and left a 5-point interval between each. So, Bin 1 with the least casualties has a feature size of 7, while Bin 5 with the most casualties (range of 347-498) has a feature size of 27.

Here is our ISIS attacks StoryLayer with graduated style at a global view:

![](images/Screen Shot 2019-01-27 at 3.22.48 PM.jpg)\

And here we've zoomed in a bit more over Europe, the Middle East and North Africa to more clearly depict the different graduated sizes of each ISIS attack feature. We can clearly see that some more major attacks occured in Paris, Nigeria, and Turkey and that many smaller attacks have occurred along the North African coast.

![](images/Screen Shot 2019-01-27 at 3.23.35 PM.jpg)\

## Lesson 2: Using Icons Commons for point Storylayers
##### Objective

In this lesson, students will learn how to import icons and apply icons to styles for point StoryLayers.

### Lecture

Icons can be applied to points when using the Simple style in the StoryScapes composer. Icons help to communicate the type of data represented by the points. For example, you might use a red cross icon on a StoryLayer that shows the distribution of hospitals.

StoryScapes has a built in 'Icons Commons' where users can upload icons that any other users, in turn, can apply to styles for point StoryLayers in a StoryScape.

If you have access to openly licensed icons, you can simply upload them to StoryScapes so that anyone can access them. Icons must be in a .svg format to be uploaded into Storyscapes.

### Activity

Now lets try uploading and using icons in StoryScapes!

1. To upload new icons to StoryScapes, click `Upload Icons` in the `Create` drop-down at the top of your screen. This opens up a simple modal;

![](images/Screen Shot 2019-01-27 at 5.40.12 PM.jpg)\

 You can either import a single icon as an .svg, or upload a set of icons as a .zip file. If you don't have an .svg icon of your own to upload, in the Data Folder we provide an example of a Flag of Russia: `data/Flag_of_Russia.svg`

 2. Add a Tag for the icon(s) to help others understand what the icon depicts.

3. Once you have uploaded the .svg, your icon you will appear on your user profile so that other users of StoryScapes can see which icons you contributed. Here's a user profile with the icons imported:

![](images/Screen Shot 2019-01-27 at 5.41.00 PM.jpg)\

 Try going to your own profile to see that your icon is available there under the Icons tab.

4. Now lets try using an icon in a StoryScape. When you are composing a StoryScape, you can add any of the icons imported by all users to a Simple style on a points-based StoryLayer. First, launch a new StoryScape, as you learned to do in Module 2. To review, you should:

  - Click `Create` and `Compose StoryScape` at the top of your screen.
  - Give your new StoryScape a Title, a Summary and a Category.
  - Begin working on Chapter 1. Give Chapter 1 a name and enter a brief description.

5. Add a StoryLayer made up of points to your StoryScape. In this example we use a StoryLayer depicting Russian airstrikes into Syria. If this StoryLayer isn't already available in your StoryScapes platform, you can upload it yourself. It is available in the Data Folder: `data/Russian_Airstrikes_Syria.zip`. Once added, the StoryLayer should look like this:

![](images/Screen Shot 2019-01-27 at 5.50.00 PM.jpg)\

6. In the left-hand sidebar of the composer, we see the name of the StoryLayer and green buttons where we can `Style` the StoryLayer, toggle its `Visibility` and `Delete` it from the StoryScape. Click `Style` to open up the style editor.

7. By default, when the StoryLayer is added to the StoryScape, it is styled with a standard circle. This time, we want to select the `Simple` styling option again. This will customize the set of tools in the style editor that are appropriate for Simple styles.

8. To apply a custom icon to the point StoryLayer, you will click the `Marker` drop-down. In this drop-down box you will see a handful of common icons, such as a circle, square and star. You'll also see the button to open the `Icon Commons`.

![](images/Screen Shot 2019-01-27 at 5.50.13 PM.jpg)\

9. The Icons Commons modal lets you search all of the icons that users have uploaded. You can scroll through them, or search by Tags:

![](images/Screen Shot 2019-01-27 at 5.49.44 PM.jpg)\

10. In this example, we select an icon of the Russian flag and click `Ok`. Now, the points in the StoryLayer appear with a Russian flag instead of the default orange circle:

![](images/Screen Shot 2019-01-27 at 5.50.56 PM.jpg)\

## Lesson 3: Adding StoryPins with Media

##### Objective

In this lesson, students will learn how to add media, such as images and videos, to StoryPins in a StoryScape.

### Lecture

To review, StoryPins let you add more qualitative information that doesn't quite make sense as part of the StoryLayer data. For example, perhaps you want a StoryPin with a newspaper article, or you want to pin a video that helps explain what the viewer is seeing in your StoryScape. Or, maybe you just want to add some clarifying text that a viewer can click to understand more about something at a specific moment in time.

In Module 2 we learned how to add StoryPins with text to a StoryScape. Just like with StoryPins that only have text, StoryPins with media can be added to a StoryScape one at a time or in bulk.

### Activity

In this Activity we add a StoryPin with a video to a StoryScape about Russian airstrikes in Syria, using the Storylayer that was used in the previous lesson.

1. First, we'll repeat the same steps completed in the previous lesson to get that StoryScape setup. Launch a new StoryScape, as you learned to do in Module 2. To review, you should:

  - Click `Create` and `Compose StoryScape` at the top of your screen.
  - Give your new StoryScape a Title, a Summary and a Category.
  - Begin working on Chapter 1. Give Chapter 1 a name and enter a brief description.

2. Add a StoryLayer made up of points to your StoryScape. In this example we use a StoryLayer depicting Russian airstrikes into Syria. If this StoryLayer isn't already available in your StoryScapes platform, you can upload it yourself. It is available in the Data Folder: `data/Russian_Airstrikes_Syria.zip`. Once added, the StoryLayer should look like this:

![](images/Screen Shot 2019-01-27 at 5.50.00 PM.jpg)\

3. Now let's start creating the StoryPin. You should already know the basics of creating a StoryPin from your work in Module 2. To review quickly, you just give your StoryPin a title and description and add it to the map. Once it’s added to the map, define a start and end time, and determine if you want it to appear on the map and/or on the timeline. If you need more help in completing these steps, refer back to Module 2.

4. To add an image or video to your StoryPin, you will paste the _embed_ link for that media from an approved StoryScapes media service. Note, the video file is also available in the Data Folder: `data/Syrian and Russian airstrikes flattening Aleppo (1).mp4`

5. Once the media is added, you can customize it in the following ways:

- Customize the size of the StoryPin pop-up window.
- If you have a video, set the offset point where you want the video to begin playing. For example, you may want your video to begin 30 seconds after the actual start of the video.
- If you have a video, define the number of seconds you want it to play for. For example, you may have two minute video, but only want it to play for one minute in your StoryScape.

6. Once you have added all of this information, update the map. The StoryPin will now appear in the chapter during the timeframe you indicated.

In this example, we have added a StoryPin with a video that highlights how Russian-backed airstrikes have caused particular destruction in Aleppo. We have set the video to last 90 seconds and located it in Aleppo.

![](images/Screen Shot 2019-01-30 at 5.32.31 PM.jpg
)\

7. To add lots of StoryPins with media at once, you will download a blank .CSV file with pre-set column headers for the information you need to have for each StoryPin. This includes the embed link you need to add for your media. Once you’ve populated the CSV with your StoryPin information, return to the composer and upload your StoryPins. See Module 2 for more description of this, if you need review.

8. Once the StoryPins are added to your StoryScape, you will likely need to click into each StoryPin individually and confirm the settings are as you want them to be.

## Conclusion

In this Module you have learned to add further narrative depth to your StoryScapes. You can now highlight numerical and statistical attributes in your StoryLayers with Choropleth and Graduated styling. You can add logical symbols to your point StoryLayers with Icons. And you can embed images and videos into your StoryPins.

By combining these new skills with the StoryScapes composing skills you learned in earlier Modules, you are now ready to publish StoryScapes about topics you find important and compelling.

## Discussion Questions

Before moving on to the next Module, reflect independently or in a group on the following questions:

1. When might it be helpful to add qualitative information in the form of StoryPins to a StoryScape?

2. Similarly, how can different styling approaches make a StoryScape seem to tell different stories? Can you provide an example?

3. Now that you have a more complete understanding of how to compose a StoryScapes, what kinds of skills do you think are most important for a person to have to be a strong StoryTeller?

4. How might StoryScapes help you bring in lessons from history into your work? Why might this be important?

5. What other questions are you still left with at this stage about the process of composing a StoryScape?
