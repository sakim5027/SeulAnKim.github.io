---
layout: post
title: GameCrawler Project Retrospective
subtitle: CodeStates First Project Retrospective
gh-repo: sakim5027/GameCrawler_client
gh-badge: [star, fork, follow]
cover-img: /assets/img/GameCrawlers/GameCrawler_logo2.png
tags: [React, Node.js, AWS(S3), HTML, CSS, Login Modal, Version Control System, Responsive Web Design, Retrospective]
comments: true
---
<br>

## Looking Back the GameCrawler project

  ![MainPage1](../assets/img/GameCrawlers/01. GameCrawler_Main Page_1.png)

This was the first group project I experienced in the CodeStates bootcamp. In this project, I worked with 2 other teammates, and participated as the Front-end web developer. During the 4 weeks, our team worked as a group and went through all the process from the service planning to the website building. Below are the things I felt while going through this first group project.

<br>

### Experience with Git

Since this was my first group project, this was the first time I experienced the **Git** in group settings. During this project, we learned **Version Control System** by creating & managing different branches within git to work on the different features of the project. 

At first, it took us hours and hours in fixing the messed up Git branches, since everyone was inexperienced with the git. But as time went by, we got used to using git in handling the branches, and got into a habit of pulling the upstream before pushing my local branches to upstream. 

Below are some of the git features I used & experienced:

- **git remote add (upstream) (url)** : Add the specific url as the upstream repository
- **git branch** : checking the list of branches I have
- **git branch (branchname)** : create a branch named (branchname)
- **git branch -m (oldbranch) (newbranch)** : change the branch name from (oldbranch) to (newbranch)
- **git branch -d (branchname)** : delete the branch named (branchname)
- **git checkout (branch)** : move to the named branch
- **git checkout -b (branch)** : create a branch and move to the new branch
- **git status** : seeing the status of modified files in the working directory
- **git add (filename)** : add(stage) the file in the working directory to the staging area
- **git add .** : add(stage) all the files in the working directory to the staging area
- **git commit -m '(commit message)'** : create the snapshot of what changes were made to the repository.
- **git pull (upstream) (branch)** : pull from the upstream branch into the local repository
- **git push (origin) (branch)** : push the local branch to the upstream repository

<br>

### Login Modal

  ![LoginModal](../assets/img/GameCrawlers/03. GameCrawler_Login Modal.png)

During this project, I could experience creating a **Login Modal** only using React, without using any outside UI frameworks such as styled components or bootstrap components. It was surprisingly difficult process, and it took me 3 whole days to finish this login modal, even after factoring in the fact that I was working on this project after work.

I had to make 3 different layers - shaded modal layer, container layer and login form layer - and all 3 layers had to work together when login button was onclicked. At first, I tried to make the modal close when user clicks on the shaded area, but there were too many errors when I tried this. So I ended up creating a close button on the top right corner of the container layer, which closes all 3 layers when onclicked.

<br>

### Importance of Teamwork & Communication

During this project, I felt the importance of teamwork and communication in the group project. There were 2 other teammates, a team leader who participated as a Back-end developer and a teammate who participated as a 2nd Front-end developer. Since there were 2 Front-end developers in the team, we formed a smaller Front-end group within the team.

The Front-end group went well, and the communication between me and other Front-end teammate was very smooth. We shared the progress every day through the messenger, and she was very understanding of my situation of being in different time zone (I was in US while the other Front-end teammate was in South Korea, so there were around 14 hours time difference). We found the time we could work together, and helped each other whenever the error or issue came up. This was probably the best teamwork experience I ever had in the group projects.

On the other hand, the communication & teamwork with our team leader, the Back-end developer did not go very well. She had a previous experience of working as a backend developer in the industry, so she was very knowledgeable of what she was doing. However, she also had a coercive attitude towards the teammates. At first, we started as a 4 team members with 2 Back-end developers, but our team leader did not go well with the other Back-end teammate, and he left the project after first week. Even after that, our team leader did not change and pushed other teammates without listening, blamed them for the project being delayed and personally attached other teammates. 

In this circumstances, I tried my best to communicate with the team leader and finish the project, but finally she refused to represent our project to the CodeStates due to the reason 'project has not met all the goals'. I wrapped up all the situation and prepared the project representation instead of our team leader 1 hour before the presentation started.

I understood what she meant, especially considering how goal-oriented she was. However, I still think we could came up with better results if our team leader was a bit more understanding and willing to help teammates, who were far more inexperienced than she was. This was the time I felt the importance of communication and teamwork, since I could experience the two extreme cases within one project and saw how group atmosphere and productivity could change according to this.

<br>

### Pressure of Deadline

In this circumstances, I felt the pressure of deadline more than ever. Among the 4 weeks, we spent around 2 weeks in planning and creating documents such as wireframe, flow charts, DB Schema and API documents. After that we were left with 2 weeks for building website, and since everyone was working on the project after their work, the time availability was far shorter than what we initially thought. 

Also, at the start of the project we distributed the estimated hours in completing each pages, but since everyone was inexperienced, it took us far longer to build each pages. As a result, we could not finish the Game review page and Statistics page, as well as the Game details page. 

Looking back at the project, I think we did not estimate the available time correctly, and ended up planning for the bigger project that what we could finish with given time. If the communication between teammates was better, we could resize the size of the project and get rid of the unnecessary features, but this did not work well. After the project, I felt the importance of knowing what I can do and coming up with correct estimates at the planning stage.


<br>