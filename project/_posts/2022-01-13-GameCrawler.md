---
layout: post
title: GameCrawler
subtitle: Codestates First Project (4 Weeks / 3 Team Members)
gh-repo: sakim5027/sakim5027.github.io
gh-badge: [star, fork, follow]
cover-img: /assets/img/GameCrawlers/GameCrawler_logo2.png
tags: [React, Node.js, AWS(S3), HTML, CSS, Login Modal, Duplicate Check, Validation Check, Responsive Web Design]
comments: true
---

## Introduction

In this 4-week project, I worked as a team of 3 members in creating a website where users can search for Game Information & write reviews. I particiapted as a **Front-end** team member, and we used below stacks.

**[ Stacks Used ]**   React, Node.js, AWS(S3), HTML, CSS

<br>

## Index
1) Project Planning
- Project Goals
- Team Rules
- Wireframe
- Flow Chart
- DB Schema
- API Document

2) Final Website & Features
- Main Page
- Game List Filtering
- Login Modal
- ID & Password Search
- Sign Up Page
- MyPage
- Responsive Web Design

3) Retrospective

<br>

## 1) Project Planning

In the project planning process, we created below documents and rules:

- Project Goals
- Team Rules
- Wireframe
- Flow Chart
- DB Schema
- API Document

<br>

### 1-1) Project Goals

While setting the project goals, we divided the goals into 3 different levels according to difficulty and importance. If you want to know what goals we could achieve or not, please see **Retrospective** at the end of this post.

**[ Bare minimum ]**
- Login / Logout / Sign Up / Duplicate ID Check / Sign Out
- Social Login using OAuth
- Mypage
- Edit User Information
- Game Filtering Feature (home)
- Game Detail Page
- Review List CRUD

**[ Advanced ]**
- Favorite List CRUD
- Statistics for Favorite Genre / Games

**[ Nightmare ]**
- Rolling Banner for New Games (Home)

<br>

### 1-2) Team Rules

Before working on the project, we also set the Team Rules to follow during the project. This includes the general rule in teamwork, as well as the basic rules in project settings.

**[ General Rules ]**
1. All team meetings will be held through Google Hangout
2. Share the issues rightaway when they come up
3. Don't be mad at team members for being inexperienced / bad
4. Write comments on the details about the code you wrote (for the review purpose)
5. Update the weekly progress in the Discord Chat Room on Monday
6. Share the information in Discord Chat Room if you made PR or updated the Wiki
7. Share the information in Discord Chat Room if any of the plans needs to be modified

**[ PR Form ]**
[Server/Client] Issue number/Issue title

**[ Commit message Form ]**
Issue Number/Issue title/feature details created or modified

**[ Branch Name Form ]**
feature_issue number

**[ Variable Name Form ]**
camelCase/ if related to DB, table name + column name

**[ File & Constructor Name Form ]**
Name it according to the page name

**[ ES-lint Setting ]**
no-unused-vars : warning



<br>

### 1-3) Wire Frame

1. Header

      ![Header](../assets/img/GameCrawlers/WireFrame/01. Header.png)

2. Footer

      ![Footer](../assets/img/GameCrawlers/WireFrame/02. Footer.png)

3. Sign Up Page

      ![SignUp](../assets/img/GameCrawlers/WireFrame/03. Sign Up.png)

4. MyPage

      ![MyPage](../assets/img/GameCrawlers/WireFrame/04. MyPage.png)

5. Update User Info Page

      ![UpdateInfo](../assets/img/GameCrawlers/WireFrame/05. Update User Info.png)

6. Home Page

      ![Home](../assets/img/GameCrawlers/WireFrame/06. Home.png)

7. Game Details Page

      ![GameDetails](../assets/img/GameCrawlers/WireFrame/07. Game Details.png)

8. Favorites Page

      ![Favorites](../assets/img/GameCrawlers/WireFrame/08. Favorites.png)

9. Review Page

      ![ReviewList](../assets/img/GameCrawlers/WireFrame/09. Review List.png)

10. Write Reviews Page

      ![WriteReview](../assets/img/GameCrawlers/WireFrame/10. Write Reviews.png)

11. Statistics

      ![Statistics](../assets/img/GameCrawlers/WireFrame/11. Statistics.png)


<br>

### 1-4) Flow Chart

![FlowChart](../assets/img/GameCrawlers/FlowChart/FlowChart.png)



<br>

### 1-5) DB Schema

![DBSchema](../assets/img/GameCrawlers/DBSchema/DB Schema.png)



<br>

### 1-6) API Document

