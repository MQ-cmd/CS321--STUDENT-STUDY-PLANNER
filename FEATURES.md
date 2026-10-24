## Project Features Document


## 1. Project Overview

The Student Study Planner is a web-based application designed to help college students organize their coursework, manage deadlines, and develop personalized study schedules.

The main goal of our project is to go beyond a traditional calendar or assignment tracker by creating a system that helps students determine what to study, how much time to spend studying, and when to complete their academic responsibilities.

Our application will use a calendar-centered interface where students can view upcoming assignments, quizzes, exams, and scheduled study sessions. Based on their courses, workload, deadlines, and personal availability, the system will recommend study schedules and help students manage their time more effectively.

## 2. Planned Features

### 2.1 Student Onboarding and Course Management

When students first use the application, they will complete a setup process to personalize their study planner.

Students will be able to:

- Add and manage courses for the current semester.
- Rate the difficulty of each course on a scale of 1–5.
- Enter their available study hours for each day of the week.
- Set preferred study times and academic goals.
- Update their course information and availability as needed.

This information will serve as the foundation for the application's study scheduling recommendations.

### 2.2 Interactive Academic Calendar

The calendar will serve as the application's main interface, allowing students to manage their academic responsibilities in one place.

The calendar will support:

- Monthly and weekly views of assignments, quizzes, exams, and study sessions.
- Adding, editing, and removing calendar events.
- Color-coded events to distinguish between courses.
- Visual indicators for approaching deadlines and overdue assignments.
- Viewing detailed information by selecting a calendar event.

The interface will also include a navigation sidebar for accessing courses, assignments, study schedules, and other features.

### 2.3 Assignment and Task Management

Students will be able to create and organize their academic tasks within the application.

Each task may include:

- Assignment or assessment title.
- Associated course.
- Due date and time.
- Assignment type, such as homework, quiz, project, or exam.
- Estimated time required.
- Priority level.
- Completion status.

Students will be able to mark assignments as completed, edit existing tasks, and filter their coursework by deadline, course, or priority.

### 2.4 Smart Study Scheduling and Prioritization

One of the primary features of our application will be its ability to recommend personalized study schedules.

The system will consider several factors when determining how students should allocate their time:

- Course difficulty.
- Assignment type and estimated workload.
- Upcoming deadlines.
- Available study hours.
- Assignment priority and completion progress.

Using these factors, the application will recommend study sessions and organize them around the student's availability.

For example, if a student has an exam in a difficult course and several smaller assignments due during the same week, the system will attempt to distribute their study time according to urgency and estimated effort.

The scheduling system will initially use custom rule-based algorithms, with the possibility of more advanced recommendations later.

### 2.5 Adaptive Scheduling and Progress Tracking

The application will help students adjust their study plans when they fall behind.

If a student misses a scheduled study session or leaves an assignment incomplete, the system will recommend changes to the remaining schedule based on the time available before upcoming deadlines.

Students will also be able to monitor their progress through task completion indicators and summaries of their academic workload.

If the remaining workload exceeds the student's available study hours, the application will display a warning rather than create an unrealistic schedule.

### 2.6 Canvas Calendar Integration

We originally considered integrating Canvas directly through its API to retrieve courses, assignments, and deadlines. However, after investigating GMU's Canvas settings, we found that students are restricted from generating their own API access tokens.

As an alternative, we plan to explore using the Canvas Calendar Feed in iCalendar (.ics) format.

This integration would allow students to:

- Import assignments and calendar events from Canvas.
- Retrieve event titles and due dates from available calendar data.
- Add imported events to their study planner.
- Organize imported events by course when course information is available.
- Avoid duplicate entries when importing updated calendar information.

We may also explore subscribing to calendar feeds for periodic synchronization.

Because calendar feeds do not necessarily include complete course details, assignment instructions, grades, or submission status, students will still be able to enter and update information manually.

### 2.7 Notifications and Reminders

