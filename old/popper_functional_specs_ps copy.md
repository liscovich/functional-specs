# <a name="Introduction" id="anchor4">Introduction</a> 

**Popper** is a behavioral experiments platform that empowers researchers in economics, psychology, sociology, and political science to create and conduct complex large-scale online experiments. 

## Role of experiments in the social sciences

 Social scientists are interested in studying human behavior. They develop theories to explain this behavior and conduct controlled experiments to test these theories. In order for a theory to be "testable", it must produce predictions (hypotheses) about human behavior that can, in principle, be proven wrong. Thus, the process of experimentation results in the falsification of inaccurate theories. 

## Classical experiments

Conducting controlled experiments in the social sciences is difficult. Unlike natural scientists, who often conduct their experiments with inanimate objects, social scientists experiment exclusively with live human beings. Human subjects cannot be forced to participate in experiments and can also quit an ongoing experimental trial at any point. For these reasons, researchers must pay human subjects to convince them to participate in and complete a trial. These trials are typically run in physical laboratories, where invited volunteer subjects engage in simple decision tasks for $15-25/hour--and sometimes more depending on their performance. 

This approach has three serious limitations: 

1. It is very expensive, requiring an equipped brick-and-mortar laboratory and significant subject payments that often exceed $500-1000 per trial. 

2. It is time-consuming and requires recruiting local human subjects more than a week in advance of the trial. 

3. Local subject pools are relatively small, so large-scale trials require using laboratories in multiple geographical locations.

