latex input:		mmd-article-header  
Title:				Popper Functional Specifications  
Base Header Level:	2  
latex mode:			memoir  
Keywords:			MultiMarkdown, Markdown, XML, XHTML, XSLT, PDF   
CSS:				fspecs.css	
xhtml header:		<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
<!---<META HTTP-EQUIV="REFRESH" CONTENT="120">-->
copyright:			2012 Popper  
latex input:		mmd-natbib-plain
latex input:		mmd-article-begin-doc  
latex footer:		mmd-memoir-footer  

<h1> Functional Specifications </h1>

Popper is a behavioral experiments platform that empowers researchers in economics, psychology, sociology, and political science to create and conduct complex large-scale online experiments.

<section class="pages">
<ul>
	<li>1 &nbsp; <a href="#Introduction">Introduction (in progress)</a> </li>
		<ul>
			<li>1.1 &nbsp; <a href="#Correlation_vs_causation">Correlation vs. Causation</a></li>
			<li>1.2 &nbsp; <a href="#Experiments_in_sciences">Experiments in the natural and social sciences</a></li>
			<li>1.3 &nbsp; <a href="#Tradeoff">Tradeoff between internal and external validity</a></li>
			<li>1.4 &nbsp; <a href="#Current">Current experimental economics</a></li>
			<li>1.5 &nbsp; <a href="#Why_Popper">Why Popper?</a></li>
		</ul>	
	<li>2 &nbsp; <a href="./researcher_site.html#Researcher_Site">Researcher Site</a></li>
		<ul>
			<li>2.1 &nbsp; <a href="#RSAudience">Audience</a></li>
			<li>2.2 &nbsp; <a href="#RSLook">Look and Feel</a></li>
			<li>2.3 &nbsp; <a href="#RSAccounts">Accounts</a></li>	
			<li>2.4 &nbsp; <a href="#RSIntroduction_page">Introduction Page</a></li>
			<li>2.5 &nbsp; <a href="#RSOur_story">Our Story</a></li>	
			<li>2.6 &nbsp; <a href="#RSExperiments">Experiments</a></li>
			<li>2.7 &nbsp; <a href="#RSDashboard">Dashboard</a></li>	
			<li>2.8 &nbsp; <a href="#RSExperiment_summary">Experiment Summary</a></li>
			<li>2.9 &nbsp; <a href="#RSTrial_summary">Trial Summary</a></li>
			<li>2.10 &nbsp; <a href="#RSProfile">Profile</a></li>
			<li>2.11 &nbsp; <a href="#RSSearch_Results">Search Results</a></li>		
		</ul>
	<li>3 &nbsp; <a href="./player_site.html#Player_Site">Player Site</a></li>
		<ul>
			<li>3.1 &nbsp; <a href="#PSAudience">Audience</a></li>
			<li>3.2 &nbsp; <a href="#PSAccounts">Accounts</a></li>
			<li>3.3 &nbsp; <a href="#PSLobby">Lobby</a></li>
			<li>3.4 &nbsp; <a href="#PSGame">Game</a></li>
			<li>3.5 &nbsp; <a href="#PSProfile">Profile</a></li>
			<li>3.6 &nbsp; <a href="#PSAbout">About</a></li>
		</ul>
	<li>4 &nbsp; Popper SDK</li>
		<ul>
			<li>4.1 &nbsp; In progress</li>
		</ul>
</ul>
</section>

<!---introduction

<h1> <a name="Introduction">Introduction</a> </h1>

# <a name="Correlation_vs_causation">Correlation vs. Causation</a>

Causality within reach. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

# <a name="Experiments_in_sciences">Experiments in the natural and social sciences</a>

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Consent from subjects

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Subjects change behavior

Subjects may change behavior because they know they are in an experiment. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

# <a name="Tradeoff">Tradeoff between internal and external validity</a>

Experiments approximate reality as much as possible. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

# <a name="Current">Current experimental economics</a>

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Milgram obedience expt: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Limits today in social science expts: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Time: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Money: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Red tape: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Current online expts = cheaper and faster but less control

# <a name="Why_Popper">Why Popper?</a>

Problem: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Current solutions and why they are bad: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

List of competitors: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Solution: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

How does Popper work? Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Popper consists of three components:

1. The Researcher Site
2. The Player Site
3. The Popper Software Development Kit

## Researcher site

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Player site

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Popper SDK

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

-->

<h1> <a name="Researcher_Site">Researcher Site</a> </h1>

