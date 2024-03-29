# Major Group Project
The starter code for the major group project.

Group members (3-5) (no Student IDs, only names):
1. Calvin Lapp (Squshy)
2. Paul Kerrigan (PPK44)
3. Henry Zheng (HenryZheng1998)


## How to use our project
To `login` you startup the app and input your username and password but if you have yet to create an account you can go to the create account text below the login form that is clickable which will open a dialog to register. To `register` you input a username, password, gender and birthday which will then take you to the home page of our app. To logout of the app you click on the logout button in the naviation the top left and it will open a dialog to confirm you want to logout.  

To see notifications working, go over to `mood/lib/notifications.dart`, in here you fill find a function called `_nextInstanceOfEightPM()`.  To view the notification working immediately, change the last parameter of `tz.TZDateTime scheduledDate = tz.TZDateTime(tz.local, now.year, now.month, now.day, 20);` to your speicifed hour.  If you want more precision then you can also add extra parameters for minutes, and seconds.  Make these changes and you will see a notification appearing at the specified time.   Keep in mind that this timezone is in UTC.

The `Calendar` page displays a calendar widget.  The individual days will change color according to the recorded moods on those days.  To see data appear here more than your current day, in the `mood/lib/views/loading_screen/loading_screen.dart` file, uncomment the line with the function call of `addEmBaby();`.  This should be on line 52. **PLEASE NOTE YOU WILL HAVE TO BE LOGGED IN PREVIOUSLY TO VIEW THESE CHANGES.  THIS WORKS OFF OF THE STORED ID IN SHARED PREFERENCES.  YOU WILL HAVE TO CREATE AN ACCOUNT IF YOU DO NOT HAVE ONE ALREADY, BE LOGGED IN AND THEN RESTART YOUR APP.**  After uncommenting and running it once, comment it out again so you do not fill the database with multiple entries for a single day.  

To add or edit a mood either navigate from the button displayed on the home screen, or through the navigation drawer.  Click the `Select Mood` button and it will take you to the specified page.  You can also do so from the `Calendar` page.  If you click on a colored day it will display a page with information about that day.  If you click on today it will take you to add a mood for today if you have not already.  If you have already added a mood for today and you click today's date, it will take you to a page displaying information about the mood.  At this page you can click a floating action button to edit the mood. 

On the `Settings` page, you can see an option for `Color Settings` and `Language Settings`.  If you click on `Color Settings` it will send you to a page where you can select colors you want displayed for certain moods.  After making changes you can save you changes and see them displayed throughout the application.  In the `Language Settings` page you can switch your languages.  Select which language you want and hit save and see the `Settings`, `Navigation`, and `Language Settings` pages translate. In the `Change Passowrd` page you can input a new password that you want to change and and a confirmation one as to make sure you submit the one you want.

From the navigation if you select `Chart`, this will take you to the `Chart` page.  Here is displayed a DataTable with information of all the moods for the user.  If you select the `Graph` option from the navigation it will take you to the `Graph` page.  On here it will show you a bar graph depicting the number of times each mood has been added for the current user.

From the navigation panel, if you go to the `Map` page, it will display a map that works similiar to `Lab09/10`.  This is added here for the requirement as we could not find a good use for maps in this project.


## Overview
This group project is designed for you to demonstrate the skills that you have learned in this course.  The final project that you submit in the last week of classes will be a completed mobile application.  Non-functional requirements, especially those associated with production-readiness, will be considered extremely important when marking this project.  You are expected to work in a group of three to five students when completing this project.  Students are not permitted to work alone on the project, as this eliminates one of the learning objectives of this assessment.  

_**Note:**  Any projects from individual students will not be accepted, except if special permission has been given by the instructor in advance._

## Detailed Instructions

### Choosing a Topic

The project topic is, for the most part, up to you.  Therefore, ensure that you choose a project topic that lets you demonstrate the skills learned in this course.  Consideration will be given to projects whose functionality is rather different from sample applications and those developed in assignments in this course.  When evaluating your project, I will consider this as requiring extra work.  More work done often equates to a higher grade.

It is acceptable if you want to do a project related to industry.  If someone you know wants a web application developed, and it lets you demonstrate the skills you’ve learned in this course, then you can use it for your project (even if you plan to sell that web application when you are finished).  Please keep in mind that nothing your prospective buyer says or does will affect the due date or expectations that I have for this project.  No matter what happens, this project is due when it is due, my expectations will be based on the content of this course, and I will expect a certain degree of professionalism and production-readiness.  Anything outside of the scope of this course will likely not earn you much, in terms of marks.  Proceed with caution.

### Basic Requirements

It is your job to incorporate as many course concepts into your project as possible.  At a minimum, your project must include the following:
- Dialogs and pickers
- Multiple screens and navigation
- Snack bars
- Notifications
- Local storage (SQLite)
- Cloud storage (Firestore or other)
- HTTP requests
- Data tables
- Charts
- Maps
- Geolocation
- Geocoding
- Internationalization

The actual size of the project (in terms of the number of screens, number of use cases, or amount of code) will differ from group to group.  Ultimately, the factor being considered is how much work appears to have gone into the project.  Larger groups will be expected to do proportionally more work.
If you incorporate concepts outside of this course (e.g. game engines, 3D graphics, sound) you will get credit, but in the subjective part of the evaluation only.  Thus, ensure that you meet the minimum requirements, outlined above, first.

### Game Development Alternative

