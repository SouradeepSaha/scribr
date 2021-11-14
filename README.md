# Scribr - An automated note taking app
This project was submitted to Garuda Hacks 2020 [Devpost Submission](https://devpost.com/software/scribr-7t9gpu) and was selected for the best pre-university hack.

## Inspiration
Simply put, students find the sudden transition to online lectures draining and lack motivation as it can be difficult to pay attention to online lectures. Not only are students not used to this new method of information delivery but the process can also be very repetitive and tiring as students adjust to their new digital learning environment. To lessen the load on students, our team developed Scribr with the goal of providing teachers an easier way to help their students with online education by reducing stress and making online education more accessible for students with various learning styles.

## What it does
Scribr is a chrome extension intended for teachers who will be providing classes online that records their lecture, transcribes it into text, and summarizes it automatically. Scribr eases the transition to online education for both teachers and students as it is a tool that makes creating and sharing lesson notes more effective. With Scribr, you can get the fully punctuated transcript of a spoken lecture, the essential points of the lecture in the form of a summary, and the ability to easily share the notes with students.

## How Scribr fits the Education Track
Scribr is a study aid that helps students adjust to a new form of learning and makes education more accessible. It can help international students in various time zones that cannot attend a lecture late at night by providing them a full transcript of the lecture. It saves student's time and allows them to focus on learning as they have a secondary source to review. It helps students who are visual learners by allowing them to re-enforce knowledge by reading lectures. It also helps auditory learners as they can focus on listening to the lecture without worrying about missed details. Scribr can help a student make more detailed, all encompassing, and effective notes.

## Challenges Faced
One of the biggest challenges we faced was implementing the Web Speech API. We were originally planning to make an Electron Desktop App however it took us a long time to realize that Google had disabled the Web Speech API for shell clients and as such we would need to use the Google Cloud Platform's Speech to Text API. While we could have used Google's API, it would make integrating Scribr into digital classrooms much more difficult and expensive. As such, we switched our project over to a Chrome Extension.

Another issue we faced is that, as a direct result of using the Web Speech API, our transcribed text did not have any punctuation marks. While this doesn't seem like a huge issue, we thought it was crucial that the text looked as natural as possible so we utilized the Smart Punctuation API from DeepAffects to add in punctuation using their Natural Language Processor.

## Accomplishments that we are proud of
By injecting a background listener script that ran on specific websites such as Microsoft Teams and Google Hangouts, we were able to expose the native Web Speech API and connect it with our chrome extension
We are proud that we were able to make all the APIs and database storage functions work in unison and asynchronously
Since we used the chrome.storage API, all data is synced across browsers with the Chrome Signin feature
We are also proud that we were able to create such a polished project within such a small time frame. Also, we are happy that we developed a product that solves a real problem, is usable, and can help teachers and students amidst difficult and uncertain times.
What we learned
We learned how to make a chrome extension that could load sophisticated javascript libraries like react and used some new APIs.

## Adding Scribr to Chrome
Download the zip file from our website (LINK) or github (LINK) and extract it.
In chrome, go to “chrome://extensions/” and enable developer mode.
Click “load unpacked” and choose the extracted folder.
You have successfully added Scribr and can now use it!
See the github link attached for more instructions.

## What's next for Scribr
There are many exciting features we hope to add to Scribr such as a deadlines section which shows all the deadlines and due dates mentioned in a lecture and allows you to add it to google calendar. We also plan to get it on the chrome web store so teachers can easily add it to their browser.