The Researcher Site ([www.popper.org](http://www.popper.org)) allows researchers to explore available experiments, create trials, recruit subjects, monitor trials in real time, and download experimental data. 

## Pages

<section class="pages">
	<ul>
		<li>2.1 &nbsp; <a href="#RSAudience">Audience</a></li>
		<li>2.2 &nbsp; <a href="#RSLook">Look and Feel</a></li>
		<li>2.3 &nbsp; <a href="#RSAccounts">Accounts</a></li>	
		<li>2.4 &nbsp; <a href="#RSIntroduction_page">Introduction Page</a></li>
		<li>2.5 &nbsp; <a href="#RSOur_story">Our Story</a></li>	
		<li>2.6 &nbsp; <a href="#RSExperiments">Experiments</a></li>
		<li>2.7 &nbsp; <a href="#RSDashboard">Dashboard</a></li>	
		<li>2.8 &nbsp; <a href="#RSExperiment_summary">Experiment Summary</a></li>
		<li>2.9 &nbsp; <a href="#RSTrial_summary">Trial Summary</a></li>
		<li>2.10 &nbsp; <a href="#RSProfile">Profile</a></li>
		<li>2.11 &nbsp; <a href="#RSSearch_Results">Search Results</a></li>
	</ul>
</section>

# <a name="RSAudience">Audience</a>

The Researcher Site is used by experimental social scientists, who use experiments to understand human behavior. These researchers come from many different backgrounds, including the fields of economics, political science, psychology, and sociology, as well as corporations and think tanks. 

Most of these researchers currently use [z-Tree](http://www.iew.uzh.ch/ztree/index.php), software from the 1990s that requires researchers to learn how to program. Researchers are accustomed to bare-bones UI for both themselves and their subjects. These researchers typically know a limited amount of programming and are open to technologically complex tools, since much of their work relies on technology such as [STATA](www.stata.com), [z-Tree](http://www.iew.uzh.ch/ztree/index.php), and [R](http://www.r-project.org/).

Users fall into two typical use cases: 

1. The Experiment Designer
2. The Trial Runner

##1. Professor Goldin, the Experiment Designer

Professor Goldin is an economics professor at Carnegie Mellon University. For over ten years, she has used [z-Tree](http://www.iew.uzh.ch/ztree/index.php), the dominant social science experiments software, to study human behavior. She knows a rudimentary amount of programming--just enough to design experiments in z-Tree. Each trial takes several weeks to run, and much of this time is spent handling logistics: recruiting subjects, waiting for subjects, screening subjects, reserving computer lab space at the university's social science experiments facility, and ensuring that subjects are paid. 

Professor Goldin hears about Popper at an Experimental Economics Conference and visits [www.popper.org](www.popper.org). On the **Introduction Page**, she reads about how Popper works and signs up for an account. She downloads the Popper SDK and reads through the Popper documentation. The first trial that she runs uses one of the stock experiments available publicly. She makes a few changes to the experiment design in [Unity3D](http://unity3d.com/), which is provided as part of the Popper SDK. Once she finishes designing the experiment to her satisfaction, Professor Goldin asks her research assistant, Robert, to run trials using this experiment. 

Soon, Professor Goldin begins designing her own experiments from scratch using templates from the Popper SDK and assets downloaded from the [Unity Asset Store](http://unity3d.com/unity/asset-store/). Popper takes care of logistical and technical issues so that Professor Goldin can focus on her research rather than tedious overhead. Her trials now take hours, rather than weeks, to run. 

##2. Robert, the Trial Runner

Robert is a research assistant working for the economics department at Carnegie Mellon University. His job this summer is to run trials and crunch data for Professor Goldin. Robert knows no programming but has taken a few statistics courses. Professor Goldin asks him to set up an account at www.popper.org. He signs up on the **Introduction Page** and follows a set of simple instructions to create an account. Robert links Professor Goldin's laboratory GitHub account with his Popper account, and is able to find the lab's private experiments on the **Experiments** page. He selects one of the experiments and fills in a set of parameters for who is allowed to participate in the trial and the type of data he would like to collect. Robert clicks Create Trial, and eligible subjects are automatically recruited from Amazon MTurk and oDesk. He monitors the progress of the trial on the **Dashboard** page. A few hours later, the trial is complete and Robert downloads the data to analyze further. 

# <a name="RSLook">Look and Feel</a>

The site serves an academic audience so the overall look of the **Introduction Page** should be classic yet modern, and convey academic legitimacy. We are leaning towards a light, clean color scheme.

# <a name="RSAccounts">Accounts</a>

<!---A GitHub account is necessary for the following three reasons. 
1. GitHub eliminates the need to implement standard workflows on our side, like log in and password retrieval. 
2. We would like to encourage users to collaborate on experiments, and GitHub provides convenient tools for sharing and discussing code.
3. Using a GitHub account, all users can push experiments.
-->

## Overview

The Researcher Site requires users to have a GitHub account and authenticates them via GitHub OAuth API. In addition to the GitHub profile information, the following data are stored for each of the users: 

- First name
- Last name
- Email address
- Department and affiliation
- Payment method (credit card/PayPal)
- Activity history on the Site (experiments, trials, experiments recommended by the user)

##Components

1. <a href="#RSSign_Up">Sign Up</a>
2. <a href="#RSLog_In">Log In</a>

##<a name="RSSign_Up"></a>1. Sign Up

There are two ways for unregistered users to Sign Up:

1. By clicking on the "Sign Up" button in the Navigation Bar. 
2. By being redirected to Sign Up after logging in with GitHub.

Sign Up consists of three steps. Only one step is displayed at a time so that users are not overwhelmed. 

###Step 1: Email Confirmation 

<a href="https://github.com/liscovich/functional-specs/blob/master/wireframes/researcher_site/sign_up_1.png?raw=true" target="_blank"><img src="https://github.com/liscovich/functional-specs/blob/master/wireframes/researcher_site/sign_up_1.png?raw=true" width="100%"></a>

<section class="pages">
	<ul>
		<a name="Sign_Up_1_1"></a><li>1. &nbsp; The user enters an email and clicks "Sign Up".</li>
		<li>2. &nbsp; The following confirmation email is sent to the user from <a href="support@popper.org">support@popper.org</a>:</li>
 	</ul>
</section>

<section class="quote">
	<p>Subject: Confirm your Popper account</p>
	
	<p>Thanks for signing up with Popper! Please follow this link to activate your account:</p>
	
	<p><a href="https://www.someurlforsignup.com">https://www.someurlforsignup.com</a></p>
	
	<p>If you have any questions, please email us.</p>
	
	<p>The Popper Team</p>
</section>

<section class="pages">
	<ul>
		<li>3. &nbsp; The user clicks on the confirmation link in the email.</li>
		<li>4. &nbsp; The user is taken back to the Sign Up page, which has the same overall design as the email confirmation Sign Up page but contains different information.</li> 
	</ul>
</section>

###<a name="Sign_Up_2">Step 2: GitHub Authentication</a>

<a href="https://github.com/liscovich/functional-specs/blob/master/wireframes/researcher_site/sign_up_2.png?raw=true" target="_blank"><img src="https://github.com/liscovich/functional-specs/blob/master/wireframes/researcher_site/sign_up_2.png?raw=true" width="100%"></a>

<section class="pages">
	<ul>
		<li>1. &nbsp; The user is prompted to log in by either using an existing GitHub account or signing up for a new one.</li>
		<li>2. &nbsp; The user clicks either Log In with GitHub or Sign Up for GitHub.</li>
		<li>3. &nbsp; The user either logs in or signs up for GitHub on the GitHub website.</li>
			<ul>
				<li><a name=3a>a.</a> &nbsp; If the user clicks Log In, he or she is taken to the GitHub App Authorization page <i>in the same browser tab</i> with parameters. If the user is not logged in, he or she is taken to the log in page instead.</li>
				<a name="Sign_Up_2_3a"></a><li>b. &nbsp; If the user clicks Sign Up, he or she is taken to the GitHub Sign Up page to create a free account at <a href="https://github.com/signup/free">https://github.com/signup/free</a> <i>in a new browser tab.</i> Once the user has signed up, he or she can close the GitHub tab and log in using GitHub from the Researcher Site Sign Up page. The workflow proceeds from part <a href="#3a">3a</a> above.</li>
			</ul>	
		<li>4. &nbsp; The user authorizes Popper to access the user's public and private information, including all repositories.</li>
			<!---This authorization is necessary to customize the user's **Experiments** so that the users's own public and private experiments are displayed. The only way to run a trial is through the **Experiments**, which means that Popper must be able to access both public and private repositories. Experiments from public repositories are visible to all users, while experiments from private repositories are visible only to users who have GitHub access to that repository.-->	
		<li>5. &nbsp; The user is redirected to the Sign Up page, which features the same design but different content.</li>
 	</ul>
</section>

###<a name="Sign_Up_3"></a>Step 3: Profile Completion

1. The user provides the following information:
	- First name
	- Last name
	- Department and affiliation
	<p>Users enter their affiliation using autocomplete. If their institution is not found from our provided list, the user simply finishes typing the affiliation. Names of departments and affiliations need to be scraped from <a href="http://edirc.repec.org/alphabet.html">http://edirc.repec.org/alphabet.html</a>.</p>
2. The user clicks "Submit" and is doing so indicates agreement to the Popper Terms of Service, which we will provide. The Terms of Service should open in a popup window.
3. The user is redirected to the <a href="#RSDashboard">Dashboard</a>.

<!---First and Last Name are required because GitHub does not ask users to input their first and last names separately, and we want to make sure that we have the full names of all users.--> 
 
##Log In

The Log In process is tied closely to the Sign Up page. You'll recall that Sign Up requires three components: email verification, a linked GitHub account, and affiliation details. Logging in includes a series of checks in the backend to make sure that a user account includes all three components.

The below diagram shows how Log In works and how it is connected to Sign Up. We will now take a look at what happens from the moment the user clicks **Log In** from the Navigation Bar. 

<!---Log in pic-->

###Check 1: Logged into GitHub?

<!---accounts 1 image-->
<section class="pages">
	<ul>
		<li>1. &nbsp; A user clicks "Log In".</li>
		<li>2. &nbsp; The Researcher Site checks whether the user is currently logged into GitHub.
	 		<ul>
	 			<li>a. If the user is not logged into GitHub, he or she is taken to the GitHub Log In page and the Researcher Site proceeds to <a href="Check_2">Check 2</a>. This Log In page is the same one that the user sees <a href="#Sign_Up_2">after clicking "Log In using GitHub"</a> from the <a href="#Sign_Up">Sign Up</a> page.</li>
	 			<li>b. If the user is logged into GitHub, the Researcher Site proceeds to <a href="#Check_3">Check 3</a>.
	</ul>
</section>

###<a name="Check_2"></a>Check 2: GitHub account?

By Check 2, the Researcher Site has determined that the user is not currently logged in with a GitHub account.

<!---accounts 2 image-->
<section class="pages">
	<ul>
		<li>1. &nbsp; The user's action depends on whether he or she has a GitHub account.</li>
			<ul>
				<li>a. &nbsp; If the user does not have a GitHub account, he or she can sign up for an account by clicking "(Pricing and Signup)", which is discussed in <a href="#Sign_Up_2_3a">Step 2, Part 3</a> of the Sign Up process.</li>
				<li>b. &nbsp; If the user does have a GitHub account, the user logs in using GitHub credentials on the GitHub Log In page, and then grants Popper access to the user's GitHub account if this has not yet been done.</li>
			</ul>
		<li>2. &nbsp; The Researcher Site proceeds to <a href="#Check_3">Check 3</a>.
	</ul>
</section>

###<a name="Check_3"></a>Check 3: Confirmed email address?
<!---accounts 3 image-->

By Check 3, the user has logged in using a GitHub account and has granted the Researcher access to GitHub account information. 

<section class="pages">
	<ul>
		<li>1. &nbsp; The Researcher Site checks whether the user's logged-in GitHub account is associated with a confirmed email address.</li>
			<ul>
				<li>a. &nbsp; If the user does not have a verified email address, he or she is directed from GitHub to the email confirmation Sign Up page, which is described in <a href="Sign_Up_1_1">Step 1, Part 1</a> of the Sign Up process.</li>
				<li>b. &nbsp; If the user does have a verified email address, he or she passes Check 3.</li>
			</ul>
		<li>2. &nbsp; The Researcher Site proceeds to <a href="#Check_4">Check 4</a>.</li>
	</ul>
</section>

###<a href="Check_4"></a>Check 4: Profile completion?
<!---accounts 4 image-->

By Check 4, the user has logged in using GitHub and the Researcher Website has verified that this GitHub account is associated with a confirmed email address.

<section class="pages">
	<ul>
		<li>1. &nbsp; The Researcher Site checks whether the user has completed <a href="#Sign_Up_3">Step 3</a> of the Sign Up process by providing a full name, department, and affiliation.</li>
			<ul>
				<li>a. &nbsp; If the user has not completed a user profile, he or she is taken to the final Sign Up page, which is described in <a href="Sign_Up_3">Step 3, Part 1</a> of the Sign Up process.</li>
				<li>b. &nbsp; If the user has completed a user profile, he or she passes Check 4.</li>
			</ul>
		<li>2. &nbsp; The user is taken to the is taken to the <a href="#RSDashboard">Dashboard</a>.</li>
	</ul>
</section>

# <a name="RSIntroduction_page"></a>Introduction page

The **Introduction Page** introduces users to Popper. The primary action that a user takes is to <a href="#Sign_Up">sign up</a>.   

<img src="https://github.com/liscovich/functional-specs/blob/master/images/Introductionpage.png?raw=true" width="100%">

##Page Components

<!---internal lnks here-->
1. Navigation Bar 
3. Overview
4. Usage Statistics
5. Features
6. Footer

##1. Navigation Bar
<!---pic-->

<img src="https://github.com/liscovich/functional-specs/blob/master/images/lpnav.png?raw=true" width="100%">

The **Navigation Bar** includes five or six links, depending on whether the user is logged in: 

<!---internal links-->
1. Logo
2. <a href="#How_It_Works">How It Works</a>
2. Our Story
3. Experiments
4. Log In with GitHub
5. Sign Up
6. Dashboard (if logged in)

The **Logo** contains the word "Popper" accompanying a stylized image of the philosopher Karl Popper. We are including Karl Popper's likeness to clarify the origin of the name "Popper" and dissociate alternative meanings of the word. 

When a user is not logged in, clicking on the Popper Logo brings the user to the <a href="#RSIntroduction_page">Introduction Page</a> at [www.popper.org](http://www.popper.org). Once the user logs in, clicking on the Popper Logo brings the user to the <a href="#RSDashboard">Dashboard</a>.

A good starting point for the logo portrait is available <a href="http://en.wikipedia.org/wiki/File:Karl_Popper.jpg" target="_blank">here</a> in the public domain from Wiki Commons.  

###Logo Requirements

- **Facial expression:** In its current form, the above portrait is problematic because Karl Popper appears as if he may be looking around. In the logo, Popper should look pensive.
- **Cropping:** The face must be cropped so that it does not look as if it belongs at a funeral.
- **Different sizes:** The word "Popper" and the portrait should be recognizable whether the logo is small or large.
- **Color scheme:** The logo should be designed to stand out well against both the light background of the Researcher Site and the dark background of Unity3D, a core component of the Popper SDK. 
- **Font:** The font of the logo should be classical and convey both authority and legitimacy, much like the logos of universities and research software. 
- **Favicon:** The logo should have a corresponding favicon that appears in the browser title bar.

<h4>Examples of Unsuccessful Logos</h4>
|						   | <img src="https://github.com/liscovich/functional-specs/blob/master/images/popper-mosaic.png?raw=true" width="180px"> | <img src="https://github.com/liscovich/functional-specs/blob/master/images/popper-round-face.png?raw=true" width="180px"> | <img src="https://github.com/liscovich/functional-specs/blob/master/images/popper-square-face.png?raw=true" width="180px"> |
----------------------------------- |  :-----------  |  :------  |   :------  | 
**Facial expression**                   | Yes: Pensive |     No: Eyes look dazed; bad photo     |  No: Confused expression      |

**Cropping**                            | Yes: Appropriate cropping |    No: Popper looks beheaded      |       Yes: Appropriate cropping    |  

**Different sizes**                     | No: This logo only works at one size. If smaller, the word "Popper" is not readable. If larger, the mosaic of squares looks patchy and unpleasant |    Yes: Would look uniform at different sizes      |      Yes: Would look uniform at different sizes     |  

**Color scheme**                        | No: Does not work against a dark background |    No: Funeral photo      |    No: Funeral photo  |  

**Font**                                | No: Font color is too light |      No: Font looks too casual    |    No: Font looks too casual     |  

**Favicon**                             | No: Difficult to use for a favicon |   No: Difficult to use for a favicon   |   No: Difficult to use for a favicon     | 

<!---	<IMG SRC="https://github.com/liscovich/functional-specs/blob/master/images/popper_eyes.png?raw=true" width="100%" ALT="POPPER_EYES" ALIGN="RIGHT">
	</center>
-->

<!---logo images here-->

<a name="How_It_Works"></a>**How It Works** links to documentation for Popper. Documentation is stored on GitHub, not on the Researcher Site. Clicking on **How It Works** takes the Researcher to a public repository linked with the official [Popper GitHub account](https://github.com/Experiments/). We will take care of writing documentation.

**Our Story** is a static About page. Its contents will be discussed later.

**Experiments** is a dynamic page on the Popper Research Site that allows researchers to browse experiments, and will be discussed later.

Log In with GitHub and Sign Up were discussed in the previous section, Accounts. <!---internal link--> The Sign Up button disappears once the user is logged in. The Log In with GitHub button is replaced with the user's full name and a dropdown navigation bar that allows the user to view profile <!---link-->or log out.

**Dashboard** is visible only if the user is logged in.

##3. Header
<!---pic-->

The purpose of the **Header** is to describe Popper briefly. At the top of the Header is a tagline:

<c>
<center>
	Behavioral Experiments Platform, a(n) [adjective] one.
</center>
</c>

The <c>[adjective]</c> is replaced with a revolving list of serious and funny words. When the user arrives on the page for the first time, one of the serious adjectives is selected and displayed at random. If the user returns to the page again (as determined by cookies), a random word from either the funny or the serious list is displayed.

**Serious** 

- an agile
- a modern
- a versatile
- a cutting-edge
- a customizable
- an addictive
 
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

Underneath the tagline is a short paragraph describing Popper. 

> Popper is a powerful blend of modern technology and social science. With Popper, you can design complex cutting-edge experiments using the most advanced tools in existence. You can also run large-scale online trials drawing subjects from the world's deepest on-demand subject pool.

##4. Usage Statistics
<!---pic-->

Three summary statistics are dynamically updated and displayed under the <!---link-->Header:

1. The number of registered researchers
2. The number of deployed experiments
3. The number of completed trials

The numbers should be larger than the corresponding items being counted. We will start displaying these statistics only once Popper gains traction. At launch, the Introduction Page will not contain this statistics block.

##5. Overview
<!---pic-->

The **Overview** introduces the key features of the platform by walking users through a typical workflow:
<!---internal links-->

| Element                          | Text |  Image |  
----------------------------------- | :----------- | :------ |  
**Start at the Frontier**                |   Research frontier. Experiments. Replicate. Technology frontier.     |    <img src="https://github.com/liscovich/functional-specs/blob/master/images/comingsoon.png?raw=true" width="100px">   | 

**Program the Way You Think**     |      <!--rewrite-->Design experiments using intuitive visual programming. Popper comes equipped with domain-specific nodes, custom-tailored for behavioral experiments. Easily automate common experiment tasks using one of our templates. Popper features full Mathematica support for computationally-intensive functionality. Those with more programming experience can delve past visual programming into the C# code underlying all experiments.       |    <img src="https://github.com/liscovich/functional-specs/blob/master/images/comingsoon.png?raw=true" width="100px">     |  

**Run When You Are Ready**  |      Draw from our on-demand online subject pool. Without the physical restraints of a lab, subjects can participate from the comfort of their homes, when you need them to. Deploy experiments in minutes, without worrying about searching and coordinating eligible subjects.       |    <img src="https://github.com/liscovich/functional-specs/blob/master/images/comingsoon.png?raw=true" width="100px">     |  

**Leave Logistics to Us** |     Popper is built on a secure cloud infrastructure of servers, which means that you can focus on science rather than logistics. We handle all technical overhead related to subjects, from recruitment to screening to payment. We also provide an archive of IRB experiment-specific approvals for your convenience to expedite your own IRB approval process.       |    <img src="https://github.com/liscovich/functional-specs/blob/master/images/comingsoon.png?raw=true" width="100px">     |  

##6. Footer
<!---pic-->

The **Footer** features general links and legal documents.

- Our Story <!---internal link-->
- Blog: Hosted on a third-party site
- Twitter: @popper_exp
- Facebook: http://www.facebook.com/popper_exp
- Contact: The "Contact" section of <!---link-->About Us
- Documentation: Hosted on GitHub, as described above<!---link-->
- Terms of Service: Navigation Bar, text, and Footer<!---link-->
- Privacy & Security: Navigation Bar, text, and Footer<!---link-->

# <a name="RSOur_story"></a>Our story

**Our Story** introduces the history of the project and its connection to Karl Popper.
<!---pic-->

##Page Components

<!---internal lnks here-->
1. Navigation Bar 
2. Portrait of Karl Popper 
3. History
4. Team and Contributors
5. Footer

##1. Navigation Bar

Same as the Introduction Page. <!---link-->

##2. Portrait of Karl Popper

**Our Story** features a <a href="http://images.npg.org.uk/800_800/0/2/mw07802.jpg">photo</a> of Karl Popper taken by Lucinda Douglas-Menzies, cropped as necessary. 

<img src="https://github.com/liscovich/functional-specs/blob/master/images/popperlucinda.png?raw=true" width="100%">

Under the cropped photo should be the text, 

<c>"&copy; Lucinda Douglas-Menzies"</c> and <c>"Reproduced with the generous permission of the photographer"</c>. 

##3. History

We will provide the text for the History of the project when it is ready.

##4. Team and Contributors 

We will provide the text for the History of the project when it is ready.

##5. Footer

Same as the Introduction Page. <!---link-->

# <a name="RSExperiments"></a>Experiments

The **Experiments** page is a searchable library of all experiments available to the user on the Popper platform. Its overall interface resembles a <a href="http://www.amazon.com/s/ref=sr_nr_scat_3245219011_ln?rh=n%3A3245219011%2Ck%3Abarbie+doll&keywords=barbie+doll&ie=UTF8&qid=1343866475&scn=3245219011&h=220dc68f97ae40d6e3790975515ccea286922364" target="_blank">product list page</a> on Amazon.

##Page Components

<!---internal lnks here-->
1. Navigation Bar 
2. List of Experiments 
3. Search Bar
4. Filter
5. Footer

##1. Navigation Bar

Same as the Introduction Page.<!---link-->

##2. <a name="RSList_of_Experiments"></a>List of Experiments

The **Experiments** page displays a dynamically generated list of all available experiments from two sources:

- Public repositories from the central Popper GitHub account (github.com/experiments)
- Other GitHub repositories in the extended Popper network. This includes public GitHub repositories of *all* Popper users, and private repositories to which the user has access.

Naturally, if the user is not logged in, he or she cannot see any experiments hosted in private repositories. 

When the user first arrives at the **List of Experiments** and when the user conducts a search, his or her private repositories are listed first and sorted by the number of trials. All other experiments are listed afterwards and sorted by:

1. Growth rate in the number of commits
2. If tied, the number of forks
3. If tied, the number of upvotes
4. If tied, the age of the repository, with younger repositories listed first

A user would typically keep a repository private while the experiment is still being developed and then make the repository public once an accompanying paper has been published and the experiment is open for peer review and replication. 

The layout of the page is fluid so that the number of experiments displayed per row changes dynamically with the browser width. Each individual experiment listing contains the following information:

- Name of the repository (functioning as the name of the experiment)
- Repository owner
- Short description of the experiment
- Number of forks
- Publication citation
- Upvotes and names of recommenders
- Last modified ## minutes/hours/days/weeks/months/years ago

The Researcher Site obtaines this information for each experiment from the metadata in its respective GitHub repository. Repositories that lack the proper metadata, source code, or executable files, are not displayed.

The [Popper GitHub account](https://github.com/Experiments/) hosts Stock Experiments that showcase the capabilities of the platform and provide researchers with fully functional templates to start their own projects. 

An "Add Experiment" button links to Popper documention for designing and publishing an experiment using the Popper SDK.

The user clicks on the experiment to go to its <a href="RSCreate_Trial">Create Trial</a> page.

##5. Search bar

The search bar performs an instant search on the <a href="#RSList_of_Experiments">List of Experiments</a>. Suggestions appear beneath the Search bar as the user begins to type, similar to Google search. Search results are updated continuously to match the current state of the query even before the user hits "Return".

To perform instant search, the Researcher Site regularly indexes metadata from all experiment repositories. This specifically includes all text fields in the metadata, such as title, description, author, and documentation.

Search results are sorted by:

1. Growth rate in the number of commits
2. If tied, the number of forks
3. If tied, the number of upvotes
4. If tied, the age of the repository, with younger repositories listed first

<section class="sideimg">

<img src="https://github.com/liscovich/functional-specs/blob/master/images/Amazon_filter.png?raw=true" width="40%" align="right">

</section>

##6. Filter

Researchers can apply instant filters to the list of displayed experiments in the style of navigating with the left navigation bar to find a product on Amazon.com. 

###Available filters:

- Category 
	- Hierarchy of fields (based on information contained in experiment metadata)
- Author
	- Names of top 10 authors (checkboxes; by number of repositories as determined by experiment metadata)
- Status
	- Published (checkbox; indicates whether the metadata for an experiment lists an accepted peer-reviewed publication based on this experiment)
	- Hosted by Popper (checkbox; indicates whether experiment is in the Popper repository)

# <a name="RSDashboard"></a>Dashboard

The **Dashboard** is an overview of all activity in the user's account. It serves as the landing page for logged in users who come to the Researcher Site via <a href="http://www.popper.org" target="_blank">www.popper.org</a>.

##Page Components

<!---internal links here-->
1. Navigation bar
2. Trials
3. Feed
4. Footer

##1. Navigation bar

Same as the Introduction Page. <!---link-->

##2. Trials

**Trials** lists a user's ongoing and completed trials. Clicking on the name of a trial brings the researcher to its **Trial Summary**<!---link--> page.

Trials are sorted by timestamp. The state of a trial appears beneath its name, and a change in state updates its time stamp, pushing the trial to the top of the list.. These states can be altered in the metadata file but by default, trials are in one of six states:

1. **Awaiting subjects:** The initial status of all trials. The trial has been created and the server is waiting for a sufficient number of subjects. The researcher can recruit more subjects by clicking the name of the trial to go to its **Trial Summary** page. 
2. **In progress:** Sufficient subjects have joined and the trial has begun.
3. **Paused:** The researcher has paused the trial.
4. **Payment pending:** The trial has ended. The researcher reviews and approves subject payments on the **Trial Summary** page.
5. **Complete:** The researcher has paid subjects and may download data. 
6. **Error:** The researcher reviews errors on the **Trial Summary** page.

Also displayed: 

- **Trial number:** Unique ID number assigned to each trial.
- **Timestamp:** Time trial corresponding to a change in state.

Clicking “More...” scrolls down the window to display more trials in the style of GitHub. <!--- screenshot of GitHub more in action-->“More” disappears once all trials have been displayed. There is no scroll bar on the Trials frame.

“New Trial” links to the **Create Trial** page.

##3. Feed

The Feed automatically updates with:

1. Changes in status, with the following phrasing:
	- **Awaiting subjects:** `<a href=”trial-summary-url”>Trial ##</a> has been created. Awaiting subjects.`
    - **In progress:** `<a href=”trial-summary-url”>Trial ##</a> is now in progress.`
	- **Paused:** `<a href=”trial-summary-url”>Trial ##</a> has been paused.`
	- **Payment pending:** `<a href=”trial-summary-url”>Trial ##</a> has finished. Please <a href=”trial-summary-url”>review</a> subject payments.`
	- **Complete:** `<a href=”trial-summary-url”>Trial ##</a> is now complete.`
	- **Error:** `An error has occurred with <a href=”trial-summary-url”>Trial ##</a>.`
2. **Fork activity**
	- `<a href=”researcher-public-profile-url”>John Nash</a> has just forked your experiment, <a href=”experiment-url”>Experiment Name</a>.`
- **Following activity**
	- `<a href=”researcher-public-profile-url”>John Nash</a> is now following <a href=”trial-summary-url”>Trial ##</a>.`
	- `You are now following <a href=”trial-summary-url”>Trial ##</a> by <a href=”researcher-public-profile-url”>John Nash</a>.`

"More..." scrolls down the entire window to display more feed information.

##4. Footer 

The Footer is the same as the one described on previous pages. <!---internal link-->

# <a name="RSExperiment_Summary"></a>Experiment Summary

The Create Trial form includes the following fields:

- Parameters (experiment-specific; may differ according to the needs of each experiment)
	- Number of subjects
	- Cost of cooperation
	- Multiplier
	- Continuation probability
	- Initial endowment
	- Exchange rate (points to dollars)
- Frame (different visualizations of the game)
- Subjects 
	
Users create a metadata file to customize the Create Trial form for an experiment. They may specify:

- Default values for any field in the form 
- The exact Parameters, which may not be the same as in the example above

The Researcher Site uses the metadata file to look up the names of available frames and their accompanying screenshots.

The Subjects section accompanies all experiments. Available options, with the default values indicated, are as follows:

- Subject pool
	- Amazon MTurk (default)
	- oDesk
	- Own subjects (Selecting this option shows a direct link, below the “Subjects” field, to the game page on the Player Website. Researchers are responsible for communicating this link to subjects.)
- Gender
	- [X] Female
	- [X] Male
- Age
	- Slider beginning at age 13 and ending at age 100; the default slider selects ages 18 to 100
- Connection speed at least ## kbps (the researcher fills in the field with a number, with the default value at 256)
- Connection latency at most ## milliseconds (the researcher fills in the field with a number, with the default value at 700)
- [X] Make trial results public

# <a name="RSTrial_summary"></a>Trial Summary

Researchers monitor trials in real time and download results on the Trial Summary page.

##Page Components

1. Navigation bar
2. Trial information
3. Trial actions
4. Subjects
5. Report
6. History
7. Footer

##1. Navigation bar

See above. <!---internal link-->

##2. Trial information

- **Name of the experiment:** Link to the Create Trial page
- **Trial number:** Trials are numbered in the order that they are created

##3. Trial actions

- **Pause/Resume:** Suspend/resume the trial temporarily.
- **Stop:** End the trial manually; clicking this button opens a popup that asks,

	Are you sure you want to end this trial now? You will be responsible for any subject payments that have accumulated so far.

End trial (red button) 
	Never mind (grey button) 

- **Replicate:** Link to the Create Trial page, with all fields already filled in. The user can replicate the trial or change parameters.

##3. Subjects

Subjects is a table of all past and current subjects for the trial. The following stock parameters can be added to or changed in the experiment metadata. 

- **Player ID:** Link to the public player profile on the Player Website. For anonymity, a new Player ID is generated for each player per game. <!---internal link to player ID discussion-->
- **Status:** A player who has the game open in the player's current browser tab is <code>Active</code>. A player who navigates to a different browser tab is <code>Inactive</code>. A player who prematurely closes the browser tab to leave the trial has <code>Dropped out</code>.
- **Stage:** If there are multiple steps in the trial, the researcher can see how far each subject has progressed.
- **IP address:** The user can prevent cheating by checking whether multiple users are actually playing from the same IP address.
- **Location:** Based on the player’s IP address. 
- **Platform** Browser & Operating system
- **Earnings** How much the subject has earned so far in the trial.
- **Approved:** The researcher approves subject payments by clicking the checkbox next to a player's earnings. This option is not available until the trial ends or the researcher manually clicks "Stop" to end the trial.

##5. Report

The Report is a list of purely quantitative data in .csv, .xls, or .pdf format. Here are suggested types of data that users collect:

- Stage
- Player
- Choice: Can be a binary variable but does not have to be; its significance is specified by the user in the source code of the experiment and on the Experiment Parameters page
- Duration: The amount of time that it took for a player to make a particular choice
- Balance: A snapshot of the player's current points balance

##6. History

The History is a raw log of all events in the game. Its content depends on experiment metadata. At minimum, History includes the initial parameters of the game, a list of subjects, and a list of all in-game events with timestamps. 

# <a name="RSProfile"></a>Profile

Each user has a public profile to showcase his or her work in the experimental social sciences on Popper.
	
##Page Components

1. Navigation bar
2. Researcher profile
3. Footer

##1. Navigation bar

See above. <!---internal link-->

##2. Researcher profile (replaced with the researcher’s name)

The profile features information pulled from the user’s GitHub account as well as user-provided information. The public view of a user’s profile displays the following:

- GitHub profile picture (Gravatar)
- Full Name
- Department
- Affiliation
- Experiments
- Trials

A logged-in user can edit the above fields and see the following private information:

- Payment credentials

##3. Footer 

See above. <!---internal link-->

# <a name="RSSearch"></a>Search Results

Users can perform an instant search for an experiment, trial, or researcher profile from any page on the Researcher Website.

## Page Components

<!---internal lnks here-->
1. Navigation Bar 
2. Search Results 
3. Footer

## 1. Navigation Bar

See above.

##2. Search Results 

Suggestions appear beneath the Search bar as the user begins to type, similar to Google search. Search results are updated continuously to match the current state of the query. 

###Indexing

To perform instant search, the Researcher Site regularly indexes the following information:

- Experiments
	- All experiment repositories: All text fields in the metadata, such as title, description, author, and documentation.
	- All ongoing and completed trials.
	- All researcher profiles.
- Trials (indexed from the Trial Summary page for each trial)
	- Trial information 
	- Trial parameters and researcher comments from the Trial History section
- Profiles
	- Full Name
	- Department
	- Affiliation
	- Names of the user’s pushed experiments
	- Categories assigned to the user’s pushed experiments
	- Names of the user’s created trials

All three results sections (experiments, trials, and profiles) are displayed with every query. If no result exists for a particular results section, the message “No results found” is displayed. Clicking “More...” opens a new page with search results from only that category. The same “More...” functionality <a href=”https://github.com/search?q=rails&type=Everything&repo=&langOverride=&start_value=1” target=”_blank”>can be found</a> in GitHub search. 

###Sorting

Experiments search results are sorted by:

1. Growth rate in the number of commits
2. If tied, the number of forks
3. If tied, the number of upvotes
4. If tied, the age of the repository, with younger repositories listed first

Trials search results are sorted by:

1. Last activity date
2. If tied, number of times search word(s) appear in 

Profile search results are sorted by

1. Appearance in the user’s name:
	- Alphabetically by last name
	- If tied, by number of experiments committed
	- If tied, by number of trials created
	- If tied, by date account was created
2. If the search term does not appear in the user’s name:
	- Appearance in names of pushed experiments
	- If tied, by appearance in names of trials created
	- If tied, by appearance in the researcher’s self summary

##3. Footer

See above.

<h1> <a name="Player_Site"></a>Player Site </h1>

Players (subjects) play games on the Popper Player Website to contribute to social science research. Most social science experiments are currently run in social science laboratories, where players type information into a screen like the following.

<!---z-tree screenshot-->
# <a name="PSAudience"></a>Audience

Researchers recruit subjects from three sources: 

1. Online labor markets, like [Amazon Mechanical Turk](https://www.mturk.com/mturk/welcome) and [oDesk](www.odesk.com).
2. Their own subject pools.
3. Visitors who independently come to the Popper Player Site.

# <a name="PSAccounts"></a>Accounts

All players must have an account to play games on the Popper Player Website, since demographic information about the player, like age and sex, are usually necessary for the researcher to interpret results. Players cannot be anonymous. On the same token, player confidentiality is important and researchers should not know all information about their subjects. Player privacy, especially their names, should be protected so that players feel that they are making decisions in the game safely without the risk of stigma or judgment. For example, a player who chooses to "betray" other players in a game should be able to do so without worrying that the researcher or other players would be able to identify them in real life. 

## Log In

The landing page of the Popper Player Website is a Log In page. Players should not be able to see games unless they log in with a verified Popper account. <!--- internal link-->

Players must log in by using their Facebook account. We want to make sure that demographic information associated with each player is as accurate as possible, which is easier if the player logs in using an account linked with his real identity. Logging in with a Facebook account also reduces the amount of demographic information that the player has to provide manually, since the Player Site can pull the player's name, age, and sex from the player's Facebook account. The player is notified with a message on the Log In page that his individual choices in a game (for example, defection or cooperation) will never be publicized. This assurance is necessary so that the player does not alter his behavior based on the possibility that his friends will see how he played certain games.

We are considering making the background of the Log In page a blurry version of the Lobby, to give players an idea of what lies in the Player Website.

## Sign Up

The player is taken through the standard Facebook authorization process, and must allow Popper to post messages on the player's timeline saying that the player just played game XYZ. If the Player Website is unable to pull certain information from the player's Facebook page, the player sees a final screen, which asks the player to provide an age and sex so that the player is served a list of games that match the player's demographics. Other more detailed information is solicited from games on an as-needed basis, before the player begins the game.

Like the Log In page, the Sign Up page should feature the same blurry version of the Lobby.

# <a name="PSLobby"></a>Lobby

The lobby is a dynamic gallery of every game that fits a player's demographic information. It features two types of games: non-paying and paying. Non-paying games are two stock games that we hope to develop, that attract and retain a core group of players. The purpose of non-paying games is to provide players with an available game even when no trials are running. At least initially, we anticipate that the Player Site will not feature a paying game 24/7. Hosting two 24/7 games thus appeals to the third type of subject mentioned above, those who independently come to the Player Site. 

Players see the following information about each game:

- Payoff range
- Brief description, provided by the researcher
- Number of participants
- Time stamp of when the trial was initiated
- A button to play the game

When the player clicks the play button, the Player Site checks whether the player's available demographic information matches what the researcher is looking for and asks the player to enter any additional demographic information that the researcher needs. These answers are then stored in the user's account and cannot be manually altered by the player. If the player's information does not match what the researcher is seeking, the player is alerted that he does not qualify for the game. We would like to minimize how often players see this message. As a player fills out more questionnaires prior to playing a game, more information will be gathered about the player and unsuitable games will not be displayed to the player in the first place. 
If the player selects a paying game but has not entered payment information (in order to get paid), the player is redirected to the Profile, where he can enter information to link his Popper account with his PayPal, Amazon Mechanical Turk, or oDesk account.

# <a name="PSGame"></a>Game

The game page is an imbedded iframe featuring the client, which is designed by the researcher.

# <a name="PSProfile"></a>Profile

The player profile features the individual's name and payment information. Details like age and sex cannot be altered once the player has provided it or once it has been pulled from Facebook. In order to get paid, a player can enter his PayPal, Amazon Mechanical Turk, or oDesk information. 

# <a name="PSAbout"></a>About

The About page is static and features a description of the Player Site and how players contribute to social science research by playing games. 