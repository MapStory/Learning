# StoryScapes101 - Introduction to the StoryScapes platform
-----------

**This course curriculum includes six 3-hour modules, each with three one-hour lessons.

### Course Modules

+ [x] Module 1 - Conveying Intelligence with StoryScapes
+ [x] Module 2 - Composing StoryScapes 1.0
+ [x] Module 3 - Collecting StoryLayer Data
+ [x] Module 4 - Curating StoryLayer Data
+ [x] Module 5 - Composing StoryScapes 2.0
+ [x] Module 6 - Collaboration & Community Building with StoryScapes

### Course Goals

This course was designed to provide a comprehensive introduction to the StoryScapes platform to geoint professionals. Those who complete the course should feel comfortable integrating StoryScapes
into a range of geoint tasks, from managing and visualizing spatio-temporal data to adding analytical nuance to data that supports decision-making.

This course is a living work product and will be continuously modified and improved based on user feedback and as the StoryScapes platform evolves.

### Module Design

Each Module contains a folder designating which version of StoryScapes
it is written for (ex. `Module 1 Lab\StoryScapes 1.0\...`).  As new StoryScapes versions are released, the prior module version will be updated and stored in a new (appropriately named) folder.

Each module contains the following four resources:

+ **Module *n* Lessons.md** - Markdown file of lessons
+ **Module *n* Lessons.docx** - MS Word document of the lessons converted from Markdown
+ **figures** - Folder containing all images reference in the lessons
+ **Lessons *n* Data** - Folder containing all data referenced in the lessons. If the data is too large for GitHub, a Markdown file containing a link to the data will instead be included.

Each lesson within the module begins with a lesson title.

+ Lesson titles are always size Header 1 `# GST 10X - Course Title` and are the only size
Header 1 in the lab document.

The Lesson Objective is described next.

An attribution block is next as we always want to give proper attribution.

+ This Markdown document contains the attribution block:
[Attribution Block for Lab Documents.md][5].
+ Lab number and titles are always size Header 2 `## Lab n: Lab Title` and are the
only size Header 2 in the lab document.

Next, Lecture, Demo and Task content is provided.

+ These three sections are always size Header 3.

The lab Tasks (logical blocks of content) are next.

+ The last Task is always a challenge for the students to attempt on their own
without (m)any step-by-step instructions.

The last two sections are Conclusion and Questions.

+ These two sections are always size Header 3 `### Conclusion` and are always
sections 4 and 5 respectively.

When a figure is placed in the lesson document, the figure is never provided a number,
instead, it is referred to by its relative placement to the referring text (ex.
refer to figure below).  *All figures should be placed within the 'figures' folder
in the same directory as the Markdown document.

### Feedback
[Open an issue][7] or [fork and submit a pull request][8] on github, or, email [Richard.Smith@tamucc.edu][6].

### License: Creative Commons 3.0 License

This work is licensed under the Creative Commons Attribution 3.0 Unported License.  To view a copy of this license, visit <http://creativecommons.org/licenses/by/3.0/>.F

### Curriculum Document Format
All curriculum is written in [Markdown][3].  Markdown was chosen for these reasons:

+ [Markdown][3] is easy to learn and contains enough functionality to render the lessons.
+ With the lab documents converted to Markdown, GitHub can track all changes
to the document; this is not possible with, say, a Word or PDF document.
+ It is very easy to convert Markdown to multiple other formats using software
such as [PanDoc][4].

_Note: We are grateful to the GeoAcademy project for inspiring our open course design using Markdown._

[1]: http://www.geoforall.org/
[2]: http://spatialquerylab.com/projects/open-source-gis/
[3]: http://daringfireball.net/projects/markdown/syntax
[4]: http://johnmacfarlane.net/pandoc/
[5]: Attribution_Block_for_Lab_Documents.md
[6]: mailto:Richard.Smith@tamucc.edu
[7]: https://guides.github.com/features/issues/
[8]: https://guides.github.com/activities/forking/
