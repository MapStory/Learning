# StoryScapes101: Introduction to the StoryScapes platform
## Module 5 -  Composing StoryScapes 2.0

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

Each lesson is planned to take about thirty minutes to complete. Combined, this module should take two hours to complete (assuming ten minute breaks between each Lesson).

## Lesson 1: Using Choropleth and Graduated styling for StoryLayers
##### Objective
In this Lesson, students will learn to add Choropleth and Graduate styling to StoryLayers.
### Lecture
The StoryScape composer offers four different styling options: Simple, Unique, Choropleth and Graduated. In a previous Lesson we learned how to use Simple and Unique styling.

Choropleth and Graduated styling are special because they cannot be used with just any StoryLayer. Choropleth and Graduated styling require that a StoryLayer have at least one attribute that is _numerical_, such as the number of students in a school, or the number of people injured in a conflict. Additionally, the numerical attribute should also be _ordinal_, meaning that bigger numbers should indicate more than lesser numbers. Numbers that serve simply to identify a feature are not ordinal. Choropleth and Graduated styling uses these numerical figures to generate different styling based on the levels the feature has on the numerical attribute.

You can determine if a StoryLayer has numerical attributes by looking at the StoryLayer detail page on the Attributes tab.

##### Using Choropleth styling
Choropleth styling assigns a hue of a _color_ to a feature based on the magnitude of a particular numerical attribute. A color ramp or gradient specifies a range of available he options. For example, a choropleth color gradient based on _red_ might assign lighter hues of red to features with lower magnitudes on the attriubte and darker hues of red for features with higher magnitudes on the attribute.

For example, below we show a chapter from a StoryScape that depicts the numbers of civilians killed in the Syrian Civil War by governorate (a subnational unit in Syria). As the number of civilians killed in a governorate increases, the shade of red used to color the governorate becomes a darker red, or even a purple.

![SCREENSHOT](images/Screen Shot 2019-01-27 at 1.50.10 PM.jpg)\

To use Choropleth styling when composing a StoryScape, first make sure there is a StoryLayer that has a numerical attribute for you to use in StoryScapes. If you're not sure if a StoryLayer has a numerical attribute to use with Choropleth styling, you can go to the StoryLayers page and look at the table of its attributes.

You can see below that the page for the StoryLayer about Syrian governorates used in the example above shows that the StoryLayers has several attributes with numerical data.

![SCREENSHOT](images/Screen Shot 2019-01-27 at 1.58.09 PM.jpg)\

The exact procedure for using Choropleth styling will differ depending on the StoryLayer you are using and the data it contains, but the essential steps will be the same.

First, you will launch new StoryScape, as you learned to do in Module 2. To review, you should:
  - Click `Create` and `Compose StoryScape` at the top of your screen.
  - Give your new StoryScape a Title, a Summary and a Category.
  - Begin working on Chapter 1. Give Chapter 1 a name and enter a brief description.

Now you are ready to add a StoryLayer.
- Click `Add a StoryLayer` and begin typing to trigger the auto-complete box for StoryLayer names. When the StoryLayer you're looking for appears, select it and click `Add`.

In this example, we have added the StoryLayer depicting casualities by Syrian governorates, as has been referenced previously in the lesson:

![SCREENSHOT](images/Screen Shot 2019-01-27 at 2.16.30 PM.jpg)\

In the left-hand sidebar of the composer, we see the name of the StoryLayer and green buttons where we can `Style` the StoryLayer, toggle its `Visibility` and `Delete` it from the StoryScape.

Click `Style` to open up the style editor. This should look familiar from your work with `Simple` and `Unique` styling from Module 2. This time, we want to select the `Choropleth` styling option. This will customize the set of tools in the style editor that are appropriate for a choropleth style:

![SCREENSHOT](images/Screen Shot 2019-01-27 at 2.21.20 PM.jpg)\

Now we can make selections in the rest of the style editor to customize the choropleth style for the StoryLayer. In this example we do the following:

_Under the `Classification` header_:

- Select the attribute `t_status`. This is the attribute with the number of civilians killed in the governorate
- Select the number 5. This will divide the data into five color bins.
- Select a color ramp. Here we select the red-blue color ramp. Lower numbers will be a lighter red. as numbers increase, theyt will appear as a darker red, purple and blue at the highest level.
- Select the `Natural Breaks` method. This will divide the data into five equally sized groups (since I selected five earlier).
  - Note, StoryScapes offers five different `Methods` for organizing data into choropleth ramps. Here's what each of them means:
    - __Natural Breaks__:
    - __Equal Interval__:
    - __Quantile__:
    - __Geometric Interval__:
    - __Standard Deviation__:

