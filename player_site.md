latex input:		mmd-article-header  
Title:				Sample MultiMarkdown Document  
Base Header Level:	2  
latex mode:			memoir  
Keywords:			MultiMarkdown, Markdown, XML, XHTML, XSLT, PDF   
CSS:				fspecs.css	
xhtml header:		<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
copyright:			2012 Popper  
latex input:		mmd-natbib-plain
latex input:		mmd-article-begin-doc  
latex footer:		mmd-memoir-footer  

<h1> <a name="Player_Site">Player Site</a> </h1>

Players (subjects) play games on the Popper Player Website to contribute to social science research. Most social science experiments are currently run in social science laboratories, where players type information into a screen like the following.

<!---z-tree screenshot-->
# <a name="Audience">Audience</a>

Researchers recruit subjects from three sources: 

1. Online labor markets, like [Amazon Mechanical Turk](https://www.mturk.com/mturk/welcome) and [oDesk](www.odesk.com).
2. Their own subject pools.
3. Visitors who independently come to the Popper Player Site.

# <a name="Accounts">Accounts</a>

All players must have an account to play games on the Popper Player Website, since demographic information about the player, like age and sex, are usually necessary for the researcher to interpret results. Players cannot be anonymous. On the same token, player confidentiality is important and researchers should not know all information about their subjects. Player privacy, especially their names, should be protected so that players feel that they are making decisions in the game safely without the risk of stigma or judgment. For example, a player who chooses to "betray" other players in a game should be able to do so without worrying that the researcher or other players would be able to identify them in real life. 

## Log In

The landing page of the Popper Player Website is a Log In page. Players should not be able to see games unless they log in with a verified Popper account. <!--- internal link-->

Players must log in by using their Facebook account. We want to make sure that demographic information associated with each player is as accurate as possible, which is easier if the player logs in using an account linked with his real identity. Logging in with a Facebook account also reduces the amount of demographic information that the player has to provide manually, since the Player Site can pull the player's name, age, and sex from the player's Facebook account. The player is notified with a message on the Log In page that his individual choices in a game (for example, defection or cooperation) will never be publicized. This assurance is necessary so that the player does not alter his behavior based on the possibility that his friends will see how he played certain games.

We are considering making the background of the Log In page a blurry version of the Lobby, to give players an idea of what lies in the Player Website.

## Sign Up

The player is taken through the standard Facebook authorization process, and must allow Popper to post messages on the player's timeline saying that the player just played game XYZ. If the Player Website is unable to pull certain information from the player's Facebook page, the player sees a final screen, which asks the player to provide an age and sex so that the player is served a list of games that match the player's demographics. Other more detailed information is solicited from games on an as-needed basis, before the player begins the game.

Like the Log In page, the Sign Up page should feature the same blurry version of the Lobby.

# <a name="Lobby">Lobby</a>

The lobby is a dynamic gallery of every game that fits a player's demographic information. It features two types of games: non-paying and paying. Non-paying games are two stock games that we hope to develop, that attract and retain a core group of players. The purpose of non-paying games is to provide players with an available game even when no trials are running. At least initially, we anticipate that the Player Site will not feature a paying game 24/7. Hosting two 24/7 games thus appeals to the third type of subject mentioned above, those who independently come to the Player Site. 

Players see the following information about each game:

- Payoff range
- Brief description, provided by the researcher
- Number of participants
- Time stamp of when the trial was initiated
- A button to play the game

When the player clicks the play button, the Player Site checks whether the player's available demographic information matches what the researcher is looking for and asks the player to enter any additional demographic information that the researcher needs. These answers are then stored in the user's account and cannot be manually altered by the player. If the player's information does not match what the researcher is seeking, the player is alerted that he does not qualify for the game. We would like to minimize how often players see this message. As a player fills out more questionnaires prior to playing a game, more information will be gathered about the player and unsuitable games will not be displayed to the player in the first place. 
If the player selects a paying game but has not entered payment information (in order to get paid), the player is redirected to the Profile, where he can enter information to link his Popper account with his PayPal, Amazon Mechanical Turk, or oDesk account.

# <a name="Game">Game</a>

The game page is an imbedded iframe featuring the client, which is designed by the researcher.

# <a name="Profile">Profile</a>

The player profile features the individual's name and payment information. Details like age and sex cannot be altered once the player has provided it or once it has been pulled from Facebook. In order to get paid, a player can enter his PayPal, Amazon Mechanical Turk, or oDesk information. 

# <a name="About">About</a>

The About page is static and features a description of the Player Site and how players contribute to social science research by playing games. 