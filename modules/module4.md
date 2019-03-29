# StoryScapes101: Introduction to the StoryScapes platform
## Module 4 -  Curating StoryLayer Data

Document Version: 01/01/2019

---

This work is licensed under the Creative Commons Attribution 3.0 Unported License.  To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/ or send a letter to Creative Commons, 444 Castro Street, Suite 900, Mountain View, California, 94041, USA.

Also, credit to GeoAcademy for inspiring this open course format.

---

## Introduction

In this module, students will learn how to curate the completeness and accuracy of StoryLayers by offering reviews and making edits to StoryLayer geometries and attributes.

This module includes the following lessons:

+	Lesson 1 – Peer Reviewing StoryLayers
+	Lesson 2 – Editing StoryLayer geometries
+	Lesson 3 – Editing StoryLayer attributes

## Lesson 1: Peer Reviewing StoryLayers

##### Objective

In this Lesson, students will learn how to review StoryLayers imported by their peers.

### Lecture

StoryScapes provides a variety of ways to review StoryLayers so that quality and accuracy can be continuously promoted and improved. In this Lesson we will cover the following Peer Review actions:

+ __Flag__ a StoryLayer
+ __Rate__ a StoryLayer
+ __Comment__ on a StoryLayer

##### Flagging a StoryLayer

Flagging a StoryLayer results in a notification being sent to a StoryScapes site Administrator. Administrators have a range of powers. They can deactivate problematic user accounts and unpublish or delete problematic StoryLayers and StoryScapes.

There are five reasons you might want to Flag a StoryLayer:
1. __Broken__: If you try and fail to perform any actions with a StoryLayer, such as playing the StoryLayer, editing the StoryLayer, or using the StoryLayer in a StoryScape), you can flag the StoryLayer as broken.
2. __Inappropriate__: If you see something in a StoryLayer that you feel is inappropriate, Flag it. The StoryLayer will not automatically be unpublished or deleted. An Administrator will determine what action should be taken.
3. __Missing Metadata__: If a StoryLayer lacks key metadata, such as a Data Source or Data Quality Statement, Flag it. An Administrator may respond by unpublishing the StoryLayer until appropriate metadata is added.
4. __Violates Terms__: StoryScapes users must abide by a set of Terms and Conditions. If you see anything that violates these Terms, Flag it.
5. __Other Issue__: Finally, you are invited to Flag anything else you deem necessary. Just include some text to describe your reasoning.

##### Rating a StoryLayer

Rate a StoryLayer on a five-star scale to communicate your overall feeling about its completeness and accuracy. There is no set rubric for StoryLayer ratings. In general, a rating of 1 means that you find the StoryLayer to be extremely incomplete and/or inaccurate. A 5 means you find the StoryLayer to be extremely complete and/or accurate.

As more and more people rate StoryLayers, the rating becomes a stronger reflection of the general population's true feeling on the StoryLayer.

The 5-star rating is another tool to help Storytellers determine if a StoryLayer is of high enough quality to use in a StoryScape.

##### Commenting on a Storylayer

Add a public Comment to a StoryLayer to communicate a message you feel all StoryScapes users need to be aware of when viewing a StoryLayer. For example, you might:
+ Add a comment describing your positive experience using the StoryLayer as part of a StoryScape
+ Add a comment that lets users know the areas this StoryLayer is in particular need of editing help
+ Add a comment letting users know about another StoryLayer that is complimentary, or that provides a contradictory perspective.

### Activity

Now its your turn.

1. To submit a Flag, first click into a StoryLayer. Click on Flag tool on the StoryLayer page. Select the Flag option you prefer and add any descriptive text that might be helpful. Click Submit.

2. To add your rating, simply find the rating tool on a StoryLayer page. Place your mouse on top of the star you'd like to assign, and Click.

3. To add your Comment, find the Share tab on a StoryLayer page. Simply type your Comment and click Post.

## Lesson 2: Editing StoryLayer geometries

##### Objective

In this Lesson, students will learn how to add, modify and delete feature geometries in a StoryLayer.

### Lecture

A StoryLayer is like a Wiki article where everyone can improve quality and accuracy through continuous editing. StoryLayer editing lets us draw on the vast knowledge - the "cognitive surplus" - that we all have about various phenomena of change in the world.

StoryLayers are comprised of features. Every feature in a StoryLayer has a geometry and attributes. The geometry determines how the feature appears on the map. Is it a point, line or polygon? And where is it located? The attributes determine the information we have _about_ the feature. For example, if your StoryLayer depicts schools in a town, you might have point geometries for each school location, and attributes for each school's name, student enrollment, grades served and whether the school os public or private.

In StoryScapes, you can edit (i.e. add, modify or delete) both geometry and attribute information for each feature.

### Activity

In this activity, we use a simple point StoryLayer depicting battles in the American Revolutionary War. The steps in the activity can reproduced with any similar dataset you have access to in StoryScapes. But, if you would like to do it with the same Revolutionary War dataset, you can access it in the Data folder and import the dataset before proceeding with this activity. `data/revolutionary_war.csv`

1. When you want to make any kind of change to a StoryLayer, you begin by clicking "Edit" from the StoryLayer detail page.

![](images/Screen Shot 2019-03-27 at 3.32.46 PM.jpg)\