_Under the `Stroke` header_:
- Select the way you want the line surrounding your features (the `Stroke`) to be depicted. StoryScapes supports strokes that are `Solid`, `Dashed`, or `Dotted`. Here dotted is selected.
- Select the thickness (or `Weight`) for the stroke. Here a stroke weight of 1 is selected.
- Select the `Color` for stroke. Here Black is selected.
- Select the `Transparency` for the stroke. A 100 percent transparency will show the color in its fullest form. Lower numbered transparencies will show a lighter stroke that is easier to see through. Here the transparency is 100.

_Under the `Label` header:
- Select an attribute with text if you want that text to appear on the map as a label. In this example, I could select the attribute that has the governorates name so that that name appears on each governorate. In this example no attribute is selected for a label. If we had selected one, we could also customize the `Size`, `Font`, `Color` and `Style` of the font used by the label.

_Under the `Rules` header_:

Once all of the `Classification` options are specified, StoryScapes will automatically generate a colors for the number of group bins you specified. In this example we had five group bins using Natural Breaks, so five group bins are generated.

StoryScapes allows you to alter and customize any of the pre-selected colors, but keep in mind that if you make changes, you should retain the core aspect of choropleth mapping - bigger numbers should correspond with darker colors.

At this point, our choropleth style for the StoryLayer looks like this:

![SCREENSHOT](images/Screen Shot 2019-01-27 at 2.47.17 PM.jpg)\

As the StoryLayer plays, governorates with higher casualties appear in darker red, purple and even blue colors as the casualties increase.

##### Using Graduated styling

Like the Choropleth style, Graduated style are based on the numerical attributes of the StoryLayer features. While Choropleth styles the features using a range of colors from a gradient, Graduated style uses the size of the feature to express the magnitude of a particular attribute. In general, features with lower values are represented by smaller features while features with higher values are represented by bigger features.

Because polygon features have fixed geographic areas, Graduated styling is not available for StoryLayers that have polygons. Graaduated styling is appropriate __only for points__ based Storylayers.

To use Graduated styling when composing a StoryScape, first make sure you've added a StoryLayer with points. Second, make sure you've added a StoryLayer that has a numerical attribute.

Let's look at an example.

Below we see the page of a StoryLayer that depicts terrorist attacks claimed by ISIS from around the world in recent years. This StoryLayer happens to have an attribute for `Casualties` that lists the number of casualties suffered from each ISIS attack. We can see that ISIS attacks in this StoryLayer have an average of 30 casualties and a median of five.

![SCREENSHOT](images/Screen Shot 2019-01-27 at 3.49.44 PM.jpg)\

In the StoryScapes composer, we can add this StoryLayer to a StoryScape, and select the `Graduated` styling option in order to help us show visually which ISIS attacks resulted in greater numbers of casualties.

To do this, we follow a very similar workflow to the one we just went through for Choropleth styling.

First, we complete the items in the style editor under _Classification_.
- Find the attribute you want to use graduated styling on.
- Select the number of bin groups you want to divide the data into. In this example we've used five.
- Select the `Method` you want to use to divide the data. Here were again using Natural Breaks.

Second, customize the way you want the point `Symbol` to look.
- Select a `Marker` type. In this example we used a circle.
- Select a `Color` for the symbol. In this example we use Black.
- Select a `Transparency` level. In this example were using 70 to provide a bit of transparency.
- `Rotate` your symbol. Since were using a Circle in this example, rotation isn't necessary. Rotation can be useful if you want your symbol to indicate direction somehow, perhaps if you're using an Arrow symbol, for example.

Third, customize the way you want the `Stroke` that borders your symbol to look.
- Select a solid, dotted or dashed stroke. In this example we use solid.
- Select a weight for the thickness of the stroke. In this example we use 1.
- Select a color for the stroke. In this example we use orange.
- Select a transparency for the stroke. In this example we use 70.

Fourth, customize the `Label` for your symbol, if you would like a label. For example, we may want the _name_ of the ISIS terrorist attack to appear on the map next to the feature symbol. If that's desired, we can select the attribute that has the attack name, and then customize the size, font, color and style of the text the name appears in. For this example, a label is not used.

Finally, under the `Rules` section, StoryScapes will automatically generate a feature size for each of the group bins you selected. In this example, we have five group bins that have been naturally broken up. Bin 1 includes ISIS attacks with 0-19 casualties. Bin 2 includes ISIS attacks with 19-59 casualties. And so forth. As a user, I can manually change the preset feature sizes. In this example, we've increased the feature sizes and left a 5-point interval between each. So, Bin 1 with the least casualties has a feature size of 7, while Bin 5 with the most casualties (range of 347-498) has a feature size of 27.

