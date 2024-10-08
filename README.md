# GitHub Copilot (Beta) Exam preparation


>[!CAUTION]
> #### BETA EXAM 
> I made this in order to prepare for the GitHub Copilot Beta exam I had the chance to participate in. Which obviously means there is no guarantee on anything. I added topics afterwards which were asked in the exam and I did not cover in my preparation material before just to be save if I did not make it and have to retake the exam when it goes live.

>[!WARNING]
> #### Keeping up-to-date/Contribution
> In case I passed the exam I obviously will not update this repository. Pull requests for corrections and updates are of course welcome.

>[!IMPORTANT]
> #### Important note
> Besides the Quiz with the name Quiz GitHub Copilot MS Learn, which was taken from the Microsoft learn modul related to GitHub Copilot all Quizes are AI generated. In my studies i noticed on or 2 questions beeing of I hope i corrected them 

# Intro:
As I took the GitHub Copilot Exam which required me to prepare on my own as no dedicated material like study guides were available I created my own using [Obsidian](https://obsidian.md/)
Which is my general purpose knowledge management system. I extracted this part for people that might be interested and made sure that the information part of the material is accessible as PDF’s. Also a brief description is included how to use the Obsidian vault part of this repository and it’s more advanced features.

# Contents Overview:
There are 2 folders basically containing everything.
## ObsidianVault
This folder contains everything needed for advanced usage with Obsidian. The .md (Markdown files) can of course be viewed directly within GitHub. The quizzes and flashcards have a format which is not supported as they are used by Obsidian plugins and might look weired on GitHub.
## pdfs
Contains PDF’s I have generated out of the study material.
## Files
I will not mention the extensions. If using the pdfs it will be .pdf. If using Obsidian or reading directly on GitHub it will be .md. Obviously.

| filename                                    | mode  | description                                                                                   |
| ------------------------------------------- | ----- | --------------------------------------------------------------------------------------------- |
| 01 - GitHub Copilot Exam Prep               | Basic | Contents of the exam and reference to used material and sites                                 |
| 02 - GitHub Copilot Writeup                 | Basic | General writeup on GitHub Copilot focuses on plans, general concepts and so on.               |
| 03 - GitHub Copilot MS Learn Q&A            | Basic | Extraction of the questions of MS Learn Modul about GitHub Copilot                            |
| 04 - Plans and Features                     | Basic | Sum up and overview of GitHub Copilot plans and corresponding features                        |
| 05 - Features Details                       | Basic | Detailed write ups on features                                                                |
| 06 - Features sum up                        | Basic | Brief summaries on features                                                                   |
| 07 - Additional Stuff                       | Basic | general AI concepts and possible clarifications                                               |
| 08 - Post Beta Exam research                | Basic | Research I did after completing the exam on topics I missed in my initial research            |
| 09 - Post Beta Exam notes                   | Basic | General notes and tips about the (beta) exam                                                  |
| Flashcards Features                         | Pro   | Flashcards I used to learn for spaced repetition learning on features                         |
| Quiz GitHub Copilot AI Generated Run 1      | Pro   | AI generated Quiz on the material first try.                                                  |
| Quiz GitHub Copilot AI Generated Run 2      | Pro   | AI generated Quiz on the material second try.                                                 |
| Quiz GitHub Copilot AI Generated Run 3      | Pro   | AI generated Quiz on the material third try.                                                  |
| Quiz GitHub Copilot MS Learn                | Pro   | Manually created Quiz based on questions and answers of the GitHub Copilot Modul on MS Learn. |
| Quiz GitHub Copliot AI Generated Features 1 | Pro   | AI generated Quiz focused on the features part first try.                                     |
| Quiz GitHub Copliot AI Generated Features 2 | Pro   | AI generated Quiz focused on the features part second try.                                    |

# Usage
## Basic:
Go to the pdfs directory have a look at the material in your preferred pdf viewing tool.
## Pro:
This section explains how to get this working within Obsidian and use the existing Quizzes and Flashcards.
### cloning the repository
Make sure to have GIT installed otherwise install it from [GIT](https://git-scm.com/downloads)
After that go to the directory in which you want to clone the repository in the command line and issue this command:
```
git clone https://github.com/AvaMZAT/GitHubCopilotExamPrep.git
```
All of the repository should now be on your machine.
### Setting up Obsidian
Go to [https://obsidian.md/](https://obsidian.md/) and Download Obsidian for your preferred OS before 

### basic obsidian usage
Launch Obsidian and on this start screen click the open button and select the main directory of the repository you just cloned.
![Image Alt Text](./images/20240816185635.png)

Now in Obsidian the Vault should be opened an in the left hand tree view you should have all the elements of the repository like this:
![Image Alt Text](./images/20240816185609.png)

### use flashcards
You want to use flashcards for spaced repetition? On the left side in the toolbar there is a “Review Flashcards” button. Now double click on the “features” entry in the spaced repetition screen and the flashcards exercise will begin:
![Image Alt Text](./images/20240816190652.png)


![Image Alt Text](./images/20240816190811.png)
Interested in details on the space repetition? Find them here: [Spaced Repetitions plugin GitHub](https://github.com/st3v3nmw/obsidian-spaced-repetition)
### use quizzes
All quizzes available in the vault are mentioned in the list above and also are recognized by the question mark icons on the pages left. To start a quiz right click on the Quiz you want to start and select “Open quiz from this note” => here we go

![Image Alt Text](./images/20240816191226.png)

## H4ckz0r 3l1t3:
This section explains when using Obsidian how to generate your own Quizzes using AI and get your own flashcards

### Create more flashcard sets
1. To create further flashcard sets you have to create a new note:
![ALT image](images/20240818215250.png)
2. in the new note it is important to create a correct tag at the beginning of the new note:
```
#flashcards/GitHubCopilot/MyNewFlashcards
```
3. create your new flashcards with the following syntax:
```
Frontside text 1 (aka questions)
?
Backside text 1 (aka answer)

Frontside text 2 (aka questions)
?
Backside text 2 (aka answer)
``` 
>[!tip] 
>More infos about the spaced repetition plugin can be found here: 
>https://github.com/st3v3nmw/obsidian-spaced-repetition

### Setup OpenAI for quiz engine
The quiz generator is based on OpenAPI for creation of questions based on content. The Quiz generator plugin is already included in this vault. The only thing you have to do is to set your own OpenAI API Key in the plugin settings:
1. Go to vault settings:
![Alt Image Text](./images/20240818220530.png)
2. Go to quiz generator community plugin settings:
![Alt Image Text](./images/20240818220653.png)
3. Insert your own OpenAI API Key:
![Alt Image Text](./images/20240818220800.png)

>[!tip]
>More infos about the quiz generator can be found here:
>https://github.com/ECuiDev/obsidian-quiz-generator

### Generate new quizzes and parameters
1. Configure question types:
	![Alt Image Text](./images/20240818221117.png)
	Personally I did not have good experience with anything besides the Multiple choice questions.
	
2. Generate new questions:
	- Klick the generator icon in the left hand menu: 
	![Alt Image Text](./images/20240818221329.png)
	- Add notes from which the quiz should be generated:
	![Alt Image Text](./images/20240818221658.png)
	- Selected the notes 
	![Alt Image Text](./images/20240818221902.png)
	- Now klick the generate button and enjoy your new quiz
	![Alt Image Text](./images/20240818222103.png)
	