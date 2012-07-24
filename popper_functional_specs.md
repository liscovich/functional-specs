#Popper Functional Specifications: Researcher Site

The Popper Functional Specs describe the three core components of Popper: (1) The Researcher Site, (2) The Player Site, and (3) The Popper Software Development Kit. These Functional Specs serve to make sure that everyone is on the same page about the functionality and purpose of each of the components of Popper. This document is an organic work in progress and will likely change over time. We will notify everyone as changes are made.

Two types of names are bolded in this document: **Web Pages** for the Researcher Site and Player Site, and **components** of the Popper Software Development Kit. These items are bolded and assigned a consistent name throughout the text. 

#Audience

The Researcher Site serves two types of users: 

1. Social Science researchers from academic institutions
2. Researchers from non-academic institutions

The first category of researchers includes professors, graduate students, and research assistants in the fields of economics, political science, psychology, and sociology. The second, non-academic category of researchers come from a variety of companies and backgrounds, including Microsoft and think tanks. Both sets of researchers attempt to use experiments to better understand and explain human behavior. 

Most of these researchers currently use z-Tree, software from the 1990s that requires researchers to learn how to program. Researchers are accustomed to bare-bones UI for both themselves and their subjects. These researchers typically know a limited amount of programming but are open to technologically complex tools, since much of their work relies on technology such as [STATA](www.stata.com), [z-Tree](http://www.iew.uzh.ch/ztree/index.php), and [R](http://www.r-project.org/).

Users fall into two typical use cases: 

1. The Experiment Designer
2. The Trial Runner

##1. Professor Goldin, the Experiment Designer

Professor Goldin is an economics professor at Carnegie Mellon University. For over ten years, she has used [z-Tree](http://www.iew.uzh.ch/ztree/index.php), the dominant social science experiments software, to study human behavior. She knows a rudimentary amount of programming--just enough to design experiments in z-Tree. Each trial takes several weeks to run, and much of this time is spent handling logistics: recruiting subjects, waiting for subjects, screening subjects, reserving computer lab space at the university's social science experiments facility, and ensuring that subjects are paid. 

Professor Goldin hears about Popper at an Experimental Economics Conference and visits [www.popper.org](www.popper.org). On the **Landing Page**, she reads about how Popper works and signs up for an account. She downloads the Popper SDK and reads through the Popper documentation. The first trial that she runs uses one of the stock experiments available publicly. She makes a few changes to the experiment design in [Unity3D](http://unity3d.com/), which is provided as part of the Popper SDK. Once she finishes designing the experiment to her satisfaction, Professor Goldin asks her research assistant, Robert, to run trials using this experiment. 

Soon, Professor Goldin begins designing her own experiments from scratch using templates from the Popper SDK and assets downloaded from the [Unity Asset Store](http://unity3d.com/unity/asset-store/). Popper takes care of logistical and technical issues so that Professor Goldin can focus on her research rather than tedious overhead. Her trials now take hours, rather than weeks, to run. 

##2. Robert, the Trial Runner

Robert is a research assistant working for the economics department at Carnegie Mellon University. His job this summer is to run trials and crunch data for Professor Goldin. Robert knows no programming but has taken a few statistics courses. Professor Goldin asks him to set up an account at www.popper.org. He signs up on the **Landing Page** and follows a set of simple instructions to create an account. Robert links Professor Goldin's laboratory GitHub account with his Popper account, and is able to find the lab's private experiments on the **Experiments Library** page. He selects one of the experiments and fills in a set of parameters for who is allowed to participate in the trial and the type of data he would like to collect. Robert clicks Create Trial, and eligible subjects are automatically recruited from Amazon MTurk and oDesk. He monitors the progress of the trial on the **Dashboard** page. A few hours later, the trial is complete and Robert downloads the data to analyze further. 

#Landing Page 

The purpose of the **Landing Page** is to convince social science researchers to sign up to use Popper. This sign up process will be discussed later. The **Landing Page** answers the question, "What Is Popper?" and provides reasons that the researcher should try to use Popper in place of their current software. 

The overall look of the **Landing Page** should be classic yet modern. Since the audience ranges from graduate students in their mid-20s to older professors, it is essential that the site does not have a plastic, generically Web-2.0 feel. We are leaning towards a light, clean color scheme. The **Landing Page** must convey academic legitimacy: it is essential that researchers not feel that they are the targets of marketing.

![Image](https://github.com/liscovich/functional-specs/blob/master/images/landingpage.png?raw=true)

The **Landing Page** consists of six components: 

1. Header (including Accounts)
2. Features
3. Sign Up
4. Footer

##1. Header

The Header contains the Logo, Navigation Bar (where we will cover user Accounts), Overview, and Usage Statistics. 

![Image](https://github.com/liscovich/functional-specs/blob/master/images/header.png?raw=true)

###Popper Logo

![Image](https://github.com/liscovich/functional-specs/blob/master/images/lplogo.png?raw=true)

The Popper Logo contains the name "Popper" accompanying a stylized likeness of the philosopher Karl Popper. The ideal portrait for this logo is available [here](http://en.wikipedia.org/wiki/File:Karl_Popper.jpg) in the public domain from Wiki Commons. 

<center>
	<IMG SRC="http://upload.wikimedia.org/wikipedia/commons/4/43/Karl_Popper.jpg" WIDTH="10%" ALT="POPPER_PHOTO" BORDER="2.5">
	</center>

We would like to include Karl Popper's likeness to clarify the origin of the name "Popper" and dissociate the name from drugs or the action of "popping". The logo should be designed to stand out well against both the light background of the Researcher Website and the dark background of Unity3D, a core component of the Popper SDK. 

The font of the logo should be classical and convey both authority and legitimacy, much like the logos of universities and research software.

<center>
	![Image](http://upload.wikimedia.org/wikipedia/commons/9/99/Harvard_University_Logo.PNG)
</center>

<center>
	![Image](http://www.dartmouth.edu/home/files/graphics/dartmouth.gif)
</center>

<center>
	![Image](http://www.utexas.edu/sites/all/themes/webcentral/_images/ribbon.png)
</center>

<center>
	![Image](http://www.wolframalpha.com/images/homepage/wa-logo.png)
</center>

Finally, the logo should have a corresponding smaller "minilogo" that appears in the title bar of web browsers. This minilogo should most likely be a "P" that corresponds stylistically with the Popper logo.

When a user is not signed in, clicking on the Popper Logo brings the user to the landing page at [www.popper.org](www.popper.org). Once the user signs in, clicking on the Popper Logo brings the user to the **Researcher Dashboard**, which will be discussed later.

###Navigation Bar

![Image](https://github.com/liscovich/functional-specs/blob/master/images/lpnav.png?raw=true)

The Navigation Bar in the Header includes four links: 

1. **How It Works**
2. **Our Story**
3. **Experiment Library**
4. *Log in*

[1] **How It Works** links to documentation for Popper. Documentation is stored on GitHub, not on the Popper Researcher Website. Clicking on **How It Works** takes the Researcher to a public repository linked with the official [Popper GitHub account](https://github.com/Experiments/). We will take care of writing documentation.

[2] **Our Story** is a static About page. Its contents will be discussed later.

[3] **Experiment Library** is a dynamic page on the Popper Research Site that allows researchers to browse experiments, and will be discussed later.

[4] User log in and sign up will be described in the "Accounts" section below. 

###Accounts

Popper user accounts pull information from two sources: GitHub and the Popper Researcher Website. Sign up begins with the creation of a GitHub account and log in is accomplished on the GitHub website, which then redirects to the Popper site. As part of the sign up process, the Researcher Website asks for additional credentials and user information relevant to Popper that GitHub does not ask for. All users are required to have a GitHub account, for three reasons. 

1. GitHub frees Popper from having to handle plumbing tasks, like log in and password retrieval. 
2. We would like to encourage users to collaborate on experiments, and GitHub provides a handy framework that encourages users to work together.
3. We would like to minimize the number of additional steps a user needs to take after signing up. Users who design experiments must have a GitHub account to push experiments, but users who only run trials do not need a GitHub account since trials can be handled solely through the website. We anticipate that some users who start out running trials may also run experiments later. Requiring all users to create a GitHub account means that users do not have to jump through an extra set of hoops to set up a GitHub account later if they decide to run experiments; they can get started right away. 

####Sign up

We will first make a brief detour to the Sign Up field on the **Landing Page** to discuss the sign up process, and then go back to the Navigation Bar to take a look at the log in process.  

<!---Landing Page screenshot with Sign Up field highlighted-->

#####Step 1

The Sign Up page consists of three separate steps. We would like to display only one step at a time while showing progress, in the style of the sign up process at [Groupon.com](Groupon.com). All steps should be displayed on the same Sign Up page with the same wrapper. The Groupon method of showing each page of the sign up is not necessarily the best choice for Popper, so the way each step is shown on our site is a design decision that we would like to discuss with Fixel. The point is that each step should be bite-sized and modular, and users should not feel overwhelmed by a long form.

The first part of the Sign Up page verifies the user's email. Most users will actually complete this step on the **Landing Page**. The user enters an email address for verification and clicks Get Started. Text appears below this portion of the page that reads, "Please check your email to verify your account." Here's the text of the email: 
  
> Hello,
> 
> We received a request to create a Popper account for [youremail@university.edu](youremail@university.edu). To verify your account and complete the sign up process, please click [here](some.authenticated.URL.com) or paste the following URL into your browser.
>
> [www.someurlforsignup.com](www.someurlforsignup.com) 
> 
> If you have any questions or believe you received this email in error, please email [support@popper.org](support@popper.org).
> 
> Thanks,
> 
> The Popper Team
 
Clicking the verification link in the email takes the user back to the **Sign Up** page if the user started out on that page, and to the Sign Up page for the first time if the user signed up through the **Landing Page**. After completing email verification, users should be able to know that they have successfully completed this step. Two design decisions have to be made here with Fixel: first, where the message "Your email nash@princeton.edu has been successfully confirmed!" is shown; second, whether the step is grayed out or invisible altogether. 
 
#####Step 2

After verifying an email address, the user is prompted with two buttons, either to log in or sign up using GitHub. GitHub does not allow user log in and sign up to be conducted on an external site, which means that this process has to take place on GitHub and then redirect the user back to the Popper Researcher Website once log in or sign up is done. 

The log in screen is part of GitHub API and looks like the following. 

<!---GitHub log in screen-->
The sign up screen is part of GitHub API as well, and looks like the following. 

<!---GitHub sign up screen-->
After log in or sign up, the user is redirected to a GitHub page to authorize GitHub access to the user's private and public information. This authorization is necessary to customize the user's **Experiment Library** so that the users's own public and private experiments are displayed. The only way to run a trial is through the **Experiment Library**, which means that Popper must be able to access both public and private repositories. Experiments from public repositories are visible to all users, while experiments from private repositories are visible only to users who have GitHub access to that repository. 

<!---GitHub authorization page-->
If the user has already granted Popper access to the user's GitHub account, Step 2 should either be hidden or minimized along with Step 1.

#####Step 3

The user is redirected to the **Sign Up** page after granting GitHub access to Popper in order to provide Popper with a few last pieces of information not available through GitHub: First Name, Last Name, Affiliation, and Department. First and Last Name are required here because GitHub does not ask users to input their first and last names separately, and we want to make sure that we have the full names of all users. Affiliation usually refers to university, but users who are not affiliated with a university should be able to click "Other", which allows them to complete a separate field with their affiliation. We would like users to be able to complete the Affiliation and Department fields using auto-complete. The complete list of all institutions and departments that run economics experiments can be found [here](http://edirc.repec.org/alphabet.html). If possible, we would like to scrape institution and department names somehow, if Brendan thinks this is possible. Manual entry of all institutions and departments into a spreadsheet is possible but would be highly time-consuming: the United States alone has 3,149 institutions, each of which has several departments. 

Finally, by clicking "Submit", the user agrees to the Popper Terms of Service, which we will provide. The Terms of Service should open in a popup window. 

##2. The Hook

The purpose of the Hook is to describe to the user, briefly, exactly what Popper is. We anticipate that initially, most users who come to www.popper.org will know little to nothing about Popper. The most that users might know is that Popper is a tool that lets social scientists run experiments.	

The header of the **Landing Page** is "Behavioral Experiments Platform, [*a(n) adjective*] one". We would like to replace the [*a(n) adjective*] with a revolving list of words, both serious and funny. This header is meant to add character and likeability to the Researcher Site. In terms of execution, we are unsure whether it would be more pleasant from a UX perspective to have the words automatically refresh every few seconds or if it would be better for the user to click a small "refresh" icon next to the [*adjective*] to make the word change.

Here is the list of words -- we would like for the succession of words to be random but the first word that appears when the user arrives on the **Landing Page** should always be a word from the Serious list. 

> **Serious** 
> 
> - an agile
> - a modern
> - a versatile
> - a cutting-edge
> - a customizable
> - an addictive
> - an advanced
> - a promising
> 
> **Funny**
> 
> - a fat-free
> - a low cholesterol
> - a low emissions
> - a PG-13
> - a lactose intolerant
> - a free range
> - a whole wheat
> - a hormone free
> - an antibiotic free
> - a TSA-compliant
> - a pasteurized

Underneath the header is a short paragraph explaining what Popper is. 

> Popper is a powerful blend of modern technology and social science. Using Popper, you can design complex cutting-edge experiments using the most advanced tools in existence. You can also run large-scale online trials drawing subjects from the world's deepest on-demand subject pool.

##3. Statistics

We would like to include usage statistics to boost the legitimacy of Popper among researchers. This portion of the **Landing Page** should be located directly under the Hook. Three statistics should be dynamically displayed and updated: the number of researchers, the number of deployed experiments, and the number of completed trials. The focus is on the numbers, which means that these digits should stand out much more than the names of what the numbers are counting. These statistics will only be available once Popper gains traction, which means that it would be ideal for there to be a way for us to activate this section of the site only once we have compelling statistics to show. This means that the **Landing Page** should visually "work" even if the statistics portion of the page is not shown. 

##4. The Features List

After the user gets some sense of what Popper is, the Features List provides a more detailed explanation of why the user should make the decision to Sign Up. The Features List describes four core selling points of Popper:

1. Start at the Frontier

2. Program the Way You Think

3. Run When You Are Ready

4. Leave Logistics to Us

These four features should be arranged on a horizontal navigation panel. Each of the four phrases should be accompanied by an image, which we will provide. Underneath the navigation panel is a frame split in half horizontally, with text in the left panel and an image in the right panel. As the user clicks on each of the four features, the contents of the frame change. We are currently deciding on the four sets of text and images to place into this frame. The following text is a draft of what we would like to include in the frame. 

###Start at the frontier

Begin running experiments right away. Browse the Experiment Library to find the best existing experiments. Share, discuss, and collaborate on best-practice experiment design effortlessly with a community of professionals. Retrieve the entire experiment protocol for any publicly available experiment 24/7 from our servers. Best of all, replicating an experiment only requires three clicks. 

Popper relies on frontier technology, which means that it improves daily. 

### Program the Way You Think
 
Design experiments using intuitive visual programming. Popper comes equipped with domain-specific nodes, custom-tailored for behavioral experiments. Easily automate common experiment tasks using one of our templates. Popper features full Mathematica support for computationally-intensive functionality. Those with more programming experience can delve past visual programming into the C# code underlying all experiments. 

### Run When You Are Ready

Draw from our on-demand online subject pool. Without the physical restraints of a lab, subjects can participate from the comfort of their homes, when you need them to. Deploy experiments in minutes, without worrying about searching and coordinating eligible subjects. 

### Leave Logistics to Us

Popper is built on a secure cloud infrastructure of servers, which means that you can focus on science rather than logistics. We handle all technical overhead related to subjects, from recruitment to screening to payment. We also provide an archive of IRB experiment-specific approvals for your convenience to expedite your own IRB approval process. 

##5. Sign Up

<!---extracted; fix-->

##6. Footer

The Popper footer contains links, and is divided into two components: general links and legal miscellaney. The general links are divided into three vertical columns. The first column, "Popper", includes links to "Our Story", "Blog", and "Contact". The second and third columns include links to Documentation. We have not yet fleshed out the Documentation of Popper enough to know how many distinct links this section will include. 

The second half of the footer is comprised of links that run horizontally along the bottom of the page. These links are "Terms of Service", "Privacy", and "Security". Under these links is the text "(c) 2012 Popper. All Rights Reserved." On the right side of this part of the footer is the Fixel logo, with the text "Designed by Fixel".

#Our Story

The **Our Story** page functions as an About page. It explains who Karl Popper is and introduces the Popper team.

**Our Story** features the same Header and Footer as the **Landing Page**. On the left is a photo of Karl Popper taken by Lucinda Douglas-Menzies. This photo should be cropped as necessary to work with the overall design of the page. We were able to secure rights to use this photo, provided we give credit to the photographer. Under the cropped photo should be the text, "(c) Lucinda Douglas-Menzies" and "Reproduced with the generous permission of the photographer". 

To the right of Karl Popper's likeness, we would like to include a section called "Behind the Name" and, beneath it, "Team". We are currently working on this text and will provide it once it is ready. For now, we anticipate that the text in each section will not be more than two paragraphs long. 

We would like the other static pages on the Researcher site to feature the same wrapper as **Our Story**. These other pages are **Contact**, **Terms of Service**, **Privacy**, and **Security**. 

**Sign Up** features the same Header and Footer as the **Landing Page** and **Our Story**.

#Experiment Library

**Experiment Library** is the final page accessible to non-signed in users from the **Landing Page**. The page includes a few additional features once a user has signed in. These differences will be noted below when relevant.

There are five main features in **Experiment Library**:

1. List of experiments
2. Search bar
3. Filter
4. GitHub authentication link
5. Header and Footer

##1. List of experiments

The main feature of **Experiment Library** is a list of public experiments. All users can see this list, no matter if they are logged in or not. The idea is to allow researchers to be able to see what Popper offers without having to sign up first. The list of experiments is an embedded frame with a scrollbar. We would like to display three experiments per row.

Three types of experiments are thus displayable in this frame: Private Experiments, Public Experiments, and Stock Experiments. These three sections are always displayed in this order. From a GitHub perspective, Private Experiments are user-specific and are drawn from the private repositories that the user links with her Popper account. Public Experiments are drawn from users' public repositories that are linked with a Popper account. Finally, Stock Experiments are drawn from public repositories in the Popper GitHub account. Each of these three types of experiments serve a slightly different purpose. Private Experiments allow researchers to run trials without having to reveal their experiment protocol before they are ready. Public Experiments allow researchers to open their work to their peers for review and replication if necessary, usually after the original researcher has already run the experiment and published results. Stock Experiments are provided by Popper and allow the very first users of the platform to begin running trials right away. They also show researchers the functionality of Popper, and serve as a template for researchers to use as they begin to design their own experiments. The Stock Experiments that Popper provides on the Researcher Website incorporate common games that researchers frequently test in the lab.

Accordingly, the List of experiments should be divided into three sections separating Private Experiments, Public Experiments, and Stock Experiments. 

The content of this frame is pulled from GitHub and sorted by date--repositories with the most recent changes will be displayed first. *Users who are signed in and who have linked their GitHub account with their Popper account will see experiments from their private repositories displayed first in the list, rather than public experiments. Next displayed will be Public Experiments, with their own experiments displayed at the top of the list. Last are Stock Experiments.* Each experiment is accompanied by a metadata, which is pulled from GitHub. The name of the repository (functioning as the name of the experiment), a description of the experiment, number of forks, and the academic journal in which the results of the experiment were published should be listed. The number of forks is necessary to list and include in the metadata because researchers may want to sort experiments by popularity, which is functionality we would like to include in the future once more experiments are available in **Experiments Library**. We anticipate that almost all public experiments in **Experiment Library** will be accompanied by a journal in which results were published. This is because we expect that researchers will not make their experiment repository public until they have published results, at which point it is good academic practice to make the experiment publicly available should peers wish to replicate the experiment.  

When a researcher hovers over an experiment, the color of the square containing the name of the experiment and its information should change color. Clicking on the experiment brings the user to the **Create Trial** page for that particular experiment, which will be discussed later. 

##2. Search bar

The search bar sifts through the contents of the List of experiments. As soon as a researcher begins to type, autocomplete suggestions should appear beneath the Search bar, in the style of Google search. When a researcher clicks on an experiment in the autocomplete list, that single experiment alone is displayed in the List of experiments. If the researcher instead hits Enter, a list of all experiments relevant to the search phrase will appear in the List of experiments, split up into the three sections mentioned above (Private Experiments, Public Experiments, and Stock Experiments). 

Autocomplete search results should be formatted as follows:

> **Name of Experiment** - Description of experiment, truncated after a certain number of characters so that the number of forks and publication journal can appear at the end of the autocomplete suggestion... - *Forks: ##; Journal Name*

##3. Filter

Researchers can click on one of five filters to find experiments. The number of filters may increase in the future, so there should be a way of adding filters as necessary. For now, the five filters for experiments are:

- All
- Social Preferences
- Networks
- Coordination Games
- Cheap Talk Games

When a user clicks on one of these filters, the filter opens up and the list of available experiments that fall under this filter are displayed in the filter navigation bar. The format of the filtered result is as follows:

>**Name of Experiment** (number of forks)

At the same time, the frame to the right of the Filter should update if necessary to be populated with all experiments that match that filter, organized by section (Private Experiments, Public Experiments, and Stock Experiments). If a user selects an experiment in the Filter, that experiment should be highlighted in the Filter and the Experiment List frame should update to display only that experiment, as well as the section that the experiment falls under (Private Experiments, Public Experiments, and Stock Experiments). Similarly, if a user selects an experiment in the Experiments List frame, this experiment should be highlighted in the Filter and the Filter should collect/collapse as necessary to open up the filter that contains the experiment. 

##4. GitHub authentication link

Users who are not logged in see the following text under the Experiments List: "To add external experiments, [Log In](linktologintopopper.com)". Clicking on Log In opens the same ajax popup window described for the **Landing Page**. 

Users who are logged in see the following text instead: "To add external experiments, [sign-in with GitHub](signinwithgithub.com)". Clicking on the link opens an ajax popup that allows a user to link her Popper account with her GitHub account. Doing so allows the user to view her Private and Public Experiments in the List of Experiments. 

The window contains five elements: a title, "Sign In with GitHub"; GitHub username; GitHub password; a "Forgot your GitHub password?" link; a button, "Submit". Clicking Submit sends a call to GitHub's API and links the user's Popper account with the GitHub account so that all public repositories are sent to the List of Experiments under Public Experiments and all private repositories are sent to the List of Experiments under Private Experiments (which are viewable by the user who owns the linked account). 

After clicking Submit, the ajax window disappears and the user sees an updated version of **Experiment Library** with additions to the List of Experiments as applicable. 

If the user enters an invalid username and/or password, the ajax window shakes from left to right and the message "Invalid user name or password" is displayed at the top of the popup, between "Sign In with GitHub" and the "GitHub username" field. If the user clicks on "Forgot your GitHub password?", a new tab opens to https://github.com/sessions/forgot_password and the user completes the password retrieval process through the GitHub website.

##5. Header and Footer

The Header of **Experiment Library** is identical to the Header found on the **Landing Page**, except for two main differences. First, the link "Our Story" is replaced by a link to **Dashboard**. Second, the user sees something different in the top navigation bar depending on whether the user is logged in. A logged-in user will see the email address of the logged-in account with a down-cursor. Clicking on the down-cursor displays the following options: Dashboard, Profile, Log Out. **Dashboard** and **Profile** are separate pages and will be described later. Log Off signs the user off Popper and brings the user back to the **Landing Page**. A message telling the user that Log Out has been completed is *not* necessary.

The Footer of **Experiment Library** is exactly the same as the Footer described on the **Landing Page**. 

#Dashboard

Researchers monitor trials in the **Dashboard**. The **Dashboard** consists of two main components: 

1. Trials
2. Feed

##1. Trials

Trials is a list of all of the researcher's trials, both complete and ongoing. A trial enters this list as soon as a researcher clicks "Create Trial" on the **Create Trial** page, which will be discussed later. Clicking on the name of a trial brings the researcher to the **Monitor Trial** page for that trial, which includes all parameters and actions specific to a particular trial. This page will be discussed later.  

Trials are sorted by activity date, which means that the most recently active trials appear at the top of the list. Trials can be in one of five statuses, and a change in status consitutes "activity" that pushes a trial to the top of the list. These statuses are displayed underneath the name of the trial, as shown in the wireframe. The five statuses are:

1. Awaiting players: The initial status of all trials that a researcher creates is "Waiting for players". This status indicates that the trial has been created and that the server is waiting for a sufficient number of subjects to join the game. The researcher can click on the name of the trial to go to that trial's **Monitor Trial** page to recruit more subjects if necessary. 
2. In progress: Once enough subjects have joined a trial, the status of the trial changes to "In progress". Subjects play the game, and as they do, data from the experiment is sent to the **Monitor Trials** page.
3. Pay subjects: Once a trial is complete, the researcher pays subjects. The researcher can review and approve subject payments from the **Monitor Trial** page.
4. Complete: After payment is complete, the status of the trial changes to "Complete". No further action is required from the researcher at this time, but the trial is saved in the List for the researcher to review and download data. 
5. Error: If there is an error with any part of the trial, the researcher can click on the trial to go to **Monitor Trial** in order to fix the error.

In addition to the status of the trial, two other pieces of information about the trial are displayed next to the name of the trial. 

- Trial number: Each trial is assigned a unique ID number. This number is necessary to keep track of trials and allows us to help users resolve issues with individual trials.
- Date and time: A timestamp corresponding with when the change in status occurred is displayed next to the name of the trial. These time stamps are important and informative for each status. For example, when a trial is first created, the time stamp in "Trial" would indicate when the trial was first created.

At the bottom of the Trials frame is a button for "More...", in the style of GitHub. Clicking this button scrolls the entire window down to display more trials. This button disappears once the researcher has displayed all existing trials. There is no scroll bar on the Trials frame itself.

At the top of the Trials frame is a button, "New Trial". Clicking this button takes the researcher to the **Create Trial** page.

##2. Feed

The Feed is on the right side of **Dashboard**. This feed automatically updates with the following information regarding changes in status and other types of activities:

- Changes in status, with the following phrasing:
	- Awaiting players: "**Trial ##** has been created. Awaiting players." As each player joins, the following message is displayed in the Feed: "**Player ##** has joined **Trial ##**."
	- In progress: "**Trial ##**" is now in progress.
	- Pay subjects: "**Trial ##** has finished. Go to the **Monitor Trial** page to review subject payments."
	- Complete: "**Trial ##** is now complete."
- Fork activity
	- "Researcher ## has just forked your experiment, **Experiment Name**."
- Following activity
	- "**Researcher ##** is now following **Trial ##**."
	- "You are now following **Trial ##** by **Researcher ##**."

Each bolded item in the above bulleted list should be a link that opens in a new tab. **Trial ##** links to the **Monitor Trial** page for a particular trial. **Player ##** links to a player profile, which is hosted externally on the Player Website. **Researcher ##** links to the public profile view of another researcher; this profile is hosted on the Researcher Website.

Just as with the Trials frame, a "More..." button below the Feed frame scrolls down the entire window and allows the researcher to see more feed information.

The Header and Footer of **Dashboard** are identical to the signed-in view in **Experiment Library**.