In addition, the software used in physical labs to create and conduct experiments is very outdated. The most popular package, [z-Tree](http://www.iew.uzh.ch/ztree/index.php), was created in the University of Zurich in the late 1990s and hasn't been updated since then.

## Online experiments

In the last 2-3 years, researchers have started conducting experiments online, using subjects from various online labor markets, most notably [Amazon Mechanical Turk](http://mturk.com). This move has radically expanded the size of the available subject pool and decreased subject payments. Now, experimental subjects can participate in trials from the comfort of their own home rather than coming to a physical lab.

However, the move to online trials introduces several new challenges:

1. **Lack of software.** Most online trials have so far been technologically limited to survey-style tasks that do not involve realtime interaction between subjects. The researchers who do conduct multiplayer studies have had to write from scratch their own ad hoc software. No reusable framework capable of supporting multiplayer online trials is currently available on the market.

2. **Low comprehension rates of written instructions.** Online subjects frequently skim, or even ignore, written experimental instructions.

3. **High subject attrition rates.** Online subjects can quit a trial simply by closing a browser tab, with few consequences. This leads to very high attrition rates, especially in trials where subjects become bored. Even though subjects in a physical lab are also allowed to quit the trial at any moment, doing so usually involves an uncomfortable interaction with the researcher. 

4. **Lower degree of control over the experimental conditions.** Subjects can communicate with each other, collude, and cheat in other ways that undermine the [internal validity](http://en.wikipedia.org/wiki/Internal_validity) of the experiment.

## Popper

The goal of Popper is to address the above four problems. It seeks to streamline the process of creating complex and visually compelling multiplayer experiments. Through Popper, researchers will use professional game development tools, which include visual scripting and an extensive library of template game assets. Popper will also provide researchers with extensive subject monitoring capabilites to minimize the possibility of cheating and other runtime irregularities.

#Popper Functional Specifications: Researcher Site

Popper consists of three components: 

1. The Researcher Site
2. The Player Site
3. The Popper Software Development Kit

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

#Accounts

We will first discuss user sign up and log in to clarify what user accounts look like, since these accounts are the backbone of the Researcher Website. After accounts, we will take a detailed look at each of pages on the Popper Researcher Website. 

Popper user accounts pull information from two sources: GitHub and the Popper Researcher Website. Sign up begins with the creation of a GitHub account and log in is accomplished on the GitHub website, which then redirects to the Popper site. As part of the sign up process, the Researcher Website asks for additional credentials and user information relevant to Popper that GitHub does not ask for. All users are required to have a GitHub account, for three reasons. 

1. GitHub frees Popper from having to handle plumbing tasks, like log in and password retrieval. 
2. We would like to encourage users to collaborate on experiments, and GitHub provides a handy framework that encourages users to work together.
3. We would like to minimize the number of additional steps a user needs to take after signing up. Users who design experiments must have a GitHub account to push experiments, but users who only run trials do not need a GitHub account since trials can be handled solely through the website. We anticipate that some users who start out running trials may also run experiments later. Requiring all users to create a GitHub account means that users do not have to jump through an extra set of hoops to set up a GitHub account later if they decide to run experiments; they can get started right away. 

The diagram below illustrates the Sign Up process. We will take a look at each step separately.

<!---Sign Up pic-->

##Sign up

We will first make a brief detour to the Sign Up field on the **Landing Page** to discuss the sign up process, and then go back to the Navigation Bar to take a look at the log in process.  

<!---Landing Page screenshot with Sign Up field highlighted-->

###Step 1

The **Sign Up** page consists of three separate steps. We would like to display only one step at a time while showing progress. All steps should be displayed on the same Sign Up page with the same wrapper. Each step should be bite-sized and modular, and fold away so that the user knows it is complete without having to see the entire step. Users should not feel overwhelmed by a long form.

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
 
###Step 2

After verifying an email address, the user is prompted with two buttons, either to log in or sign up using GitHub. GitHub does not allow user log in and sign up to be conducted on an external site, which means that this process has to take place on GitHub and then redirect the user back to the Popper Researcher Website once log in or sign up is done. 

The log in screen is done through GitHub API and looks like the following. 

<!---GitHub log in screen-->
The sign up screen is done through GitHub API as well, and looks like the following. 

<!---GitHub sign up screen-->
After log in or sign up, the user is redirected to a GitHub page to authorize GitHub access to the user's private and public information. This authorization is necessary to customize the user's **Experiments Library** so that the users's own public and private experiments are displayed. The only way to run a trial is through the **Experiments Library**, which means that Popper must be able to access both public and private repositories. Experiments from public repositories are visible to all users, while experiments from private repositories are visible only to users who have GitHub access to that repository. 

<!---GitHub authorization page-->
If the user has already granted Popper access to the user's GitHub account, Step 2 should either be hidden or minimized along with Step 1.

###Step 3

The user is redirected to the **Sign Up** page after granting GitHub access to Popper in order to provide Popper with a few last pieces of information not available through GitHub: 

- First Name
- Last Name
- Affiliation
- Department

First and Last Name are required here because GitHub does not ask users to input their first and last names separately, and we want to make sure that we have the full names of all users. Affiliation usually refers to an institution such as a university. We would like users to be able to write in their affiliation using auto-complete. If their institution is not found from our provided list, the user simply finishes typing the name of the affiliation. For example, typing "D" should bring up Duke University in autocomplete (among other affiliations) but Bob's Garage of Experiments would be written as-is. 

The complete list of all institutions and departments that run economics experiments can be found [here](http://edirc.repec.org/alphabet.html). If possible, we would like to scrape institution and department names somehow from this website. Manual entry of all institutions and departments into a spreadsheet is also possible but would be highly time-consuming: the United States alone has 3,149 institutions, each of which has several departments, and we want to include all institutions and departments from every country in the world. 

Finally, by clicking "Submit", the user agrees to the Popper Terms of Service, which we will provide. The Terms of Service should open in a popup window.

##Log In

The Log In process is tied closely to the Sign Up page. You'll recall that Sign Up requires three components: email verification, a linked GitHub account, and additional information. The log in process includes a series of checks in the backend to make sure that a user account includes all three components.

The below diagram shows how Log In works and how it is connected to Sign Up. We will now take a look at what happens from the moment the user clicks "Log In" from the Navigation Bar. 

<!---Log in pic-->

###Logged into GitHub?

<!---accounts 1 image-->
When a user clicks "Log In", Popper first checks whether the user is currently logged into GitHub from the current browser. If the user is not logged into GitHub, the user is taken to the GitHub log in page, which is the same page that the user sees after clicking "Log In using GitHub" from the **Sign Up** page.

###GitHub account?

<!---accounts 2 image-->
Now that the user is on the GitHub log in page, let's assume the user is not logged into a GitHub account from the current browser. 

If the user does not have a GitHub account, she can sign up for an account by clicking "(Pricing and Signup)". Just as during Sign Up, the user then grants Popper access to public and private GitHub user information. This user does not have a complete Popper account, so Popper redirects the user to the **Sign Up** page. 

Popper then checks whether this GitHub account is associated with a verified email address in the Popper user account database. 

If there is already an associated email address, Step 1 shows the message, "Your email nash@princeton.edu has been successfully confirmed!" and Step 1 is shown as complete in the same way as during Sign Up. Step 2 is also shown as complete, and the user will need to complete Step 3 on the **Sign Up** page. 

The more likely scenario is that the GitHub account is not associated with a verified email address. In this case, Step 1 should be shown as incomplete and Step 3 should not be available for the user to complete. The user verifies an email address in Step 1. Both Step 1 and Step 2 are shown as complete and the user finishes Sign Up by filling out Step 3.

If the user does have a GitHub account, the user logs in using GitHub credentials on the GitHub log in page, and then grants Popper access to the user's GitHub account.

###Verified email address?
<!---accounts 3 image-->

Once the user is logged into a GitHub account, Popper checks whether this GitHub account is associated with a verified email address. This check is identical to the one mentioned in the previous subsection, "GitHub account?". The difference is that in the previous section, the check happens while the user is on the **Sign Up** page, while here the check happens without taking the user to **Sign Up** just yet.

If the user does not have a verified email address, she is taken to the Sign Up page to complete Step 1. Since the user has already logged into GitHub and granted Popper access to the GitHub account, Step 2 is marked as complete and the user proceeds straight to Step 3.

If the user does have a verified email address, she is taken to the final check: "Has the user entered Popper credentials?"

###Popper credentials?
<!---accounts 4 image-->

Popper now checks whether this user, who has a verified email address and a linked GitHub account, has entered additional Popper credentials required in Step 3 of **Sign Up**. 

If the user has not entered Step 3 information, the user is taken to the **Sign Up** page to complete Step 3.

If additional user information exists, the user is logged in and taken to the **Dashboard**. 

#Landing Page 

The purpose of the **Landing Page** is to convince social science researchers to sign up<!---IL--> to use Popper. The **Landing Page** answers the question, "What Is Popper?" and provides reasons that the researcher should try to use Popper in place of their current software. 

Since the site serves an academic audience, the overall look of the **Landing Page** should be classic yet modern, and convey academic legitimcy. We are leaning towards a light, clean color scheme.

![Image](https://github.com/liscovich/functional-specs/blob/master/images/landingpage.png?raw=true)

The **Landing Page** consists of seven components: 

1. Logo
2. Navigation Bar
3. Overview
4. Usage Statistics
5. Features
6. Sign Up (Verify Email)
7. Footer

##1. Logo
<!---pic-->

![Image](https://github.com/liscovich/functional-specs/blob/master/images/lplogo.png?raw=true)

The Popper Logo contains the name "Popper" accompanying a stylized likeness of the philosopher Karl Popper. The ideal portrait for this logo is available [here](http://en.wikipedia.org/wiki/File:Karl_Popper.jpg) in the public domain from Wiki Commons. 

<center>
	<IMG SRC="http://upload.wikimedia.org/wikipedia/commons/4/43/Karl_Popper.jpg" WIDTH="10%" ALT="POPPER_PHOTO" BORDER="2.5">
	</center>

We would like to include Karl Popper's likeness to clarify the origin of the name "Popper" and dissociate the alternative meanings of the word. The logo should be designed to stand out well against both the light background of the Researcher Website and the dark background of Unity3D, a core component of the Popper SDK. 

The font of the logo should be classical and convey both authority and legitimacy, much like the logos of universities and research software.

<center>
	<img src="https://github.com/liscovich/functional-specs/blob/master/images/harvard_logo.png?raw=true" width="100%">
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

Finally, the logo should have a corresponding smaller "minilogo" that appears in the browser title bar. This minilogo should most likely be a "P" that corresponds stylistically with the Popper logo.

When a user is not signed in, clicking on the Popper Logo brings the user to the landing page at [www.popper.org](www.popper.org). Once the user signs in, clicking on the Popper Logo brings the user to the **Researcher Dashboard**, which will be discussed later.

##2. Navigation Bar
<!---pic-->

![Image](https://github.com/liscovich/functional-specs/blob/master/images/lpnav.png?raw=true)

The Navigation Bar in the Header includes four links: 

- **How It Works**
- **Our Story**
- **Experiments Library**
- **Log in**

[1] **How It Works** links to documentation for Popper. Documentation is stored on GitHub, not on the Popper Researcher Website. Clicking on **How It Works** takes the Researcher to a public repository linked with the official [Popper GitHub account](https://github.com/Experiments/). We will take care of writing documentation.

[2] **Our Story** is a static About page. Its contents will be discussed later.

[3] **Experiments Library** is a dynamic page on the Popper Research Site that allows researchers to browse experiments, and will be discussed later.

[4] User log in and sign up were discussed in the previous section, "Accounts". <!---internal link-->

##3. Overview
<!---pic-->

The purpose of the Overview is to describe Popper briefly. We anticipate that initially, most users who come to [www.popper.org](www.popper.org) will know little to nothing about Popper. The most that users might know is that Popper is a tool that lets social scientists run experiments.	

The header of the **Landing Page** is <code>"Behavioral Experiments Platform, [a(n) adjective] one"</code>. We would like to replace the <code>[a(n) adjective]</code> with a revolving list of serious and funny words. We are unsure from a UX perspective whether it would be more pleasant to have the words automatically refresh every few seconds or if it would be better for the user to click a small "refresh" icon next to the <code>[a(n) adjective]</code> to make the word change.

Here is the list of words -- we would like for the succession of words to be random but the first word that appears when the user arrives on the **Landing Page** should always be a word from the Serious list. 

**Serious** 

- an agile
- a modern
- a versatile
- a cutting-edge
- a customizable
- an addictive
- an advanced
- a promising
 
**Funny**
 
- a fat-free
- a low cholesterol
- a low emissions
- a PG-13
- a lactose intolerant
- a free range
- a whole wheat
- a hormone free
- an antibiotic free
- a TSA-compliant
- a pasteurized

Underneath the header is a short paragraph explaining what Popper is. 

> Popper is a powerful blend of modern technology and social science. Using Popper, you can design complex cutting-edge experiments using the most advanced tools in existence. You can also run large-scale online trials drawing subjects from the world's deepest on-demand subject pool.

##4. Usage Statistics
<!---pic-->

We would like to include usage statistics to boost the legitimacy of Popper among researchers. This portion of the **Landing Page** should be located directly under the Hook. Three statistics should be dynamically displayed and updated: the number of researchers, the number of deployed experiments, and the number of completed trials. The focus is on the numbers, which means that these digits should stand out much more than the names of what the numbers are counting. These statistics will only be available once Popper gains traction, which means that it would be ideal for there to be a way for us to activate this section of the site only once we have compelling statistics to show. This means that the **Landing Page** should visually "work" even if the statistics portion of the page is not shown. 

##5. Features
<!---pic-->

After the user gets some sense of what Popper is, the Features List provides a more detailed explanation of why the user should make the decision to Sign Up. The Features List describes four core selling points of Popper:

1. Start at the Frontier

2. Program the Way You Think

3. Run When You Are Ready

4. Leave Logistics to Us

These four features should be arranged on a horizontal navigation panel. Each of the four phrases should be accompanied by an image, which we will provide. Underneath the navigation panel is a frame split in half vertically, with text in the left panel and an image in the right panel. As the user clicks on each of the four features, the contents of the frame change. We are currently deciding on the four sets of text and images to place into this frame. Below is a draft of what we would like to include in the frame. 

###Start at the frontier

Begin running experiments right away. Browse the Experiments Library to find the best existing experiments. Share, discuss, and collaborate on best-practice experiment design effortlessly with a community of professionals. Retrieve the entire experiment protocol for any publicly available experiment 24/7 from our servers. Best of all, replicating an experiment only requires three clicks. 

Popper relies on frontier technology, which means that it improves daily. 

### Program the Way You Think
 
Design experiments using intuitive visual programming. Popper comes equipped with domain-specific nodes, custom-tailored for behavioral experiments. Easily automate common experiment tasks using one of our templates. Popper features full Mathematica support for computationally-intensive functionality. Those with more programming experience can delve past visual programming into the C# code underlying all experiments. 

### Run When You Are Ready

Draw from our on-demand online subject pool. Without the physical restraints of a lab, subjects can participate from the comfort of their homes, when you need them to. Deploy experiments in minutes, without worrying about searching and coordinating eligible subjects. 

### Leave Logistics to Us

Popper is built on a secure cloud infrastructure of servers, which means that you can focus on science rather than logistics. We handle all technical overhead related to subjects, from recruitment to screening to payment. We also provide an archive of IRB experiment-specific approvals for your convenience to expedite your own IRB approval process. 

##6. Sign Up (Verify Email)
<!---pic-->

Users can begin the sign up process by entering their email in this field for verification. Read more about the sign up process in the previous section, "Accounts". <!---internal link-->

##7. Footer
<!---pic-->

The Popper footer contains secondary navigation and is divided into two components: general links and legal miscellany. The general links are divided into three vertical columns. The first column, "Popper", includes links to "Our Story", "Blog", and "Contact". The second and third columns include links to Documentation. We have not yet fleshed out the Documentation of Popper enough to know how many distinct links this section will include. 

The second half of the footer is comprised of links that run horizontally along the bottom of the page. These links are "Terms of Service", "Privacy", and "Security". Under these links is the text <code>"&copy; 2012 Popper. All Rights Reserved."</code> On the right side of this part of the footer is the Fixel logo, with the text <code>"Designed by Fixel"</code>.

The Sign Up and Log In pages feature the same Logo, Navigation Bar, and Footer as the **Landing Page** and *Our Story**

#Our Story

The **Our Story** page is a static About page. It explains who Karl Popper is and introduces the Popper team.

**Our Story** features the same Header and Footer as the **Landing Page**. On the left is a photo of Karl Popper taken by Lucinda Douglas-Menzies. This photo should be cropped as necessary to work with the overall design of the page. We were able to secure rights to use this photo, provided we give credit to the photographer. Under the cropped photo should be the text, <code>"&copy; Lucinda Douglas-Menzies"</code> and <code>"Reproduced with the generous permission of the photographer"</code>. 

To the right of Karl Popper's likeness, we would like to include a section called <code>"Behind the Name"</code> and, beneath it, <code>"Team"</code>. We are currently working on this text and will provide it once it is ready. For now, we anticipate that the text in each section will not be more than two paragraphs long. 

We would like the other static pages on the Researcher site to feature the same wrapper as **Our Story**. These other pages are **Contact**, **Terms of Service**, **Privacy**, and **Security**. **Terms of Service**, **Privacy**, and **Security** should open up in popup windows.

#Experiments Library

**Experiments Library** is the final page accessible to users who are not signed in from the **Landing Page**. The page includes a few additional features once a user has signed in. These differences will be noted below when relevant.

There are five main components in **Experiments Library**:

1. Logo
2. Navigation Bar
3. Footer
4. List of Experiments
5. Search Bar
6. Filter

##1. Logo

Same as **Landing Page**. <!---internal link-->

#2. Navigation Bar

A logged in user sees "Dashboard" where the "Our Story" link used to be. The "Log In" link is replaced by the user's email address, which opens out to a menu with the options "Profile" and "Log Out". <!---internal links--> Log Off signs the user off Popper and brings the user back to the **Landing Page**. A message telling the user that Log Out has been completed is not necessary: the user will know that log out is successful because the email address in the top right hand corner will once again be replaced by the "Log In" link.

A logged out user sees the same Navigation Bar as the logged-out version described on the **Landing Page**. <!---internal link-->

#3. Footer

Same as **Landing Page**. <!---internal link-->

#4. List of Experiments

The main feature of **Experiments Library** is a list of public experiments. All users can see this list, no matter if they are logged in or not. The idea is to allow researchers to be able to see what Popper offers without having to sign up first. The list of experiments is an embedded frame with a scrollbar. We would like to display three experiments per row.

This frame displays two sections of experiments: User Experiments and Stock Experiments, in this order. User Experiments are pulled from the user's GitHub repositories, which means that experiments contained in public repositories are visible to all other users and those from private repositories are visible only to someone who has GitHub access to that repository. A user would typically keep a repository private while the experiment is still being developed and then make the repository public once an accompanying paper has been published and the experiment is open for peer review and replication. 

Stock Experiments are stored in the [Popper GitHub account](https://github.com/Experiments/) and can be public or private. Stock Experiments allow researchers to run experiments right away, without having to design their own experiments from scratch. This is particularly important when Popper launches because no users will have designed their own experiments yet. Stock Experiments also provide researchers with templates of the most commonly run experiments in the social sciences. 

Popper reads through the content of a user's repositories and pulls only the ones that contain full experiments. Popper makes this determination by looking for metadata, source code, master client, and client files. If the user's GitHub account does not contain any experiments, "No experiments pushed to GitHub. Click [here](linktodocumentation.com) to learn how to design experiments." should be displayed in the section for User Experiments. "Here" links to Popper documentation on the [Popper GitHub account](https://github.com/Experiments/).

These experiments are sorted by date--repositories with the most recent changes are displayed first. The name of the repository (functioning as the name of the experiment), a description of the experiment, number of forks, and the academic journal in which the results of the experiment were published should be listed. The number of forks is necessary to list and include in the metadata because researchers may want to sort experiments by popularity, which is functionality we would like to include in the future once more experiments are available in **Experiments Library**. 

When a researcher hovers over an experiment, the square containing the name of the experiment and its information should change color. Clicking on the experiment brings the user to the **Experiment** page (formerly known as **Create Trial**) for that particular experiment, where the user can learn more about the experiment and create a trial.  

##5. Search bar

The search bar sifts through the contents of the List of experiments. As soon as a researcher begins to type, autocomplete suggestions should appear beneath the Search bar, in the style of Google search. When a researcher clicks on an experiment in the autocomplete list, that single experiment alone is displayed in the List of experiments. If the researcher instead hits Enter, a list of all experiments relevant to the search phrase will appear in the List of experiments, split up into the two sections mentioned above (User Experiments, Stock Experiments). 

Autocomplete search results should be formatted as follows:

> **Name of Experiment** - Description of experiment, truncated after a certain number of characters so that the number of forks and publication journal can appear at the end of the autocomplete suggestion... - *Forks: ##*; *Journal Name*

##6. Filter

Researchers can also search for an experiment by browsing with the filter, in the style of navigating with the left navigation bar to find a product on [Amazon.com](Amazon.com). 

[insert explanation of filters here, Andrey...]

At the same time, the frame to the right of the Filter should update if necessary to be populated with all experiments that match that filter, organized by section (User Experiments and Stock Experiments). If a user selects an experiment in the Filter, that experiment should be highlighted in the Filter and the Experiment List frame should update to display only that experiment, as well as the section that the experiment falls under (User Experiments and Stock Experiments).

#Dashboard

Researchers monitor trials in the **Dashboard**. The **Dashboard** consists of two main components: 

1. Trials
2. Feed

##1. Trials

Trials is a list of all of the researcher's trials, both complete and ongoing. A trial enters this list as soon as a researcher clicks "Create Trial" on the **Create Trial** page, which will be discussed later. Clicking on the name of a trial brings the researcher to the **Trial Summary** page for that trial, which includes all parameters and actions specific to a particular trial. This page will be discussed later.  

Trials are sorted by activity date, which means that the most recently active trials appear at the top of the list. Trials can be in one of five statuses, and a change in status consitutes "activity" that pushes a trial to the top of the list. These statuses are displayed underneath the name of the trial, as shown in the wireframe. The five statuses are:

1. Awaiting players: The initial status of all trials that a researcher creates is "Waiting for players". This status indicates that the trial has been created and that the server is waiting for a sufficient number of subjects to join the game. The researcher can click on the name of the trial to go to that trial's **Trial Summary** page to recruit more subjects if necessary. 
2. In progress: Once enough subjects have joined a trial, the status of the trial changes to "In progress". Subjects play the game, and as they do, data from the experiment is sent to the **Trial Summary** page.
3. Pay subjects: Once a trial is complete, the researcher pays subjects. The researcher can review and approve subject payments from the **Trial Summary** page.
4. Complete: After payment is complete, the status of the trial changes to "Complete". No further action is required from the researcher at this time, but the trial is saved in the List for the researcher to review and download data. 
5. Error: If there is an error with any part of the trial, the researcher can click on the trial to go to **Trial Summary** in order to fix the error.

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
	- Pay subjects: "**Trial ##** has finished. Go to the **Trial Summary** page to review subject payments."
	- Complete: "**Trial ##** is now complete."
- Fork activity
	- "Researcher ## has just forked your experiment, **Experiment Name**."
- Following activity
	- "**Researcher ##** is now following **Trial ##**."
	- "You are now following **Trial ##** by **Researcher ##**."

Each bolded item in the above bulleted list should be a link that opens in a new tab. **Trial ##** links to the **Trial Summary** page for a particular trial. **Player ##** links to a player profile, which is hosted externally on the Player Website. **Researcher ##** links to the public profile view of another researcher; this profile is hosted on the Researcher Website.

Just as with the Trials frame, a "More..." button below the Feed frame scrolls down the entire window and allows the researcher to see more feed information.

The Header and Footer of **Dashboard** are identical to the logged-in view in **Experiments Library**. <!---internal link-->

#Experiment

The **Experiment** page is the same thing as the **Create Trial** page described in the original [Popper brief](https://github.com/Experiments/popper-design/blob/master/popper_brief.md). 

This page describes the experiment and allows the user to run a trial of the experiment. **Experiment** consists of four components:

1. Header
2. Footer
3. Experiment Description
4. Create Trial

##1. Header

Logged in users see the same Header as the logged in version described in Experiment Library. Logged out users see the Header described in the landing page. <!---internal link-->

##2. Footer

The Footer is the same as the one described on previous pages. <!---internal link-->

##3. Experiment Description

Popper reads the metadata file from the experiment GitHub repository to dynamically generate the Experiment Description. The metadata file itself is generated using the **Experiment Parameters** form on the Popper website. This page of the site does not need to be designed, since it should use the same design as the Sign Up page. We would like to provide users with a stock list of parameters that usually accompany any experiment, but also give users the flexibility to omit and add fields as necessary. A user should also be able to click "Edit" next to a field to change portions of the Experiment Description if the experiment came from this user's repository. Even if an experiment is public, the Experiment Description is read-only for users who do not own the GitHub experiment repository, and these users do not see "Edit" next to any of the fields. 

Here is a preliminary list of stock fields that we suggest accompany all experiments.

**User provided**

- Name of the experiment.
- Authors of the experiment with links to their Popper profiles. <!---internal link-->
- Description of the experiment.
- References.
- IRB approval(s): All social science research conducted in the United States receiving federal funding requires an IRB approval form before the researcher can conduct the experiment. It would be up to the researcher to make sure that the appropriate form is complete and attached, since Popper is not responsible or liable for monitoring the IRB approval process for researchers.
- Categories: We will provide a list of categories for each field. As the user begins typing, this field would provide suggested categories in "tag" form. The researcher would also be able to enter other categories that are not included in our suggestions. The purpose of categories is to sort experiments so that they are searchable using the Filter tool in the Experiment Library.

**Automatically generated for all experiments**

- Original repository, if the experiment repository was forked
- Link to GitHub repository holding the experiment
- Automatically generated "citation link" of the form "http://expt.cc/######", where # is a randomly generated digit. This citation link is a short URL to the **Experiment Page** for an experiment
- Discussion: Researchers should be able to post comments about an experiment. A user must be logged in to leave comments, as we would like to make sure comments are made by actual researchers. 

##4. Create Trial

As with Experiment Description, Create Trial is generated based on what the user specifies in the **Experiment Parameters** form. Users would be able to add to or delete from a stock list of parameters for a trial. Here is the list of suggested parameters:

- Number of subjects
- Cost of cooperation
- Multiplier
- Continuation probability
- Initial endowment
- Exchange rate (points to dollars)
- Frame (different visualizations of the game)
- Subjects (the pool of subjects for the trial)
- Gender
- Age
- Option to make trial results public
- Connection speed
- Connection latency

Below the create trial box is a list of previous trials that were run using the same experiment. Clicking on the name of the trial brings the user to the **Trial Results** page, which is accessible only if the user ran the trial or if the trial results are made public. Clicking on the name of the researcher brings the user to the researcher's Popper **Profile**.

Create Trial must be able to accomodate a wide range of parameters because experiments differ greatly. Since the parameters depend on the coding of the master client and client files of the experiment, the researcher would know what parameters are necessary and what parameters the server would accept as inputs based on the design of the experiment. 

#Trial Summary

The **Trial Summary** is the same as the **Monitor Trial** page described in the original [Popper brief](https://github.com/Experiments/popper-design/blob/master/popper_brief.md). This page allows the researcher to monitor an individual trial in real time and download the results once the trial is complete. **Trial Summary** consists of six components:

1. Header
2. Footer
3. Trial Information
4. Players
5. Report
6. History

##1. Header

See above. <!---internal link-->

##2. Footer

See above. <!---internal link-->

##3. Trial Information

- Name of the experiment: Clicking on this link brings the user to the **Experiment Page** for this particular experiment.
- Trial number: For reference purposes. Trials are numbered in the order that they are created on Popper.org.
- Start: Initiate the server instance and begin the trial.
- Stop: End the trial manually.
- Pause: Suspend the trial temporarily.
- Replicate: The user is brought to the **Experiment** page for this trial with all fields in Create Trial already filled in. All the user needs to do is click "Create Trial" to replicate the trial, or change parameters if desired.

##4. Players

The researcher can see a list of all subjects who have participated or are currently participating in the trial. The following stock parameters are suggested but can be added to or deleted on the **Experiment Parameters** page.

- Player ID: The researcher does not know subject names. Clicking on the Player ID of a subject brings the user to the public player profile on the Popper Player Website, which will be discussed later.
- Status: A player who has the game open in the player's current browser tab is <code>Active</code>. A player who navigates to a different browser tab is <code>inactive</code>. A player who prematurely closes the browser tab to leave the trial has <code>Dropped out</code>.
- Stage: If there are multiple steps in the trial, the researcher can see how far each subject has progressed.
- IP address: The user can prevent cheating by checking whether multiple users are actually playing from the same IP address. 
- Location
- Platform
- Earnings
- Approved: The researcher approves subject payments buy clicking the checkbox next to a player's earnings. This option is not available until the trial ends or the researcher manually clicks "Stop" to end the trial.

##5. Report

The Report is a list of purely quantitative data. The data collected for each trial is specified by the user. At the conclusion of a trial, the user can download the data in the form of a .csv, .xls, or .pdf file. Here are suggested types of data that users collect:

- Stage
- Player
- Choice: Can be a binary variable but does not have to be; its significance is specified by the user in the source code of the experiment and on the **Experiment Parameters** page.
- Duration: The amount of time that it took for a player to make a particular choice.
- Balance: A snapshot of the player's current points balance.

##6. History

The History is a qualitative description of the events of the trial. Like the Report, the output of the History of a trial depends on what the user specifies. Regardless of these specifications, the history should include at the minimum the Timestamp of an event and the name of the event.

#Profile

Wireframe needs to be created.

#Experiment Parameters

Wireframe needs to be created.