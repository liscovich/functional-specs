#Popper Functional Specifications

The Popper Functional Specs describe the three core components of Popper: (1) The Researcher Site, (2) The Player Site, and (3) The Popper Software Development Kit. These Functional Specs serve to make sure that everyone is on the same page about the functionality and purpose of each of the components of Popper. This document is an organic work in progress and will likely change over time. We will notify everyone when changes are made.

Two types of names are bolded in this document: **Web Pages** for the Researcher Site and Player Site, and **subcomponents** for the Popper Software Development Kit. These items are bolded and assigned a consistent name throughout the text. 

#Researcher Site

##Audience

The Researcher Site serves two types of users: 

1. Social Science researchers from academic institutions
2. Researchers from non-academic institutions

The first category of researchers includes professors, graduate students, and research assistants in the fields of economics, political science, psychology, and sociology. The second, non-academic category of researchers come from a variety of companies and backgrounds, including Microsoft and think tanks. Both sets of researchers attempt to use experiments to better understand and explain human behavior. 

Most of these researchers currently use z-Tree, software from the 1990s that requires researchers to learn how to program. Researchers are accustomed to bare-bones UI for both themselves and their subjects. These researchers typically know a limited amount of programming but are open to technologically complex tools, since much of their work relies on technology such as [STATA](www.stata.com), [z-Tree](http://www.iew.uzh.ch/ztree/index.php), and [R](http://www.r-project.org/).

Users fall into two typical use cases: 

1. The Experiment Designer
2. The Trial Runner

###1. Professor Goldin, the Experiment Designer

Professor Goldin is an economics professor at Carnegie Mellon University. For over ten years, she has used [z-Tree](http://www.iew.uzh.ch/ztree/index.php), the dominant social science experiments software, to study human behavior. She knows a rudimentary amount of programming--just enough to design experiments in z-Tree. Each trial takes several weeks to run, and much of this time is spent handling logistics: recruiting subjects, waiting for subjects, screening subjects, reserving computer lab space at the university's social science experiments facility, and ensuring that subjects are paid. 

Professor Goldin hears about Popper at an Experimental Economics Conference and visits [www.popper.org](www.popper.org). On the **Landing Page**, she reads about how Popper works and signs up for an account. She downloads the Popper SDK and reads through the Popper documentation. The first trial that she runs uses one of the stock experiments available publicly. She makes a few changes to the experiment design in [Unity3D](http://unity3d.com/), which is provided as part of the Popper SDK. Once she finishes designing the experiment to her satisfaction, Professor Goldin asks her research assistant, Robert, to run trials using this experiment. 

Soon, Professor Goldin begins designing her own experiments from scratch using templates from the Popper SDK and assets downloaded from the [Unity Asset Store](http://unity3d.com/unity/asset-store/). Popper takes care of logistical and technical issues so that Professor Goldin can focus on her research rather than tedious overhead. Her trials now take hours, rather than weeks, to run. 

###2. Robert, the Trial Runner

Robert is a research assistant working for the economics department at Carnegie Mellon University. His job this summer is to run trials and crunch data for Professor Goldin. Robert knows no programming but has taken a few statistics courses. Professor Goldin asks him to set up an account at www.popper.org. He signs up on the **Landing Page** and follows a set of simple instructions to create an account. Robert links Professor Goldin's laboratory GitHub account with his Popper account, and is able to find the lab's private experiments on the **Experiments Library** page. He selects one of the experiments and fills in a set of parameters for who is allowed to participate in the trial and the type of data he would like to collect. Robert clicks Create Trial, and eligible subjects are automatically recruited from Amazon MTurk and oDesk. He monitors the progress of the trial on the **Researcher Dashboard** page. A few hours later, the trial is complete and Robert downloads the data to analyze further. 

##Landing Page 

The purpose of the **Landing Page** is to convince social science researchers to _Sign up_ to use Popper. This Sign up process will be later discussed in further detail. The **Landing Page** answers the question "What Is Popper?" and provides reasons that the researcher should try to use Popper in place of their current software. 

The overall look of the **Landing Page** should be classic yet modern. Since the audience ranges from graduate students in their mid-20s to older professors, it is essential that the site does *not* have a plastic, generically Web-2.0 feel. We are leaning towards a light, clean color scheme. The **Landing Page** must convey academic legitimacy: it is essential that researchers not feel that they are marketing targets.

The **Landing Page** consists of six components: 

1. The Header

2. The Hook

3. Statistics

4. The Features List

5. Sign Up

6. The Footer

###1. The Header

The Header contains the Popper Logo and the Navigation Bar. 

####Popper Logo

The Popper Logo contains the name "Popper" accompanying a stylized likeness of Karl Popper, the philosopher after whom the product is named. The ideal portrait for this logo is available [here](http://en.wikipedia.org/wiki/File:Karl_Popper.jpg) in the public domain from Wiki Commons. We would like to include Karl Popper's likeness to emphasize that the name "Popper" does not refer to drugs or the action of "popping". The logo should be designed to stand out well against both the light background of the Researcher Website and the dark background of Unity3D, which is a core component of the Popper SDK. 

The font of the logo should be classical and convey both authority and legitimacy, much like the logos of universities ([Harvard](http://www.harvard.edu/), [Dartmouth](http://www.dartmouth.edu/), [University of Texas](http://www.utexas.edu/)), as well as research technologies like [Wolfram Alpha](http://www.wolframalpha.com/). Finally, the logo should have a corresponding smaller "minilogo" that appears in the title bar of web browsers. This minilogo should most likely be a "P" that corresponds stylistically with the Popper logo.

####Navigation Bar

The Navigation Bar in the Header includes four links: 

1. How It Works

2. Our Story

3. Experiment Library

4. Log in

*How It Works* links to documentation for Popper. Clicking on this link takes the Researcher to a public repository linked with the official [Popper GitHub account](https://github.com/Experiments/). We will take care of writing documents for the Documentation repository to explain to users how to use Popper.

*Our Story* links to the **Our Story** page, which functions as an About page. **Our Story** is a static page and its contents will be discussed later.

*Experiment Library* links to our **Experiment Library**, which is a page on the Popper Research Site that allows researchers to explore all available experiments. **Experiment Library** is dynamic and looks different for each user as it pulls information from GitHub repositories linked with each user's account. This page of the site will be discussed later.  

*Log in* opens an ajax popup window that allows researchers who already have an account to log in using their Email and Password. We would like to use each user's email address as their User Name to minimize the number of steps it takes to sign up and to encourage the creation of only one account per researcher. The ajax popup window should be minimalistic: at the top of the window should be the words "Log in". Under these words should be two fields: "Email" and, beneath that, "Password". Under the password field should be a a link that says "Forgot password?". Under "Forgot password?" should be a button that says "Log in". Under this button should be another button that contrasts in color with the "Log in" button, and says "Sign up". We do not anticipate this Sign Up button to be the primary way that new users create an account, but we would still like to provide the option of signing up for a new user who happens to click on "Log in".

A valid user name and password combination signs in the user and brings the user to the **Researcher Dashboard**. Users who are signed in should, by default, remain signed in unless they log out. There should not be a "Remember Me" checkbox: we want to minimize clutter and only show what the user needs to see. If the user enters an invalid username or password, the fields should vibrate quickly left to right and the message "Invalid username or password." should appear beneath the Password field, in the location where the "Log in" button was originally. The "Log in" and "Sign up" buttons appear beneath the "Invalid username or password" message, in all making it appear as if the "Invalid username or password" status pushed the two buttons down the page.

If a user clicks on the "Forgot password?" link, the ajax popup should change to display the title "Forgot Password?" and only one field: "Email". Under this field is a message that says, "To reset your password, please enter your email address." Underneath this message should be a button that says "Submit". If the email address that the user enters cannot be found in the database, the popup window shakes from left to right rapidly and displays the error message, "Sorry, your email address could not be found." If the email matches one in the database, the message "Please check your email for instructions to reset your password." replaces the text "To reset your password..." and [support@popper.org](support@popper.org) sends a formatted email with the subject "Reset your Popper password" to the user. At the top of the email is a header incorporating the Popper logo. The following text appears: 

> ***Forgot your password?***
>
> To reset your password, please click the link below:
> 
> [Link to reset password]
> 
> If you have any questions, please email us at [support@popper.org](support@popper.org).
> 
> Thanks,
> 
> The Popper Team

When the user clicks the password reset link, a new tab should open in the user's browser bringing the user to the **Landing Page** with an ajax popup window in the exact same style as the Log In popup window described above. The title of this popup is "Reset Password", with three fields. The first field is "Email Address" and should be pre-populated with the email address for the password reset. Right underneath is a second field, "New Password" and beneath that, a third field, "Confirm New Password". Under "Confirm New Password" is a button, "Submit". The password must be at least 6 characters in length, and contain both numbers and letters. If the password doesn't fit these parameters, the ajax popup shakes from left to right and the following message shows up at the top of the screen, directly below "Reset Password": Your password must be at least 6 characters long and contain both letters (A-Z) and numbers (0-9). 

Once the user clicks "Submit" for a valid new password, the ajax popup window switches back to the Log In layout described above, with the email address field pre-populated with the email address that was just used for Reset Password. 

###2. The Hook

The purpose of the Hook is to describe to the user, briefly, exactly what Popper is. We anticipate that initially, most users who come to www.popper.org will know little to nothing about Popper. The most that users might know is that Popper is a tool that lets social scientists run experiments.

The header of the **Landing Page** is "Behavioral Experiments Platform, [*a(n) adjective*] one". We would like to replace the [*a(n) adjective*] with a revolving list of words, both serious and funny. This header is meant to add character and likeability to the Researcher Site. In terms of execution, we are unsure whether it would be more pleasant from a UX perspective to have the words automatically refresh every few seconds or if it would be better for the user to click a small "refresh" icon next to the [*adjective*] to make the word change. As a design decision, we are unsure whether the "an [adjective] one" phrase should be capitalized or lower case.

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

###3. Statistics

We would like to include usage statistics to boost the legitimacy of Popper among researchers. This portion of the **Landing Page** should be located directly under the Hook. Three statistics should be dynamically displayed and updated: the number of researchers, the number of deployed experiments, and the number of completed trials. The focus is on the numbers, which means that these digits should stand out much more than the names of what the numbers are counting. These statistics will only be available once Popper gains traction, which means that it would be ideal for there to be a way for us to activate this section of the site only once we have compelling statistics to show. This means that the **Landing Page** should visually "work" even if the statistics portion of the page is not shown. 

###4. The Features List

After the user gets some sense of what Popper is, the Features List provides a more detailed explanation of why the user should make the decision to Sign Up. The Features List describes four core selling points of Popper:

1. Start at the Frontier

2. Program the Way You Think

3. Run When You Are Ready

4. Leave Logistics to Us

These four features should be arranged on a horizontal navigation panel. Each of the four phrases should be accompanied by an image, which we will provide. Underneath the navigation panel is a frame split in half horizontally, with text in the left panel and an image in the right panel. As the user clicks on each of the four features, the contents of the frame change. We are currently deciding on the four sets of text and images to place into this frame. The following text is a draft of what we would like to include in the frame. 

####Start at the frontier

Begin running experiments right away. Browse the Experiment Library to find the best existing experiments. Share, discuss, and collaborate on best-practice experiment design effortlessly with a community of professionals. Retrieve the entire experiment protocol for any publicly available experiment 24/7 from our servers. Best of all, replicating an experiment only requires three clicks. 

Popper relies on frontier technology, which means that it improves daily. 

#### Program the Way You Think
 
Design experiments using intuitive visual programming. Popper comes equipped with domain-specific nodes, custom-tailored for behavioral experiments. Easily automate common experiment tasks using one of our templates. Popper features full Mathematica support for computationally-intensive functionality. Those with more programming experience can delve past visual programming into the C# code underlying all experiments. 

#### Run When You Are Ready

Draw from our on-demand online subject pool. Without the physical restraints of a lab, subjects can participate from the comfort of their homes, when you need them to. Deploy experiments in minutes, without worrying about searching and coordinating eligible subjects. 

#### Leave Logistics to Us

Popper is built on a secure cloud infrastructure of servers, which means that you can focus on science rather than logistics. We handle all technical overhead related to subjects, from recruitment to screening to payment. We also provide an archive of IRB experiment-specific approvals for your convenience to expedite your own IRB approval process. 

###5. Sign Up

The Sign Up process should feature minimal initial friction. To sign up, users enter their email address in a field located under The Features List. Next to this field is a button, "Get Started", that sends an email with the subject "Verify Account" from support@popper.org. Once the user clicks "Get Started", text appears below this portion of the page that reads, "Please check your email to verify your account."

Like the Reset Password email mentioned above, the Verify Account email features a header with the Popper logo. Here's the text of the email: 

> Hello,
> 
> We received a request to create a Popper account for [email address]. To verify your account and complete the sign up process, please click [here](some.authenticated.URL.com). 
> 
> If you have any questions or believe you received this email in error, please email support@popper.org.
> 
> Thanks,
> 
> The Popper Team

Clicking "here" in the above email opens a new window and takes the user to the Sign Up page, which will be discussed in detail later.

###6. Footer

The Popper footer contains links, and is divided into two components: general links and legal miscellaney. The general links are divided into three vertical columns. The first column, "Popper", includes links to "Our Story", "Blog", and "Contact". The second and third columns include links to Documentation. We have not yet fleshed out the Documentation of Popper enough to know how many distinct links this section will include. 

The second half of the footer is comprised of links that run horizontally along the bottom of the page. These links are "Terms of Service", "Privacy", and "Security". Under these links is the text "(c) 2012 Popper. All Rights Reserved." On the right side of this part of the footer is the Fixel logo, with the text "Designed by Fixel".