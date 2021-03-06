
<img class="ui fluid centered image" src="/screenshots/CSLogo.png">

## CS
Collaborative Study (CS) is a scheduling app designed for UH ICS students to plan study sessions together. CS aims for ICS majors to form connections and better one another as students.
Users of this app will be able to:
* Maintain a public profile page
* Find, rate, and form groups with other students
* Join and create study sessions through a public calender
 

## Guided Tour

#### Public Landing Page

<img class="ui fluid centered image" src="/screenshots/publicLandingPage.png">
The first page users see before logging in is an informational page about Collaborative Study. Users will log in under the the "Account" dropdown using their UH username and password.

#### Profile Page

<img class="ui fluid centered image" src="/screenshots/profilePage.png">
Each user receives an editable profile page so others may learn more about them.

On this page, users can create a listing of courses under two categories, "Pros" or "Studs". Pros (short for "Professors") are classes students are competent in, while Studs (short for "Students") are classes they might need help in. Courses are color coded to reflect the individual's confidence of understanding of the subject matter; green: well understood, yellow: some gaps in understanding, red: limited knowledge.

#### Review Page

<img class="ui fluid centered image" src="/screenshots/reviewPage.png">
Accessed from the "Reviews" button on a profile, the reviews page is a listing of ratings and reviews left by other users about the profile's owner. Any user is welcome to submit reviews for another user, though they are regulated by an administrator after submission.

#### My Calendar Page

<img class="ui fluid centered image" src="/screenshots/myCalendar.png">
The Calendar page is a visual display of all upcoming public study sessions you have joined. Users may click on a day to create a study session for that day, or may click existing study sessions for more details.

#### Groups Page

<img class="ui fluid centered image" src="/screenshots/groupsPage.png">
When users become comfortable working with specific students, they can form a study "Group" to quicken the process of making study sessions with them. Users may create new groups or join existing ones through the groups page.

#### Study Session Page

<img class="ui fluid centered image" src="/screenshots/studySessionsPage.png">
A listing of all the upcoming study session created by users on CS. Study sessions may be searched for by course using the search bar at the top.

#### Study Session Details Page

<img class="ui fluid centered image" src="/screenshots/studySessionDetailsPage.png">
A more detailed explanation of a study session can be brought up, either through clicking the "More Info" button on the Study Session Page or clicking a study session on the calendar.
From here, users may join the study session as a Pro (tutor) or Stud (tutee). Students that join as Pros are welcome to add and remove topics that will be taught at that session.

#### Create Study Session Form

<img class="ui fluid centered image" src="/screenshots/createStudySessionPage.png">
Clicking on a day in the calendar results in a modal to create a study session on that day. Users will specify the session title, course, topic, start time and end time for their session.

####Public Calendar Page

<img class="ui fluid centered image" src="/screenshots/calendarPage.png">
The public Calendar page is a visual display of all upcoming public study sessions, including sessions that the user has not signed up for. Users may click on a day to create a study session for that day, or may click existing study sessions for more details.

#### Chat Room Page

<img class="ui fluid centered image" src="/screenshots/messagesPage.png">
A chat room for all online users is also available under the "Chat Room" tab.

