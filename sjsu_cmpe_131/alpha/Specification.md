# CMPE 131 | San Jose State University | Team 9

| Members | Position | [GitHub](https://github.com/shohinsan/sjsu_cmpe_131) |
| ----------- | ----------- | ----------- |
| Shohin Abdulkhamidov | Lead Software Engineer | [shohinsan](https://github.com/shohinsan) | 
| Adam Nguyen | Software Engineer | [RenRaiden](https://github.com/RenRaiden) |
| Thuy Tran | Software Engineer | [thuytran100401](https://github.com/thuytran100401) |
| Thomas Ng | Software Engineer | [hicbag](https://github.com/hicbag) |

---

- `Date:` September 16, 2021

- `Product Name:` Labiso ScholarRabbit

- `Problem Statement:` Cross-platform web app for students to access from all devices to study more effectively through 
memorizing, searching notes, and managing time to avoid distractions over period of their school time

---

### Features To Be Implemented In This Project
- General Features:
  * **Ability for users to sign-up, login/logout**
  * **Be able to delete Account**
- Memorizing:
  * **Input a markdown file and output flash cards.**
  * **Share flashcards (add to their account)**
  * Create pdf of flash cards to print
  * Change Order of Cards Based Off Accuracy 
- Notes:
  * **Render Markdown Notes**
  * **Convert Markdown to PDF**
  * **Share Notes With Other People (Add to Their Account)**
  * Find text in files
  * Quickly rename files using regular expressions
- Time Management: 
  * **Create Time Blocks** 
  * **Use Pomodoro Timer** 
  * Track hours worked per day
  * Track Assignments/Projects Worked on/Finished 

---

### 1. Ability for users to sign-up, login/logout
### Non-functional Requirements
- System responds to each {User} input within milliseconds.
- Cross-platform access through the web
- Consider using English, but later add other languages as well.
### Summary
- Creating an account for a new user
### Actors
- {User}
### Preconditions
- {User} does not have an account
### Triggers
- {User} needs to sign-up
### Primary Sequence
- {User} clicks “Sign Up” button
- {User} enters personal information
- {User} checks if username is not taken
- {User} makes unique password
- {User} verifies password through verification (2nd time)
- {User} submits
- System eventually creates a new account
### Primary Postconditions
- {User} account has been added to website
- {User} is able to login
### Alternate Sequences
- System displays an error
- System prompts user to enter different data
- Password entered does not match
- System displays an error to the {User}
- System prompts {User} to type password again
### Alternate Trigger
- Ability for {User} to create an account using outside sources like Google, Facebook, and etc.
### Alternate Postconditions

---

### 2. Be Able To Delete An Account
### Non-functional Requirements
### Summary
- Ability for users to remove an account from database.
### Actors
- {User}
### Preconditions
- {User} must have an account
### Triggers
- {User} decision to delete an account
### Primary Sequence
- {User} clicks deactivate an account in the settings
- Modal prompts to {User} if they are sure to remove an account?
- {User} confirms his decision to delete an account
- System removes {User} account from database
### Primary Postconditions
- {User} account has been removed from database
- {User} is not able to login
### Alternate Sequences
### Alternate Trigger
- {User} needs to approve removal of their account using Two-Factor Authentication in order to proceed request
### Alternate Postconditions

---

### 3. Input a Markdown File And Output Flash Cards
### Non-functional Requirements
### Summary
- Ability for users to upload Markdown file and get flashcards back based off the input
### Actors
- {User}
### Preconditions
- {User} is logged in
- {User} uploaded Markdown file
### Triggers
- System outputs and visualizes file as a Note
### Primary Sequence
- Markdown file has been visualized as a note
### Primary Postconditions
- {User} outputs visualized note
### Alternate Sequences
### Alternate Trigger
- {User} uploads shared link from third-party source
### Alternate Postconditions

---

### 4. Share Flashcards (Add to their account)
### Non-functional Requirements
### Summary
- Ability for users to share notes with others 
### Actors
- {User1}
- {User2}
### Preconditions
- {User1} must be signed in.
- {User1} has flashcards on account
### Triggers
- {User1} clicks Share button from specific note
- {User2} receives a notification
### Primary Sequence
- {User1} clicks share button
- System pops up modal "done" 
### Primary Postconditions
- {User1} has shared note to {User2}
- System shows the same Note to {User2}
### Alternate Sequences
- Ability for {User1} to copy/paste the link for third-party sources
### Alternate Trigger
- Ability for {User1} to share the link directly to social media
### Alternate Postconditions

---

### 5. Create pdf of flash cards to print
### Non-functional Requirements
### Summary
- Users can create a pdf of flash cards so that they can print
### Actors
- {User}
- Flashcard
### Preconditions
- {User} must be signed in.
- Flashcards must exist on the account
### Triggers
- {User} selects "create pdf" button
### Primary Sequence
- {User} clicks the "Create PDF" button
- {User} chooses the flashcard
- System creates PDF
### Primary Postconditions
- PDF has been created
- Ability for {User} to download or print PDF file
### Alternate Sequences
- System displays an error
- System asks to select Flashcard again
### Alternate Trigger
- {User} share pdf directly to social media
### Alternate Postconditions
- {User} does not have Flashcard to print

---

### 6. Change Order of Cards Based Off Accuracy
### Non-functional Requirements
### Summary
- When doing flashcards, change the order of the cards based off previous attempts at memorizing
### Actors
- {User}
- Flashcard
### Preconditions
- {User} must be signed in.
- Flashcard must exist on the account
- {User} must attempt to memorize
### Triggers
- Order of cards will be automatically changed when {User} attempts.
### Primary Sequence
- {User} chooses Flashcard to attempt
- System automatically changes the order
### Primary Postconditions
- Order of cards has been changed
### Alternate Sequences
- System displays an error
- System keeps changing the order of cards
### Alternate Trigger
### Alternate Postconditions
- {User} attempts to delete the card

---

### 7. Mind map of Flashcards
### Non-functional Requirements
### Summary
- Ability for users to input Flashcards in order to create a mind map. 
Starting point is the map while Flashcards are the branches. System will prompt {User} to input a 
starting map and will ask {User} to input Flashcards as the branches. 
### Actors
- {User}
### Preconditions
- {User} is logged in
- {User} has Flashcards
### Triggers
- {User} sends request to Mind Map to visualize their Flashcards
### Primary Sequence
- {User} clicks “Create Mind Map using Flash Cards”
- System prompts {User} to input starting point map
- System prompts {User} to input branch(es) for map(s)
- {User} clicks finish map
### Primary Postconditions
- {User} will be able to view their mind map
### Alternate Sequences
### Alternate Trigger
- {User} is using Mind Map of Flashcards for the first time
### Alternate Postconditions
- {User} does not have Flashcards

---

### 8. Render Markdown Notes
### Non-functional Requirements
### Summary
- Rendering markdown notes on the flash cards.
### Actors
- {User}
- Flashcard

### Preconditions
- {User} must be logged in. 
- Flashcards must exist on the account. 
- At least there should be some notes on the Flashcard.

### Triggers
- {User} used specific key to activate the “render markdown notes” option. 
### Primary Sequence
- {User} chooses notes on the flash card
- {User} uses specific key 
- System renders the notes

### Primary Postconditions
- The markdown notes have been rendered.
- The markdown notes can be seen. 

### Alternate Sequences
- System displays error.
- System asks to use a valid key.
- System prompts {User} to mark down some notes.

### Alternate Trigger
### Alternate Postconditions
- There is no notes on the Flashcard to Markdown

---

### 9. Convert Markdown to PDF
### Non-functional Requirements
### Summary
- Users can convert markdown notes to a PDF format.
### Actors
- {User}
- Flashcard
- Note
### Preconditions
- {User} must have created notes on the Flashcard
- {User} is signed in 
- Flashcards must exist on the account.
### Triggers
- {User} selected the “convert markdown to pdf” option.
### Primary Sequence
- {User} selects notes to convert
- {User} clicks “convert to pdf” button
- System converts the selected notes to pdf format

### Primary Postconditions
- Markdown notes have been converted to pdf.
### Alternate Sequences
- System displays error
- System asks {User} to do the sequence again. 
### Alternate Trigger
- Markdown pdf notes could be used to print and share to social media.
### Alternate Postconditions
- No markdown to convert to pdf.

---

### 10. Share Notes With Other People (Add to their account)
### Non-functional Requirements
### Summary
- User can share notes with other people by adding a note to their account
### Actors
- {User1}
### Preconditions
- {User1} must be signed in
- {User1} has a note
### Triggers
- {User} requires adding a note to another user 
### Primary Sequence
- {User1} clicks "Add Note" by another user's name
- System prompts user to input note
- {User1} clicks "finish"
### Primary Postconditions
- {User1} and other user(s) will be able to view note made by {User1} 
### Alternate Sequences

### Alternate Trigger
- {User} adds note(s)
- {User} delete note(s)
### Alternate Postconditions
- {User} does not have notes

---

### 11. Find Text in Files
### Non-functional Requirements
### Summary
- Ability for users to find specific strings of text within their files 
### Actors
- {User}
### Preconditions
- {User} is signed in 
- {User} has files on account
### Triggers
- Search function for files on account
### Primary Sequence
- System prompts user with "search box"
- {User} types in a string in question
- System lists the files when the string is found in
### Primary Postconditions
- {User} is able to quickly find text within their account files
### Alternate Sequences
- System prompts {User} with error saying text not found 
### Alternate Trigger
- Text requested does not exist within account
### Alternate Postconditions

---

### 12. Quickly rename files using regular expressions
### Non-functional Requirements
### Summary
- Ability for users to quickly rename files on account using simple and known expressions
### Actors
- {User}
- System
### Preconditions
- {User} is logged in 
- {User} has files on account 
### Triggers
- {User} clicks on a file to rename
### Primary Sequence
- System prompts user with a text box 
- {User} uses expressions to rename file 
- System updates file names
### Primary Postconditions
- Files specified on account are renamed
### Alternate Sequences
- System prompts user with error saying there are no files 
### Alternate Trigger
- There are no files on account 
### Alternate Postconditions

---

### 13. Create graph (nodes and edges) of connections between notes
### Non-functional Requirements
### Summary
- Ability for users to create a graph which connects notes using nodes and edges.
### Actors
- {User}
### Preconditions
- {User} is logged in
- {User} has notes to input or existing notes
### Triggers
- User requires notes or existing notes
### Primary Sequence
- {User} clicks “Create Graph of Connection between Notes”
- System prompts {User} to input notes or choose existing notes
- System prompts {User} to assign a node to each note
- System prompts {User} to assign edge(s) between nodes
- System generates graph
### Primary Postconditions
- {User} will be able to view graph of connection between notes
### Alternate Sequences
- Error duplicate node
- Error duplicate edge
### Alternate Trigger
- First time using graph of connections between notes
### Alternate Postconditions
- {User} does not have notes

---

### 14. Create Time Blocks
### Non-functional Requirements
### Summary
- {User} will be able to add time blocks scheduling out their 
### Actors
- {User} 
- System
### Preconditions
- {User} is logged on 
### Triggers
- {User} clicks “add time blocks” 
### Primary Sequence
- {User} is prompted with Excel type table 
- {User} can click and drag to create blocks
- System saves data of block
### Primary Postconditions
- {User} will now have the ability to see timeblocks (see Visualize Timeblocks) 
### Alternate Sequences
### Alternate Trigger
### Alternate Postconditions

---

### 15. Use Pomodoro Timer
### Non-functional Requirements
### Summary
- Ability for users to use Pomodoro timer to help with study sessions.
### Actors
- {User}
- System
### Preconditions
- {User} is logged in
### Triggers
- {User} navigates to the timer
### Primary Sequence
- {User} is prompted with a timer
- {User} can select short or long break
- {User} can click start to start the timer
- System will run timer for 25 minutes (default time)
- A second timer will be run for 5 minutes (short break) or 10 minutes (long break)
- System will reset the timers
### Primary Postconditions
- {User} can see how ong they have studied/worked (see Track Hours worked per day use case)
### Alternate Sequences
- {User} can change the study timer or break time
- Timer will run for different lengths based off those preferences
### Alternate Trigger
- {User} changes the settings
### Alternate Postconditions

---

### 16. Track Hours Worked Per Day
### Non-functional Requirements
### Summary
- Ability for users to add hours studied/worked per day 
### Actors
- {User}
- System (Pomodoro Timer)
### Preconditions
- {User} is logged in
- Pomodoro Timer is used
### Triggers
- Pomodoro Timer is run 
### Primary Sequence
- {User} will navigate to the hours worked view 
- System prompts user with a daily calendar view with numbers of hours/minutes worked 
## Primary Postconditions
- Ability for {User} to see time worked per day 
### Alternate Sequences
- System shows calendar view with nothing on it 
### Alternate Trigger
- {User} never used the Pomodoro timer 
### Alternate Postconditions

---

### 17. Track Assignments/Projects Worked on/Finished
### Non-functional Requirements
### Summary
- Ability for users to check off and list their projects/assignments to see what they have done and what still needs to be done
### Actors
- {User} 
- System
### Preconditions
- {User} has an account 
- {User} is logged in 
### Triggers
- {User} initially clicks “assignments” 
- {User} clicks “add assignments” 
- {User} clicks on an assignment
### Primary Sequence
- {User} is brought to calendar view
- {User} clicks add assignments
- {User} is prompted with form to enter assignment name, description, and date due 
- {User} submits
- System inputs data into {User} account 
- System shows on calendar
### Primary Postconditions
- {User} has assignments listed on their account and their due dates 
- {User} can “close” assignments and mark them as done aiding in productivity and time management
### Alternate Sequences
- {User} clicks on an assignment 
- {User} is prompted with assignment information 
- {User} can close assignment to remove it from the calendar 
- System add assignment to finished list 
### Alternate Trigger
### Alternate Postconditions

---

### 18. Visualize Time Blocks
### Non-functional Requirements
### Summary
- Ability for users to see the time they allotted for themselves on a calendar 
### Actors
- {User} 
- System
### Preconditions
- {User} is logged in 
- {User} has created time blocks
### Triggers
- {User} views the calendar
### Primary Sequence
- {User} goes to calendar view
- System displays added time blocks on calendar 
- Ability for {User} to change color of blocks for organization
### Primary Postconditions
- Ability to see time blocks added to account by {User} 
- {User} can recolor blocks 
### Alternate Sequences
- If no time blocks are on account the system won’t display anything
### Alternate Trigger
### Alternate Postconditions

---

### 19. Visualize Hours Worked and Projects
### Non-functional Requirements
### Summary
- Ability for users to view their hours worked and projects on a time chart
### Actors
- {User}
### Preconditions
- {User} is logged in
- {User} has hours worked
- {User} has project
### Triggers
- {User} requires information about their work hours
### Primary Sequence
- {User} clicks “Add Visualize Hours Worked and Projects” 
- System prompts {User} to input hour(s) worked
- System prompts {User} to input project(s)
- System generates timetable visualizer
### Primary Postconditions
- {User} will be able to view hours worked and projects on a time chart
### Alternate Sequences
- Invalid time display error
### Alternate Trigger
- First time using visualize hours worked and projects
### Alternate Postconditions
- {User} does not have hours worked and projects

---
