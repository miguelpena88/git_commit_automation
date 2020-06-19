**Github Commit Autommation**

In this project I will be building a tool that automatically makes daily GitHub commits using Python. The frequency of commits per day will follow a random number sequence from 1-10. All the notebooks and files I used for this project are available in this repository.

My approach to tackeling this project began by separating it into two main parts:

1. Automate edits to update a notebook--this is needed before making any github commit

2. Automate the command line instructions that will be coming from script

*This project is still a work in progress and I will be updating this notebooks as I move forward with any revisions*

**Background**

The idea for this project came out of necisity. As a data scientist searching for a job in the current job market, I could not spare to have my github contributions calendar overlooked by non-technical recruiters for having some areas of grey, or days of no commits; thus I made this project to boost my current github activity. 

**Script to command-line**

I began my project by using the Python subprocess module to send instructions to the command line from my notebook. After testing out several use cases, I saved each instruction to a variable--following the required steps to making a github commit from the Terminal command line: "git add", "git commit", and "git push"

![github-small](https://raw.githubusercontent.com/rohit120582sharma/Documentation/master/images/git.png)

After testing out each command individually, I created a function that intakes a notebook name and outputs an "up-to-date" message when the commit has been compleated--the current branch is up-to-date with origin/master. 

**Automating notebook edits**
 
Now that I have created a function that commits any notebook within the current project folder, I went on to create a new notebook that would edit itself. Like I mentioned earlier, an edit must be made to a notebook before it's ready to be commited. So I decided to catalogue each time a commit is made during a single day into dictionary that would ultimatly be saved/updated into an excel sheet.


**Current version**

The current version of this project is meant be run at the beginning of each day to give ample time for proper commit dispersal.

I plan on adding to this project and to its possible use cases. Feel free to reach out with any questions or suggestions! :)