Students who want to create a mobile game have the option to do so, but this topic won’t be covered until week 10 of the course.  Therefore, it is expected that this option will require significant self-learning to get a head start before the main lectures/examples covering game development.  The objective requirements, listed above, will be relaxed quite a bit for groups developing a game, but the expectations are just as high.  If you wish to pursue this option, please contact the instructor so that we can work out a set of expectations for the major project.

### Evaluation
When evaluating this project, the instructor and the TAs will attempt to give a metric to the amount of work involved, considering several important factors (design, cleanliness of code, code comments, variable/function naming, security checks, error checking, usability/user-friendliness/aesthetic, accessibility, and performance).  This metric will be affected by the size of your group (i.e. what will be evaluated is the average work done per group member).

The marking will occur in two phases.  The idea behind these phases is that your project should improve over time, so that the final product is comprehensive, professional, and production-ready.  It is hoped that your project will make a great portfolio item for when you apply for jobs.  The phased marking should also prevent groups from waiting until just a few days before the due date before starting their project.

### Formative Assessment
The first phase of marking, performed by a TA(s) in week 10.  This will evaluate whether or not you have included the topics from the first 9 weeks of the course, which will be mostly objective, but will also include a small subjective mark describing the work done, the user interface design, and the code/design quality.  A rubric will be included on Canvas, so you can verify in advance which topics will be included.  The purpose of the pre-evaluation is to give you an idea of the quality of your project before the end of the term, so that you can make any adjustments necessary to get the grade you want.  This evaluation will be worth 10% of your final grade.

#### Functional requirements (7 marks total)

Max Score | Requirement
--------- | ----------- 
1.50 | Multiple screens/navigation
1.00 | Dialogs and pickers
1.00 | Notifications
0.50 | Snackbars
1.50 | Local storage
1.50 | Cloud storage

#### Non-functional requirements (3 marks total)

Max Score | Requirement
--------- | ----------- 
1.00 | Amount of work done
1.00 | User interface design/usability
1.00 | Code and design quality

### Summative Assessment

The final phase of marking will be carried out exclusively by the instructor.  For students who have met all of the objective requirements, as evaluated in the first two marking phases, will be evaluated on a strictly subjective evaluation, similar to that done in the second phase.  This evaluation will be carried out more strictly, with higher expectations.  This evaluation will be worth 30% of your final grade.

#### Functional requirements (5 marks total)

Max Score | Requirement
--------- | ----------- 
0.50 | multiple screens and navigation
0.25 | dialogs and pickers
0.50 | snackbars and notifications
0.75 | local storage
0.75 | cloud storage
0.50 | data tables and charts
0.50 | maps
0.50 | geolocation
0.25 | geocoding
0.50 | internationalization

#### Non-functional requirements (25 marks total)

Max Score | Requirement
--------- | ----------- 
5.00 | code and design quality
5.00 | user interface design and usability
15.00 | amount of work done

## How to Submit
The project starter is available on GitHub Classroom, which really just has a `.gitignore`, since I want you to have freedom over this project.  There won’t be any starter code, you will start from scratch.  Accept the invite link for this project on GitHub Classroom (shared in Canvas), and use the new repository generated to store your project files.  This is setup as a group project, so one person can sign up, and others group members can also contribute to the project in that new repository.  

The instructor and the TA(s) will use this repository to download the latest version of your project, along with other information (e.g. commit logs) available through Git, when they want to mark the project.

_**Note:**  Only one of the group members will accept the GitHub Classroom invitation.  It is recommended that every member of the team verify the final repository on GitHub on submission day, so that everybody can be sure that the correct files were submitted and on time.  You should also clone the latest version into a fresh directory, and run it locally on your machine to ensure that it works without any unusual configuration._

_**Note:**  Work equity will be evaluated using the Git commit logs for your project.  If you decide to work together which results in a misrepresentation of work equity in the commit logs, be sure to mention this in your `README.md`._

To submit this project, please push all your work to your repository, and add the names of all group members names (but not their SIDs) and their corresponding GitHub usernames (so we can tell who made which commits) to the `README.md` file (at the top).

_**Note:**  Any instances of plagiarism will result in the student(s) receiving a mark of zero for the project, and further disciplinary action will be taken.  Plagiarism includes, but is not limited to:_
- Copying of (any amount of) work from the Internet, without proper citation
- Submitting a body of work, cited or not, that is primarily not your own work
- Copying of (any amount of) work from another student, past or present, without proper citation
- Allowing your own work to be copied by a fellow student

## Getting Help
If you run into difficulty, you may wish to check out some of the following resources:

- https://api.flutter.dev/  - The standard documentation for Flutter, all classes and methods.
- https://dart.dev/tutorials - A series of tutorials for the Dart programming language, focusing entirely on the features of Dart.
- https://flutter.dev/docs/reference/tutorials - A series of tutorials for the Flutter platform, focusing mainly on the widgets and API.
- https://flutter.dev/docs/codelabs - A series of deep-dive, more comprehensive, tutorials to learn more about the Flutter platform.
- https://flutter.dev/docs/cookbook - A set of recipes for commonly used features of Flutter.
- https://github.com/flutter/samples/blob/master/INDEX.md - A repository containing some completed Flutter applications.
- http://stackoverflow.com/ - A forum for asking questions about programming.  I bet you know this one already!

Of course, you can always ask the TA for help!  However, learning how to find the answers out for yourself is not only more satisfying, but results in greater learning as well.

## How to Submit
Create your flutter project, and copy it into this folder, commit, and then push your code to this repository to submit your major group project.
