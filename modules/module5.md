# StoryScapes101: Introduction to the StoryScapes platform
## Module 5 -  Composing StoryScapes 2.0
### Objective –

Document Version: 01/01/2019

---

This work is licensed under the Creative Commons Attribution 3.0 Unported License.  To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/ or send a letter to Creative Commons, 444 Castro Street, Suite 900, Mountain View, California, 94041, USA.

Also, credit to GeoAcademy for inspiring this open course format.

---

## Introduction

In this module, students will learn to compose StoryScapes that utilize advanced styling functions and StoryPins with media embeds. This Module builds upon the Composer 1.0 Module that introduced students to the StoryScapes composer.

This module includes the following lessons:

+	Lesson 1 – Using Choropleth and Graduated styling for StoryLayers
+	Lesson 2 – Using Icons Commons for point Storylayers
+	Lesson 3 – Adding StoryPins with Media

Each lesson is planned to take about XXXX minutes to complete. Combined, this module should take XXX hours to complete (assuming ten minute breaks between each Lesson).

## Lesson 1: Using Choropleth and Graduated styling for StoryLayers
##### Objective
In this Lesson, students will learn to add Choropleth and Graduate styling to StoryLayers.
### Lecture
The StoryScape composer offers four different styling options: Simple, Unique, Choropleth and Graduated. In a previous Lesson we larned how to use Simple and Unique styling.

Choropleth and Graduated styling are special because they cannot be used with just any StoryLayer. Choropleth and Graduated styling require that a StoryLayer have at least one attribute that is numerical, such as the number of students in a school, or the number of people injured in a conflict. Choropleth and Graduated styling use these numerical figures to generate different styling based on the levels the feature has on the numerical attribute.

You can determine if a StoryLayer has numerical attributes by looking at the StoryLayer detail page on the Attributes tab.

![SCREENSHOT](figures/Twopartsofthegeospatialdatamodel.png "Two parts of the geospatial data model")

##### Using Choropleth styling
Choropleth styling assigns a _color_ to a feature based on its he magnitude of a particular numerical attribute. A color ramp or gradient specifies a range of available options between two fixed colors. For example, a color gradient between yellow and blue could include colors like yellow-green, green, blue-green, among others. The advantage of using choropleth is that it gives a smooth transition from one value to another.

For example, we might have a StoryLayer that shows how many people were killed and injured in each region of Syria during the Civil War there. By using Choropleth styling with a red gradient, we make the regions with higher casualties are darker red color and the regions with less casualties could be a lighter shade of red.

To use Choropleth styling when composing a StoryScape, first make sure you've added a StoryLayer that has a numerical attribute.

Then, select the Choropleth styling option. Select the Attribute that you want to style on, and determine the number of gradient levels you want. Select a color gradient. Select a method for breaking up the numerical data. For example, if you want each level to have the _same number_ of cases, you could select Natural Breaks. XXXXXXX

![SCREENSHOT](figures/Twopartsofthegeospatialdatamodel.png "Two parts of the geospatial data model")

##### Using Graduated styling

Like the Choropleth style, Graduated style are based on the numerical attributes of the StoryLayer features. While Choropleth styles the features using a range of colors from a gradient, Graduated style uses the size of the feature to express the magnitude of a particular attribute. In general, features with lower values are represented by smaller features while features with higher values are represented by bigger features.

Because polygon features have fixed geographic areas, Graduated styling is not available for StoryLayers that have polygons. Graaduated styling __only for points__.

To use Graduated styling when composing a StoryScape, first make sure you've added a point StoryLayer. Second, make sure you've added a StoryLayer that has a numerical attribute.

Then, select the Graduated styling option. Select the Attribute that you want to style on. Select the number of graduated levels you want. Select a method for breaking up the numerical data. For example, if you want each level to have the _same number_ of cases, you could select Natural Breaks. XXXXXXX

You can then further customize the look of your point features by choosing the type of point marker you want to use, the color you want to use, and more.

### Demonstration

Now that you've learned how to add Graduated and Choropleth styling to a StoryLayer in the StoryScapes composer, let's watch an example of a user performing these actions:

Watch this video. VIDEO.

### Tasks

Now it's your turn! If possible, return to the StoryScape you worked on in the Composer 1.0 Module.

- [x] Find a point StoryLayer that has a numerical attribute to add to your StoryScape. Implement a Graduates style.
- [x] Find a polygon layer that has a numerical attribute to add to your StoryScape. Implement a Choropleth style.
- [x] Save your StoryScape and re-publish it. Send the link to a colleague to review.

## Lesson 2: Using Icons Commons for point Storylayers
##### Objective
In this lesson, students will learn how to apply custom icons to styles for point StoryLayers.
### Lecture

Icons can only be applied to StoryLayers made up of points. Icons help to communicate the type of data represented by the points. For example, you might use a red cross icon on a StoryLayer that shows the distribution of hospitals.

StoryScapes has a built in 'Icons Commons' where users can upload icons that any other users, in turn, can apply to styles for point StoryLayers in a StoryScape.

