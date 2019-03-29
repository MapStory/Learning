# StoryScapes101: Introduction to the StoryScapes platform

## Module 3 - Collecting StoryLayer Data

Document Version: 01/29/2019

---

This work is licensed under the Creative Commons Attribution 3.0 Unported License.  To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/ or send a letter to Creative Commons, 444 Castro Street, Suite 900, Mountain View, California, 94041, USA.

Also, credit to GeoAcademy for inspiring this open course format.

---

## Introduction

In this module, students will learn to import data to make point, line and polygon StoryLayers. A StoryLayer is a data file that is used to display geographic information with temporal attribute(s) on StoryScapes.

This module includes the following lessons:

+	Lesson 1 – Importing point StoryLayers
+	Lesson 2 – Importing polygon StoryLayers
+	Lesson 3 – Writing High Quality Metadata

## Lesson 1: Importing point StoryLayers

#### Objective
In this lesson students will learn to import a `.CSV` file with point features and write high-quality metadata.

### Lecture

#### Get your data "StoryScapes Ready"
To import data, you'll use the import modal, which is accessible from your profile, from the header, or from the StoryScapes homepage.

![](images/Create-Dropdown.JPG "Create Dropdown")\

To successfully import your data into StoryScapes, you’ll need to make sure your data conforms to the required _file, projection, and time_ formatting types.

Required file types

+ StoryScapes supports data imports in the **.csv** format (for points) and the **.shp** format (for points, lines or polygons)

Required projections

+ StoryScapes requires all data to be projected using the 4326 projection.

Required formatting

+ StoryScapes requires that all data imported have time attributes, as well as location/geometry information (Lat, Lon).
+ Time attributes should be presented in **ISO 8601** or one of the following formats:
	- yyyy
	- Jun 2012—MMM-y
	- May/15/2012—MMM/d/yyyy
	- 11/1/2012—M/d/y
	- yyyy-MM-dd'T'HH:mm:ss.SSS'Z'
	- yyyy-MM-dd'T'HH:mm:sss'Z'
	- yyyy-MM-dd'T'HH:mm:ss'Z'
	- yyyy-MM-dd'T'HH:mm'Z'
	- yyyy-MM-dd'T'HH'Z'
	- yyyy-MM-dd
	- yyyy-MM

### Activity

This example uses a simple csv point dataset. To access it, go to the Data Folder and download `data/module-3-csv-points.csv`

![](images/sample-csv-data.JPG "See module-3-csv-points.csv")\

1. Once you have your data prepared, go to "Create" and "Import StoryLayer" at the top of your screen.

2. Upload your data file

3. Name your StoryLayer.

 ![](images/Import-Wizard-CSV-4.JPG "Name your StoryLayer")\

4. Confirm that the storylayer has time attributes.

 ![](images/Import-Wizard-CSV-5.JPG "Select StoryLayer Time Attribute")\

5. Configure time information.

 ![](images/Import-Wizard-CSV-6.JPG "Select StoryLayer Time Attribute")\

6. Enable versioned editing.~~

 ~~![](images/Import-Wizard-CSV-X.JPG "Enable Version Editing")\~~

7. Finalize upload.

 ![](images/Import-Wizard-CSV-7.JPG "Confirm Upload")\

## Lesson 2: Importing Polygon StoryLayers

#### Objective
In this lesson, students will learn how to import a Shapefile with polygon or line features.

### Lecture

#### Get your data "StoryScapes Ready"

To import a polygon StoryLayer, you will likely use a Shapefile. Currently, our importer accepts **zipped** shapefiles for points, lines and polygons. If you have experience with common GIS workflows, this will be familiar to you. If not, it is a good idea to consult more comprehensive lessons on how to work with GIS data.

#### Importer Modal

Importing a polygon layer with a Shapefile is very similar to importing a point layer with a .CSV file.

A key difference is that you must first zip the constitutent files into a single zipped files.

For example, if you export your shapefile you will have several files that are siblings of each other

![](images/SHP-Files-1.JPG)\