* [API Document](https://github.com/sakim5027/sakim5027.github.io/blob/master/assets/document/Game%20Crawler_API.pdf "https://github.com/sakim5027/sakim5027.github.io/blob/master/assets/document/Game%20Crawler_API.pdf")



<br>

## 2) Final Website & Features

Below are the fianl website we created and the main features.

- Main Page
- Game List Filtering
- Login Modal
- ID & Password Search
- Sign Up Page
- MyPage
- Responsive Web Design


<br>

### 2-1) Main Page

  ![MainPage1](../assets/img/GameCrawlers/01. GameCrawler_Main Page_1.png)

This is the **Landing Page** of our website. In the header, there is logo and the website name (Game Crawler), along with the Review page, Statistics page and Login button. The main page shows all the games list with their poster image, and each image has the favorite button (heart shape) on it. The footer has our website name and contact information. 

Once we log in, the page changes as below:

  ![MainPage2](../assets/img/GameCrawlers/01. GameCrawler_Main Page_2.png)

The main thing that changes once you log in is the Login button on the top right corner. The login button now changes to the Logout button, and a new button for the Mypage shows up.

<br>

### 2-2) Game List Filtering

  ![GenreSelection](../assets/img/GameCrawlers/02. GameCrawler_Genre.png)

In the Main Page, there is a radio button for the **genre selection**. If specific genre is selected, the games in the main page filters and shows the games in that specific genre. Also, you can type in the name of the game in the **search bar**, and it will also filter and shows up the game you are looking for.

<br>

### 2-3) Login Modal

  ![LoginModal](../assets/img/GameCrawlers/03. GameCrawler_Login Modal.png)

If you click on the Login button, the **Login Modal** pops up and the previous page is shaded. In this page, you can login using your ID and Password. If you do not have a ID, you can sign up by clicking on the Sign Up button, and if you forgot your ID or Password, you can search for your ID or password as well. There is also Google Login button (O-Auth Login) which allows you to sign up using your existing google email.

<br>

### 2-4) ID & Password Search

  ![IdPwSearch](../assets/img/GameCrawlers/07. GameCrawler_Id&Pw Search.png)

If you click onto the **Find your ID / Password** button in the Login Modal, you will be directed to the **ID & Password Search** page. In this page, you can find your ID using your registered email, or find your password using your ID and email. All information will be sent to the registered email, and you can check your lost ID or password in your email.

<br>

### 2-5) Sign Up Page

  ![SignUp](../assets/img/GameCrawlers/05. GameCrawler_Sign Up.png)

If you click onto the **Sign Up** button in the Login Modal, you will be directed to the **Sign Up Page**. In this page, you can create a new ID, password, nickname and register your email associated with the ID. Also, you get to choose your favorite game genre.

When creating the ID and password, you need to go through the **validation check**. Your ID needs to be between 4-12 letters including Capitals & numbers, and it should also pass the **duplicate check**. Your password, in other hand, needs to be between 6-12 letters including Capitals & numbers, and the same password needs to be entered twice. This process is shown in below gif image:

  ![IdPwCheck](../assets/img/GameCrawlers/06. GameCrawler_Id&Pw Check.gif) 

In this image, you can see that the web does the validation check and shows the appropriate alert messages below the input box as you enter the ID & password.


<br>

### 2-6) MyPage

  ![MyPage](../assets/img/GameCrawlers/04. GameCrawler_MyPage_2.png)

Once you successfully created your new ID, you will be directed to **MyPage**. In this page, you can see your user information, such as nickname, email and favorite genre. If you wrote any game reviews in the past, it will also be show up in this page uner **My Reviews**. 


  ![MyPageUpdate](../assets/img/GameCrawlers/04-1. GameCrawler_MyPage Update.png)

If you want to update your user information, you can click onto the update button and it will direct you to the **User Info Update** page. In this page, you can change your nickname, password, favorite genre or associated email. When you are changing the password, you will have to go through the **validation check** again, and the same password needs to be entered twice as well.


<br>

### 2-7) Responsive Web Design

  ![ResponsiveWeb1](../assets/img/GameCrawlers/08. GameCrawler_Responsive Web Design_1.gif)

While creating the Game Crawler website, we could successfully implement the **Responsive Web Design** using the media query in CSS. As you can see from the above gif image, the game list in the landing page re-arranges as the page gets smaller.


  ![ResponsiveWeb2](../assets/img/GameCrawlers/08. GameCrawler_Responsive Web Design_2.gif)

When the screen is small, the navigation bar menus ultimately becomes an icon on the top right corner. In this mode, you can click onto the icon and it will show up the navigation bar menus in the drop-down. The drop-down menu works the same as it was in the wide view, and you can see it directs to the correct page as intented.



<br>

## 3) Retrospective

With lack of time, we could not finish all the goals we initially set at the start of the project. (For example, review page and statistic page could not be completed until the project deadline.) However, I am glad I could come up with my first website that actually works with basic features. For the detailed retrospective, please see my blog post **Game Crawler Project Retrospective**. 