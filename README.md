<h1 align="center">
    Workshop - Web Scraping with Python - Part 2
</h1>

<p align="center">
    <img width="250" height="250" src="https://cdn4.iconfinder.com/data/icons/emoji-2-5/64/_robot_emoticons_smiley-512.png">
</p>
<br>

<h3 align="center">
    The objective of this workshop is to create <br> a bot to play a game for us
</h3>
<br><br>

### **What's a scrap?**
Scraping is the action of collecting source code of a web page, with a program.
<br><br>

# **Before this workshop**

In the previous workshop, we saw how to make a dynamic dictionary using 
the Larousse's website.
<br><br>
We also took a look to different ways to protect a website against webscraping. <br>
So today we are going to see how to pass through these protections. :wink: <br>
More precisely how to pass through dynamic website (website using javascript for html generation).
<br><br>

# **Objective of this workshop**
In this workshop, we are going to make a bot that play a game called "SimpleMMO" for us.
<br><br>

# **Something you need to be aware of !**

<p align="center">
    <img width="100" height="100" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f6/OOjs_UI_icon_alert-destructive.svg/1024px-OOjs_UI_icon_alert-destructive.svg.png">
</p>
<br>
The use of scripts is forbidden on this website.<br>
This topic is for educational purposes, we are not responsible for the use you make of it.<br>

For this workshop you will have to create an account and delete it at the end of the workshop.<br>
If you are detected by the anticheat, your account will be banned.<br>

<br>

# **Prerequisite**

For this workshop we are going to use Selenium, a python testing library.
To install Selenium, use the following command.
> pip install selenium

# **Get started**

## **Exercise 1 - Set the webdriver**

As we are going to load javascript, we need a web driver.<br>
1- Go inside your python script, set a webdriver using selenium.<br>
2- Get the following page
> https://web.simple-mmo.com

<br>

## **Exercise 2 - Cookies**

This website uses cookies to auto connect the user.<br>
So lets connect your account automatically:<br>
1- Save your cookie inside a Json<br>
> To get your cookie use selenium
2- Add cookies to the webdriver<br>
3- Get the following webpage
> https://web.simple-mmo.com/travel

4- After the end of the program save all cookies which are generated during the process inside your Json

<br>

## **Exercise 3 - Stepping**

Now, we are connected to the website, on the main game page, so let's start our bot.<br>
Now we can see a button with `Step` as content, it's the main game button.<br>
1- Using class `By` created by selenium, find the button element.<br>
The class `By` can be used like:
```python
from selenium.webdriver.common.by import By
...
elem = browser.find_element(By.XPATH, ...)
...
```
> By contain different type of searching like XPATH, CSSSelector, id, etc etc

2- Click on this object<br>
3- Use `random` and `time sleep`, to create a bot thats looks more like a human player.<br>

<br>

## **Exercise 4 - Fight**

In this game, sometimes there are different type of action such as: story, fight ect.. As we are handling story, let's try "fight" interaction.<br>
1- Reproduce stepping part, but adapted for the fighting mode<br>
2- When we click on this button another page is loading, so you need to make your code do the same.<br>
> Your type of action need to be based on the content of the actual webpage
3- Make your bot click on the attack button<br>

<br>

## **Exercise 5 - Optimize**
In this game there are a lot of different types of actions, so add actions to your bot to be more efficient and get rich.

<br>

# **To go further**
Now that you have the basics to make dynamic webscraper, here some ideas to improve your skills:
- Bypass the anti-cheat
- Try more dynamic website (like agar.io)