When you zip these files, make sure to include _only_ the `SHP`, `SHX`, `DBF`, and `PRJ` files.

![](images/SHP-Files-2.JPG)\

#### A Note on Temporal Data Format

StoryScapes reads a temporal attribute (or two temporal attributes) to iterate over time. Therefore, each feature must have a _geometry_ and _time_ attribute. If you're data is arranged so that each temporal value is an attribute you will have to "stack" them.

So Data like the following:

![](images/Temporal-Data-1.JPG)\

Would become something like this:

![](images/Temporal-Data-2.JPG)\

### Activity

Try importing a Shapefile of your own. In the Data folder we provide a pre-zipped dataset ready for import. Its the ISIS Area of Territorial Control dataset that is used in Module 2. Access the data at `data/changing_areas_of_isis_control.zip`.

Follow the same steps you used in the previous lesson:

1. Go to "Create" and "Import StoryLayer" at the top of your screen.

2. Upload your data file

3. Name your StoryLayer.

4. Confirm that the storylayer has time attributes.

5. Configure time information.

6. Enable versioned editing.

7. Finalize upload.

## Lesson 3: Writing High-Quality metadata

#### Objective

In this Lesson students will learn how and why to write metadata once they have successfully imported a StoryLayer.

### Lecture

Once your StoryLayer is successfully created, you will be taken to the Metadata Modal to complete your metadata.

Completing high-quality metadata (or “data about the data”) for StoryLayers is absolutely vital when using StoryScapes. Without metadata, other users have no way to adjudicate the quality and reliability of content shared. StoryScapes requires the following Metadata fields for all StoryLayers:

+ __Title__: The title should make it clear what the StoryScape is about.  It is also appropriate to include the start and end dates for the StoryScape in the Title.  Here's an example Title: "Patterns of US Population Growth (1790-Present)".
+ __Summary__: The Summary is where you provide a brief description so that the reader will quickly understand what the content is about.
+ __Language__: Language of Source Data
+ __Data Source(s)__: Write where you got your data here.  Include hyperlinks to the original data source if available. Here is an example of a data source statement, which was used for a StoryLayer on global border changes: _The Humanitarian Information Unit in the Department of State provided Simplified World Polygons at https://hiu.state.gov/data/data.aspx._
+ __Data Quality Statement__: The Data Quality Statement is a general explanation of the data producer’s knowledge about the lineage of a dataset. This is your opportunity to admit the limits in your data and areas where it could be improved by others.
+ __Purpose__: Under purpose, write about why you created this StoryLayer.  This information will help others learn whether they should use your StoryLayer in their StoryScape. For example, a StoryLayer depicting country border changes by decade would not be a good StoryLayer to use in a StoryScape about the changing territorial control of the Syrian Government by month during the Syrian Civil War.

The Metadata Modal also allows the StoryLayer owner to determine if the StoryLayer should be published and therefore viewable by anyone, or private and only viewable by the StoryLayer owner. If you own the StoryLayer, you can return to the Metadata Modal and update the metadata at any time.

### Activity

Now it's your turn! Go to one of the StoryLayers you imported in a previous lesson and click `Edit StoryLayer` and then `Metadata`. Take the time to write as high-quality metadata as you can. Note the questions where you don't have good responses, and think about what kind of strategies you would undertake to find answers for these questions.

## Conclusion

Over the course of this module, you've learned how to get data from files and schema uploaded and imported into the platform. You've also seen how to update and maintain good metadata which is important for data validity and usability.

This creates the foundation for developing rich and meaningful StoryScapes.

## Discussion Questions

Before moving on to the next Module, reflect independently or in a group on the following questions:

1. What kids of data sources are you aware of that could be accessed for data to import into StoryScapes?

2. What are some of the issues that we need to think about in terms of data that is appropriate or inappropriate for import into StoryScapes?

3. What other kinds of data formats besides .csv and .shp do you work with and feel StoryScapes should be able to support?

4. How does adding the dimension of _time_ to geospatial data change the field of GIS? What are the benefits you see, and the drawbacks?

5. What other comments, questions or concerns do you have about this Module?
