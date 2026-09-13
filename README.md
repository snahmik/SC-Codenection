# Tidy

**Team:** Er Rui Xian, Ho Wan Zhen, Hans Kim Qin Duan, Ong Zi Rui. 
**Problem Statement:** Stress & Workload Manager. 
**Video Presentation:**  [https://youtu.be/2WJzPt55qns?si=oSkXS0_O-zssUMlS](https://youtu.be/2WJzPt55qns?si=oSkXS0_O-zssUMlS) 
**Presentation Slides:** [https://canv. .link/qmigoi7tq8240jg](https://canva.link/qmigoi7tq8240jg) 
## 1. Project Overview

## 2. Ideation and Process
### **Ideas**
- **Accepted Ideas**

| **Idea**                                              | **Why it was dropped / kept**                                                                                                                                                                    |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Task rescheduling suggestion                          | Reduces mental overhead required from users during a task rescheduling, allowing them to easily move tasks to a later day whilst being confident that they still have time to complete it later. |
| Stress score checking during task scheduling          | Prevents users from scheduling tasks/events that collide or otherwise cause tiredness/burnout.                                                                                                   |
| Stress score calculation and guided relaxations       | Daily stress score allows AI to determine whether adding a task to a given day may overwhelm a user. <br><br>Guided relaxation provides grounding and relaxation to users in high stress days.   |
| Profile establishment during app onboarding           | Responses to onboarding questions acts as a baseline value to be referenced from AI to provide personalised rescheduling suggestions and accurate stress score calculations.                     |
| Periodic well-being check-ins in AI chat              | The user's recent well-being allows AI to better determine a user's load capacity for a given day.                                                                                               |
| Contextual AI chat with persistent memory             | Allow the app's rescheduling suggestions to cater more towards a user's preferences, whilst making stress score calculations more accurate for users.                                            |
| AI chat panel serving as a user's primary entry point | Reduces cognitive load of users when using the app as tasks can be carried out using natural language.                                                                                           |
 - **Rejected Ideas**

| **Idea**                                                             | **Why it was dropped / kept**                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Interactive calendar view for scheduled tasks/events                 | There are plenty of well-established products that provide similar services, this feature does not make our product unique. Existing products include Notion Calendar, Google Calendar, Apple Calendar .etc<br><br>Instead of competing with existing calendars, we provide the functionality of our application whilst allowing users to still be using their preferred calendar app, reducing onboarding friction.                                                                 |
| Historical mood tracker that logs each mood entry provided by a user | Storing a log of mood entries does not align with our app’s core functionality of managing a student’s task and stress levels, and instead shifts our app to be more of an emotion/journalling app<br><br>Mood entries will only be used at the time of change itself for the AI to calculate a more personalised/accurate stress score alongside better rescheduling suggestions                                                                                                    |
| Focus timer for study sessions                                       | Focus timer implementations have been widely implemented across dedicated apps, social channels and OS level tools.<br><br>A focus timer shifts our app towards policing how a student studies minute-by-minute rather than preventing academic burnout before it happens. <br><br>Introducing such a feature introduces feature bloat that diverges from the main goal of the application, which also does not help in making our application different from existing applications. |
### Ideation Boards
1) AI Chatting User Flow
![[ai-chat-flow-chart.png]]
This flow chart illustrates the interaction of a user with the in-app AI chat. The interactions listed here would mostly take place within the AI chat panel itself, with dynamic message widgets that handles user interactions.
2) Task/Events Fetching User Flow
![[task-fetching-flow-chart.png]]
This flow chart illustrates the fetching of events and tasks from Google Calendar. It highlights the flow of core features within our app, including stress score calculations, task rescheduling suggestions and guided relaxations.

**Other flow charts that have been created to visualise our app's flow can be found in the following link:** [Miro Board](https://miro.com/app/board/uXjVHrxLcGc=/?share_link_id=632907770894) 
### Mentor Feedback

| **Date**                      | **Mentor**    | **Feedback Received**                                                                                                                                                         | **What Was Changed**                                                                                                                                            |
| ----------------------------- | ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 3 September 2026<br>21:15<br> | Khor Jia Quan | Personalised / Context-driven AI suggestions and stress calculations is something unique                                                                                      | Scope of application is focused on differentiating features (Personalisation of suggestions and stress calculation / AI chat panel) instead of generic features |
|                               |               | Prepare UI snapshots for better illustration of idea to allow for further feedbacks by mentors                                                                                | -                                                                                                                                                               |
| 9 September 2026<br>21:45<br> | Zach Kong     | Emphasise on the functionality of the AI chat panel, better integrating it into the application to allow users to use it as a primary method to interact with the application | Pre-existing UI is redesigned to complement the AI chat feature more, allowing smoother UX via the AI chat panel<br><br>                                        |
|                               |               | Configuring AI chat to have contextual awareness and long-term memory to provide users with a more personalised experience                                                    | AI suggestions and stress calculations adapt to ongoing user behaviour and mood, using onboarding responses only as a baseline.                                 |
|                               |               | Mood input can be handled by the AI chat instead as moods are difficult to quantify objectively                                                                               | The rigid mood selection menu is replaced with periodic AI check-ins<br><br>                                                                                    |
|                               |               | Abstracting the separation between Google Tasks and Google Events within our application since both task and event types have similar data fields                             | Task and event creation are no longer separated into distinct tabs. The appropriate API is now determined automatically from user input.<br>                    |

# 3. Design and Prototype

# 4. What Makes It Different
# 5. Technical Architecture & Feasibility