## Developer Guide
If you would like to make modifications to this app, download Meteor ([here](https://www.meteor.com/)) and any IDE of your choice. Personally, our team enjoyed using [IntelliJ IDEA](https://www.jetbrains.com/idea/). Please note that you should be comfortable with HTML, Javascript, CSS, and Jquery before working on our code. The tutorials provided on the Meteor website should also help you get used to the platform.

After downloading Meteor, clone [our repo](https://github.com/CollaborativeStudy/CS) from GitHub and get working on it. You may run the app locally through the command line by changing to the "app" directory and running "meteor --settings ../config/settings.development.json".

When you are finished making changes, send us a pull request and we'll check it out!

## Who are we?
 We are CollaborativeStudy, a group of Information and Computer Science (ICS) majors at the University of Hawaii at Manoa. As ICS majors, we know best: the life of a computer science student can be a difficult and lonely one. It isn't unusual to be a lone wolf, studying by yourself. 
 
 Our organization came together to end that. Together, we are developing a student app that allows ICS majors to connect and study with other students. Doing this will create a fun and safe environment for students who want to make friends but are too shy or intimidated to do so. I hope you will support us throughout this development!

## Our Journey
 To view the progress we're making on the app, see our project milestones at http://github.com/CollaborativeStudy/CS/projects

## Initial User Study

 The test subjects were different majors. We wanted to see how other people would react to this app. We had one ICS major, and the rest were engineer majors, a communications major, an accounting major and a dental hygiene major. We separate these people into three group studies. We had them go to our website and use it without too much instruction. As they dive into our app, they provided all the feedback they could offered. 
 
 The majority agreed that overall the main features seemed to work okay however there were a few bugs. Sometimes tutorial blocks will not exit and some actions did not do anything. They even offered many suggestions for improvement. However, for a first test try we believe that we showed great features and a lot potential to our first users!
 
## Usability Test (4/11/17)

CS held it's second usability test on April 11th, 2017 with a group of three UH Manoa students of varying majors. Along with some bugs, we found two significant areas that need attention:
1) organization and reasoning behind certain elements of the app (most notably, the “proficiency” rating)
2) providing thorough explanation of usage, so as to ease the user experience

Suggested improvements and issues are listed below by the page they were designated for.

*My page*
- Course listing should include all possible ICS courses offered at UH Manoa
- Pro and stud sets should be disjoint; a user cannot be both a tutor and a tuttee at a subject
- Possibly rename “stud”, as it is common slang for being skilled at something
- Proficiency is unecessary if the courses are already being separated into pros and studs. It is redundant to have “high” proficiency as a pro and “low” proficiency if you're a stud. Additionally, it doesn't make sense to say one has “high” proficiency as a student.
- Include an “add all” option for courses
- If proficiency is kept as an aspect to the app, the tutorials should explain the color meanings and explain how to change it
- Red (used for low proficiency) is too bright and degrading

*Reviews*
- Should indicate when a user is not yet rated vs. having zero stars

*Create Study Session*
- Study session data should be editable
- Both pros and studs should be able to add topics, or, an explanation for why only pros can add topics should be included
- Buggy clicking to activate the modal from the calendar

*Chat*
 - Spam filter suggested to limit sending multiple messages in a short time period
 - Shift+enter should add a new line instead of sending message
 - Automatic scrolling when new messages are sent
- Timestamps

*Groups*
- Upload image option instead of solely URL
- “Member is already in this  group or does not exist” error unclear
- Button should say “Edit” instead of a picture, instead of being a picture and changing to “Edit” on hover
- Button animation doesn't continue after a click, instead remains as “Edit”

Group Sessions
- Buggy submission with modals unable to close
- Form should allow for more time options, along with a “Year” field for the date.
- Data validation to prevent “fake dates” (ex: February 30th) or dates significantly into the future from being submitted
- Fix padding on modals

*Study Sessions Page*
- Dates should be listed on cards instead of only in details

Tutorial*
- Tutorials should have instructions for first time users with arrows pointing to the topics in question

*General*
- Options for military time in addition to standard
- Back buttons

Thank you for the participants in the test. With this criticism, CS can improve to become much fmore useful and user-friendly.

### Authors and Contributors
Click our names for our online portolios or check out our githubs!<br>

[Mariah Gaoiran](https://mariahgaoiran.github.io/) (@mariahgaoiran) <br>
[Jipeng "Neal" Huang] (https://huang6606521.github.io/) (@huang6606521) <br>
[Chad Morita](https://chadmorita.github.io/) (@chadmorita) <br>
[Mary Santabarbara](https://marysantabarbara.github.io/) (@marysantabarbara) <br>