Here is our ISIS attacks StoryLayer with graduated style at a global view:
![SCREENSHOT](images/Screen Shot 2019-01-27 at 3.22.48 PM.jpg)\

And here we've zoomed in a bit more over Europe, the Middle East and North Africa to more clearly depict the different graduated sizes of each ISIS attack feature. We can clearly see that some more major attacks occured in Paris, Nigeria, and Turkey and that many smaller attacks have occurred along the North African coast.

![SCREENSHOT](images/Screen Shot 2019-01-27 at 3.23.35 PM.jpg)\

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
In this lesson, students will learn how to import icons and apply icons to styles for point StoryLayers.
### Lecture

Icons can be applied to StoryLayers made up of points when using the Simple style in the StoryScapes composer. Icons help to communicate the type of data represented by the points. For example, you might use a red cross icon on a StoryLayer that shows the distribution of hospitals.

StoryScapes has a built in 'Icons Commons' where users can upload icons that any other users, in turn, can apply to styles for point StoryLayers in a StoryScape.

##### Uploading new icons

If you have access to openly licenses icons, you can simply upload them to StoryScapes so that anyone can access them.

To upload new icons to StoryScapes, click `Upload Icons` in the `Create` drop-down at the top of your screen. This opens up a simple modal that looks like this:

![SCREENSHOT](images/Screen Shot 2019-01-27 at 5.40.12 PM.jpg)\

Icons must be in a .svg format to be uploaded into Storyscapes. You can either import a single Icon as an .svg, or upload a set of icons as a .zip file. Add a Tag for the icon(s) to help others understand what the icon depicts.

Once uploaded, your icons you will appear on your user profile so that other users of StoryScapes can see which icons you contributed. Here's a user profile with the icons imported:

![SCREENSHOT](images/Screen Shot 2019-01-27 at 5.41.00 PM.jpg)\

##### Adding icons to styles for point StoryLayers in the StoryScapes composer

When you are working on composing a StoryScape, you can add any of the icons imported by all users to a Simple style on a points-based StoryLayer. Here's how it works.

First, you'll launch new StoryScape, as you learned to do in Module 2. To review, you should:
  - Click `Create` and `Compose StoryScape` at the top of your screen.
  - Give your new StoryScape a Title, a Summary and a Category.
  - Begin working on Chapter 1. Give Chapter 1 a name and enter a brief description.

Second, add a StoryLayer made up of points to your StoryScape.
- Click `Add a StoryLayer` and begin typing to trigger the auto-complete box for StoryLayer names. When the StoryLayer you're looking for appears, select it and click `Add`.

In this example, we have added the StoryLayer depicting Russian-backed airstrikes into Syria during the Syrian Civil War.

![SCREENSHOT](images/Screen Shot 2019-01-27 at 5.50.00 PM.jpg)\

In the left-hand sidebar of the composer, we see the name of the StoryLayer and green buttons where we can `Style` the StoryLayer, toggle its `Visibility` and `Delete` it from the StoryScape.

Click `Style` to open up the style editor.

By default, when the StoryLayer is added to the StoryScape, it is styled with a standard orange circle.

This time, we want to select the `Simple` styling option again. This will customize the set of tools in the style editor that are appropriate for Simple styles.

To apply a custom icon to the point StoryLayer, you will click the `Marker` drop-down. In this drop-down box you will see a handful of common icons, such as a circle, square and star. You'll also see the button to open the `Icon Commons`:

![SCREENSHOT](images/Screen Shot 2019-01-27 at 5.50.13 PM.jpg)\

The Icons Commons modal lets you search all of the icons that users have uploaded. You can scroll through them, or search by Tags:

![SCREENSHOT](images/Screen Shot 2019-01-27 at 5.49.44 PM.jpg)\

In this example, we select an icon of the Russian flag and click `Ok`. Now, the points in the StoryLayer appear with a Russian flag instead of the default orange circle:

![SCREENSHOT](images/Screen Shot 2019-01-27 at 5.50.56 PM.jpg)\

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

![SCREENSHOT]()\

##### Adding many StoryPins with Media all at once

To add lots of StoryPins with media at once, you will download a blank .CSV file with pre-set column headers for the information you need to have for each StoryPin. This includes the embed link you need to add for your media. Once you’ve populated the CSV with your StoryPin information, return to the composer and upload your StoryPins. Once the StoryPins are added to your StoryScape, you will likely need to click into each StoryPin individually and confirm the settings are as you want them to be.

![SCREENSHOT]()\

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