The application will help students stay aware of approaching deadlines and incomplete coursework.

Planned functionality includes:

- Reminders for upcoming assignments and exams.
- Warnings for overdue or incomplete tasks.
- Notifications when scheduled study sessions are missed.
- Customizable reminder preferences.

We may also implement email notifications so students can receive reminders outside the application.

### 2.8 AI-Assisted Study Resources

An advanced feature we are considering is an AI-powered study assistant that helps students find educational resources related to their assignments, quizzes, and exams.

For example, if a student has an upcoming quiz covering sorting algorithms, the system could recommend relevant YouTube tutorials, GeeksforGeeks articles, and other educational resources.

Students would be able to enter the topics covered by an assessment, and the application would use that information to search for useful study materials.

The purpose of this feature is to make it easier for students to find resources without having to search multiple websites themselves.

The application would aim to provide links to real, relevant resources rather than generating unverified references.

### 2.9 Study Analytics

We are also considering adding an analytics section to help students understand their study habits and academic workload.

Potential features include:

- Tracking total study hours each week.
- Displaying assignment completion rates.
- Comparing estimated study time with actual time spent.
- Identifying weeks with unusually high workloads.
- Visualizing study progress through charts.

These insights could help students improve their time management and make adjustments to their study schedules.

## 3. Proposed Technologies

We are considering the following technologies for the development of our application:

- **Frontend Development:** React, JavaScript, HTML, and CSS for building the website's interface, calendar, dashboard, and navigation components.

- **Calendar Interface:** FullCalendar for displaying assignments, deadlines, and study sessions through an interactive calendar.

- **Backend Development:** Node.js and Express for handling application logic, assignment management, scheduling operations, and communication between the frontend and database.

- **Database:** SQLite for storing course information, assignments, study schedules, user preferences, and completion records.

- **Canvas Integration:** ical.js for processing Canvas Calendar Feed (.ics) files and extracting calendar events.

- **Study Scheduling:** Custom JavaScript algorithms for calculating assignment priorities, allocating study hours, and adjusting schedules.

- **Version Control:** Git and GitHub for managing source code, documenting progress, tracking issues, and collaborating with team members.

- **Email Notifications:** Nodemailer with an appropriate email service provider for potential deadline and task reminders.

- **AI Integration:** External AI and resource-search APIs for potentially generating personalized study recommendations and locating educational materials.

These technologies are currently proposed and may be adjusted as the project develops.

## 4. Development Plan

We plan to develop the application in stages, beginning with the essential features before introducing more advanced functionality.

### Phase 1 – Minimum Viable Product (MVP)

Our initial goal is to create a working application that demonstrates the main functionality of the Student Study Planner.

The MVP will focus on:

- Student onboarding and course setup.
- Manual assignment and task management.
- Interactive academic calendar.
- Course difficulty configuration.
- Basic study schedule generation.
- Assignment prioritization.
- Completion tracking.

### Phase 2 – Additional Functionality

Once the core application is working, we plan to expand it with:

- Canvas calendar import.
- Adaptive scheduling improvements.
- Deadline reminders and notifications.
- Additional usability improvements.

### Phase 3 – Advanced Features

Depending on our progress and available development time, we may implement:

- AI-assisted study resource recommendations.
- Email notifications.
- Automatic calendar feed synchronization.
- Advanced study analytics.

## 5. Project Goals and Expected Outcome

Our primary goal is to develop a functional and user-friendly academic planning system that helps students organize their coursework and manage study time more effectively.

By combining an interactive calendar, assignment management, course difficulty estimates, and personalized scheduling recommendations, we hope to create an application that offers more practical assistance than a traditional calendar.

The project will also allow our team to apply software engineering concepts such as requirements analysis, software architecture, collaborative development, testing, and project management.

Our expected outcome is a working web application that demonstrates these concepts while providing students with a useful tool for planning and managing their academic responsibilities.