In the StoryLayer Editor you will see the following buttons on the left-hand side:
+ Add Feature
+ Edit Feature
+ Metadata
+ View Table
+ View history
+ Exit

![](images/Screen Shot 2019-02-14 at 8.53.13 PM.jpg)\

2. To add one new feature, click `Add Feature`. A drawing tool will appear that lets you add a point feature for StoryLayers with points, or draw shapes for a StoryLayer with polygons. In this example we add a point to a StoryLayer depicting battles in the American Revolutionary War.

![](images/Screen Shot 2019-02-14 at 8.58.37 PM.jpg)\

3. After you've added a feature, a modal will appear where you can input time information for the feature as well as other attribute information. In this example we add a date for a hypothetical Revolutionary War battle in Halifax, Nova Scotia and give it the name 'Pretend Battle'

![](images/Screen Shot 2019-02-14 at 8.59.03 PM.jpg)\

4. Once the feature is edited, the action will be recorded in the `History` tab:

![](images/Screen Shot 2019-02-14 at 9.14.04 PM.jpg)\

 And, now when the StoryLayer is played, the newly added "Pretend Battle" appears in Halifax, Nova Scotia:

![](images/Screen Shot 2019-02-14 at 9.01.07 PM.jpg)\

5. If you have many features ready to add to a StoryLayer, rather than adding them one by one in the editor, you can `Append` them all at once. To append features to a StoryLayer, first click `Edit Layer` and then `Append Data`:

![](images/Screen Shot 2019-02-14 at 9.21.55 PM.jpg)\

 Doing so will bring up a modal where you can dowload a blank .csv or .shp file, depending on whether you are appending points (.csv) or polygons (.shp).

![](images/Screen Shot 2019-02-14 at 9.43.01 PM.jpg)\

6. Open the downloaded file, paste your features into it, and then return to the modal where you can upload the file.

![](images/Screen Shot 2019-02-14 at 9.46.54 PM.jpg)\

 Once you've done so, your appended features will appear as part of your StoryLayer.

7. If you see a feature in a StoryLayer that you believe is incorrect, you can delete it from the StoryLayer. To do so, simply click on the feature you want to delete. This will pop-up the feature's attribute information as well as a set of tools including a `Trashcan`. Click this to delete the feature. In this example, we delete the `Pretend Battle` in the American Revolutionary War StoryLayer that we created earlier.

![](images/Screen Shot 2019-02-14 at 9.53.32 PM.jpg)\

8. You may find a feature that you don't think needs to be deleted, but just needs to be moved to a different location. To modify a feature geometry, simply click on a feature inside the StoryLayer editor, just as you did to delete a feature. On the pop-up, click the `Edit Geometries` option. In the example below we are preparing to modify our `Pretend Battle` of the American Revolutionary War in Halifax, Nova Scotia:

![](images/Screen Shot 2019-02-14 at 10.04.10 PM.jpg)\

## Lesson 3:

##### Objective

In this Lesson students will learn how to edit attribute information about features in StoryLayers.

### Lecture

A StoryLayer is like a Wiki article where everyone can improve quality and accuracy through continuous editing. StoryLayer editing lets us draw on the vast knowledge - the "cognitive surplus" - that we all have about various phenomena of change in the world.

StoryLayers are comprised of features. Every feature in a StoryLayer has a geometry and attributes. The geometry determines how the feature appears on the map. Is it a point, line or polygon? And where is it located? The attributes determine the information we have _about_ the feature. For example, if your StoryLayer depicts schools in a town, you might have point geometries for each school location, and attributes for each school's name, student enrollment, grades served and whether the school os public or private.

In StoryScapes, you can edit (i.e. add, modify or delete) both geometry and attribute information for each feature.

### Activity

1. If you have attribute information _about a feature_ that you'd like to add, or you see attribute information that needs to be changed or removed, click on the feature in the StoryLayer editor and click `Edit Attributes`. This will bring up a modal where you can add, modify or delete attribute information. In this example we modify the name of 'Pretend Battle' to be 'Great Pretend Battle':

![](images/Screen Shot 2019-02-14 at 10.14.30 PM.jpg)\

2. Another way to make changes to feature attributes is from the `Table View`. To access the Table, click `View Table` on the left-hand sidebar of the StoryLayer editor:

![](images/Screen Shot 2019-02-14 at 10.23.16 PM.jpg)\

 From the Table View you can add, modify or delete information in individual cells, like a spreadsheet:

![](images/Screen Shot 2019-02-14 at 9.00.02 PM.jpg)\

## Conclusion

In this Module you learned the skills necessary to become a Curator for the StoryScapes community. You learned to peer review StoryLayers by doing things like adding comments or submitting Flags. And, you learned to edit feature geometries and attributes. The StoryScapes community depends on Curators who are both knowledgeable and committed to making regular edits. So your efforts are appreciated!

## Discussion Questions

Before moving on to the next Module, reflect independently or in a group on the following questions:

1. What kind of data projects can you think of that would benefit from the 'crowd-editing' model that StoryScapes provides?

2. What kind of data projects should not be subject to any curation or editing activities? What makes these projects different than others?

3. What are some of the risks involved with StoryLayer curation that need to be attended to?

4. Are there other examples of applications that offer data curation that have worked well? What factors do you attribute to success?

5. What other comments, questions or concerns do you have about this Module?