If you have access to openly licenses icons, you can simply upload them to StoryScapes so that anyone can access them. Then, when you are composing a StoryScape, you can access all the icons uploaded by the user community.

![SCREENSHOT](figures/Twopartsofthegeospatialdatamodel.png "Two parts of the geospatial data model")

##### Uploading new icons

Icons must be in a .svg file format. To upload new icons to StoryScapes, click Icons Commons from the header. This opens up a simple modal where you can upload a single Icon as an .svg, or upload a set of icons as a .zip. Any Icons you upload will appear on your user profile. As previously mentioned, when you or any user is in the StoryScapes composer, you can access all uploaded icons as part of your styles for point StoryLayers.

![SCREENSHOT](figures/Twopartsofthegeospatialdatamodel.png "Two parts of the geospatial data model")

##### Adding icons to styles for point StoryLayers in the StoryScapes composer

When you or any other StoryScapes user, are working on a StoryScape, you can see all of the icons in the Icons Commons, and use one to style a StoryLayer made up of points.

![SCREENSHOT](figures/Twopartsofthegeospatialdatamodel.png "Two parts of the geospatial data model")

### Demonstration

Now that you've learned how to add custom icons to point StoryLayers in the StoryScapes composer, let's watch an example of a user performing these actions:

Watch this video. VIDEO.

### Tasks
Now it's your turn! Complete the following:

- [x] Upload a new .svg file to the StoryScapes Icon Commons. If you don't have access to an SVG file to use, visit one of the following repositories: XXXXXX. Go to your StoryScapes profile to confirm the Icon is listed there.
- [x] Return to the StoryScape you've been working on throughout the course, if you have a point StoryLayer in your story. If not, launch a new StoryScape and add a point StoryLayer to the StoryScape
- [x] Use Simple styling on the point StoryLayer and add an icon - either the one you uploaded or another icon that is available.
- [x] Save and publish your story, and share the link with a colleague for review.

## Lesson 3: Adding StoryPins with Media
##### Objective
In this lesson, students will learn how to add media, such as images and videos, to StoryPins in a StoryScape.

### Lecture

In a previous Lesson we learned how to add StoryPins with text only to a StoryScape. As a reminder, StoryPins let you add more qualitative information that doesn't quite make sense as part of the StoryLayer data. For example, perhaps you want a pin with a newspaper article that was important, or you want to pin a video that helps explain what the viewer is seeing in your StoryScape. Or, maybe you just want to add some clarifying text that a viewer can click to understand more about something at a specific moment in time.

Just like with StoryPins that only have text, StoryPins with media can be added to a StoryScape one at a time or in bulk.

###### Adding StoryPins with Media one at a time

To add StoryPins with media one at a time, just give your pin a title and description and add it to the map. Once it’s added to the map, define a start and end time, and determine if you want it to appear on the map and/or on the timeline.

To add an image or video to your StoryPin, you will paste the _embed_ link for that media from an approved StoryScapes media service XXXX. Once the media is added, you can customize it in the following ways:
+ Customize the size of the StoryPin pop-up window.
+ If you have a video, set the offset point where you want the video to begin playing. For example, you may want your video to begin 30 seconds after the actual start of the video.
+ If you have a video, define the number of seconds you want it to play for. For example, you may have two minute video, but only want it to play for one minute in your StoryScape.

Once you have added all of this information, update the map. The StoryPin will now appear in the chapter during the timeframe you indicated.

![SCREENSHOT](figures/Twopartsofthegeospatialdatamodel.png "Two parts of the geospatial data model")

##### Adding many StoryPins with Media all at once

To add lots of StoryPins with media at once, you will download a blank .CSV file with pre-set column headers for the information you need to have for each StoryPin. This includes the embed link you need to add for your media. Once you’ve populated the CSV with your StoryPin information, return to the composer and upload your StoryPins. Once the StoryPins are added to your StoryScape, you will likely need to click into each StoryPin individually and confirm the settings are as you want them to be.

![SCREENSHOT](figures/Twopartsofthegeospatialdatamodel.png "Two parts of the geospatial data model")

### Demonstration

Now that you've learned how to add StoryPins with media to a StoryScape, let's watch an example of a user performing these actions:

Watch this video. VIDEO.

### Tasks

Now it's your turn! Return to the StoryScape you've been working on throughout the course. Add a new StoryPin that requires media (either an image or a video). Add the proper embed link and customize the StoryPin. Save and re-publish your StoryScape. Share the StoryScape link with a colleague to review to confirm the StoryPin media appears as it should.

## Conclusion

In this Module you have learned to add further narrative depth to your StoryScapes. You can now highlight numerical and statistical attributes in your StoryLayers with Choropleth and Graduated styling. You can add logical symbols to your point StoryLayers with Icons. And you can embed images and videos into your StoryPins.

By combining these new skills with the StoryScapes composing skills you learned in earlier Modules, you are now ready to publish StoryScapes about topics you find important and compelling.

## Discussion Questions

Before moving on to the next Module, take fifteen minutes to reflect independently or in a group on the following questions:
