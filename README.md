<h1 align="center">
    Workshop - Scrapping Web Python - Part 2
</h1>

<p align="center">
    <img width="250" height="250" src="https://cdn4.iconfinder.com/data/icons/emoji-2-5/64/_robot_emoticons_smiley-512.png">
</p>
<br>

<h3 align="center">
    The objective of this workshop is to create <br> a bot for a game
</h3>
<br><br>

# **Before**

In the previous workshop, we saw how to make a dynamic dictionary using 
the Larousse's website.
<br><br>
We also shortly saw a different way to protect a website against webscrapping. <br>
So today we are going to see how to pass through these protections. :wink: <br>
More precisely how to pass through dynamic website (website using javascript for html generation).
<br><br>

# **Objectif of this workshop**
In this workshop, we are going to make a bot that plays for us at SimpleMMO.
<br><br>

# **Prevention**

<p align="center">
    <img width="100" height="100" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f6/OOjs_UI_icon_alert-destructive.svg/1024px-OOjs_UI_icon_alert-destructive.svg.png">
</p>
<br>
The site does not accept the use of scripts.<br>
This topic is for educational purposes, we are not responsible for the use you make of it.<br>

For this workshop you will have to create an account and delete it at the end of the workshop.<br>
If you are detected by the anticheat, your account will be banned.<br>

<br>

# **Prerequisite**

For this workshop we are going to use Selenium, a python testing library.
Install Selenium.
> pip install selenium

# **Get started**

## **Exo1 - Set the webdriver**

Like we are going to load javascript, we need a web driver.<br>
1- So inside your python script, set a webdriver using selenium.<br>
2- Get the following page
> https://web.simple-mmo.com

<br>

## **Exo2 - Cookies**

This website use cookie to auto connect the user.<br>
So let's connect automatically an account:<br>
1- Save your cookie inside a Json<br>
2- Add cookies to the webdriver<br>
3- Get the following webpage
> https://web.simple-mmo.com/travel

4- After the end of the program save all cookies which are generated during the process inside your Json

<br>

## **Exo3 - Stepping**

Currently, we are connected to the website on the main playing page, so let's start our bot.<br>
Currently we saw a button with `Step` as content, it's the main playing button.<br>
1- Using class `By` creating by selenium, find the button element.<br>
2- Click on this object<br>
3- Use random and time sleep, to create a bot looking more like a player.<br>

<br>

## **Exo4 - Fight**

In this game, sometime there are different type of action: story, fight and different type of action. Currently we handling story, so let's try fight interaction.<br>
1- Reproduce stepping part, but adapted to fighting mode<br>
2- When we click on this button another page is loading, so you need to adapt your code to be compatible.<br>
3- Use the bot to click on the attack button<br>

<br>

## **Exo5 - Optimisation**
In this game there is a lot of different types of action, so add action to your bot to be more efficient.

<br>

# **To go further**
Now that you have the basis to make dynamic webscraper, here some ideas to improve your skills:
- Bypass the anti-cheat
- Try more dynamic website (like agar.io)
