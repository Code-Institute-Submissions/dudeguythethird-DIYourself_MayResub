# DIYourself - A DIY sharing platform.

![image of project across various devices](static/assets/images/testing/diyourself-responsive.png)

## Contents

  * [UX](#ux)
    + [User 1 (DIY fan, new to site)](#user-1--diy-fan--new-to-site-)
    + [User 2 (DIY fan, returning)](#user-2--diy-fan--returning-)
    + [User 3 (Developer)](#user-3--developer-)
  * [Theming](#theming)
    + [Color Palette](#color-palette)
    + [Fonts](#fonts)
    + [Theme Images](#theme-images)
  * [Features](#features)
    + [Features Left to Implement](#features-left-to-implement)
  * [Technologies Used](#technologies-used)
  * [Testing](#testing)
  * [Database Structure](#database-structure)
  * [Bugs](#bugs)
  * [Deployment](#deployment)
    + [How to run this project locally](#how-to-run-this-project-locally)
    + [Cloning this project](#cloning-this-project)
    + [Deploy this Project](#deploy-this-project)
  * [Credits](#credits)
    + [Content](#content)
    + [Media](#media)
    + [Acknowledgements](#acknowledgements)

[DIYourself](https://diy-sharing-site.herokuapp.com/) is a site that allows its users to create formatted DIY method guides and share them with other practical people. Users make accounts that allow them to create, edit and delete DIY guides. All guides are viewable by all users, that includes those who do not yet have an account. Users with accounts may only edit and delete their own guides. Included in each method is an optional field that allows users to include a link to a video for their guide, should one exist.The goal of this project is to create a space for practical people of all kinds to share their personal techniques, or to share and amplify the work of others. In this sense, I think it serves a real life function as it could become a useful resource for homeowners, renters, or anyone looking to try out a fun project.
 
## UX

The UX for this site is being driven by three main considerations:

1. Functionality: the site must perform as outlined above.
1. Simplicity: the site must perform this functionality in as straightforward a manner as possible.
1. Theme: the site must achieve the first two considerations while also being appropriately thematized around DIY, making things, and practical self-sufficiency.
 
These considerations are ranked in importance already, ie. 1 is most important and 3 is the least, though I do not think that many sacrifices will need to be made to the less important consideration of theme. The majority of what consideration 3 demands, I think, can be achieved through colour, font, and image choice. 1 and 2, on the other hand, inform the structure of information directly. 

In order to meet these requirements, I have decided on a layout that looks roughly as belown (displayed are wireframes for the desktop site, wireframes for the tablet and phone experiences are available in assets/images/wireframes):

![image of homepage wireframe on desktop](/static/assets/images/wireframes/homepage-desktop.png)

![image of login page wireframe on desktop](/static/assets/images/wireframes/login-desktop.png)

![image of method form wireframe on desktop](/static/assets/images/wireframes/method-form-desktop.png)

![image of profile wireframe on desktop](/static/assets/images/wireframes/profile-desktop.png)

![image of project wireframe on desktop](/static/assets/images/wireframes/project-desktop.png)

![image of signup wireframe on desktop](/static/assets/images/wireframes/signup-desktop.png)

As you can see, the homepage consists simply of a list of DIY methods each with an expandable description, a search bar,  and an image that conveys something about the theme. If a user wishes to view the method in its entirety, they may click the ???Learn More??? button (I may change the text here to something more direct like ???View Method???). Clicking view method takes you to a method page which will be different depending on whether the user viewing the page is logged in as the method???s author. If they are, then it will look as depicted, as they are permitted to edit and delete said method. Otherwise, these buttons will not be displayed. 

There are also log in and sign up pages that I think are very self explanatory. 

To help explain why I think the above layout is appropriate for this project I will outline some potential user stories to show how my UX meets their needs.

### User 1 (DIY fan, new to site)

I am looking for a site to help me find new DIY methods to help me upholster a chair. I navigate to DIYourself and notice a list of various method guides on the home page. I spot the search bar and try searching for ???chair???, this produces a tailored list of results and one of them looks like it might tell me what I need to know. I click ???Learn More??? and peruse the method. I decided to give it a go myself. It works well but during the time I spend upholstering the chair, an idea occurs to me for a new DIY method, inspired by the one I tried. 

I return to DIYourself and click the button in the header to create a new method. The site prompts me to create a new account, so I go through the account creation process and then navigate back to the method creation form. I write out the steps to my method using the easy to follow form and then click publish. 

### User 2 (DIY fan, returning)

I have made a post on DIYourself but I want to edit it. I return to the website and navigate to the ???My Profile??? section (from the nav bar) where the posts that I have made are stored. I find the one I am looking for and click ???View Method???, then ???Edit???. I use the form to make the edits that I need to, it looks just like the method creation form except that its fields are prefilled with the data that I put there for my initial method.

### User 3 (Developer)

I am a developer who is on DIYourself either randomly or because they want to check out Joseph Keable???s work. I try making an account, making a method, and decide that I want to contact the developer of the site (Joseph Keable). To do so I can scroll to the bottom of any page and use the social media links found there to contact the site???s developer.

## Theming

In order to achieve a ???DIY feel??? for my site, I will be using a carefully selected combination of images, colours, and fonts. Below are some samples of each that are intended to convey a sense of where I would like to go thematically. They are not my final choices! The live website may vary from what is shown, though I think the vibe will be the same. 

### Color Palette

![image of brown and red colour palette](/static/assets/images/color/colour-pallete1.png)

![image of brown and red colour palette](/static/assets/images/color/colour-pallete2.png)

### Fonts

![image of rustic font sample](/static/assets/images/fonts/font1.png)

![image of rustic font sample](/static/assets/images/fonts/font2.png)

### Theme Images 

![image of woodworking tools](/static/assets/images/theming/woodwork-tools-min.jpg)

![image of woodworking tools](/static/assets/images/theming/woodwork-tools2-min.jpg)

![image of a guitar](/static/assets/images/theming/guitar-min.jpg)

![image of christmas decorations](/static/assets/images/theming/christmas-min.jpg)

![image of candles being made](/static/assets/images/theming/candles-min.jpg)

![image of woodworking tools](/static/assets/images/theming/woodwork-tools3-min.jpg)

## Features

1. Site-wide:
    1. A header: This element allows users to navigate around the site. By default it contains a title, a subtitle and three buttons. The buttons: log in, create a new account, and create a new method (if you are not logged on, this simply prompts you to create an account). If you are logged in, the ???create account??? and login buttons are replaced by a logout button and a ???my profile??? button. 
    2. A footer: This element allows users to view basic copyright information about the site and contains links to the developers social media, so that they can contact said developer if wanted
1. Homepage:
    1. A search bar: this allows you to filter the site???s DIY methods by keywords.
    2. A dynamic list of the site???s methods: each method has a description as well as a button link to its own method page. This allows users to peruse methods in search of something interesting. 
1. DIY Method page:
    1. Contents of the method page fill out dynamically based on the method that it is for.
    2. ???Edit??? and ???Delete??? buttons are available for the author of the method only. 
1. Create DIY method page:
    1. This contains a form where users can fill out the details of their DIY method. The form contains fields for: Method Title (Text, Required), Method type (Text, Dropdown, Required), a video link (Text, Link Format, Optional) and Step 1 (Text, Required). It also has a button that allows users to add additional steps (which are all optional). 
1. Edit DIY method page:
    1. The same as the create page, except the form has been filled in with the details of your existing post. 
1. Sign up page:
    1. This contains a form for new users to register to the site. They must provide an alphanumeric username and password with no special characters between 5 and 25 characters long. The password must be confirmed to register. This helps prevent users creating an account with the wrong password by accident. 
    2. There is also a link directing users to log in, if they already have an account. 
1. Login page:
    1. This is the same as the sign up page except it is for existing users. Therefore the form contains no ???Confirm Password??? field.
    2. The form also instead prompts users to sign up if they have not yet done so. 
1. Profile Page:
    1. This page contains all of a user???s posts to the site.
    2. Also contains options to add, edit, and delete categories, if the logged in user is an admin. Admin status is determined with the boolean field ???is_admin??? in the user objects within the project???s database. It is not possible to alter the value of this through the site itself, you have to change it manually in the database on mongoDB. By default, the value of ???is_admin??? for newly created accounts is ???false???. This prevents users from granting themselves admin rights.

### Features Left to Implement
- Comments section + ability to reply to comments.
- Ability to upvote and downvote comments and posts
- Custom images for different methods (on a type by type basis).

## Technologies Used

*   HTML5
    *   This project uses **HTML5** to provide structure and content to the site.
*   CSS3
    *   This project uses **CSS3** to provide styling, layout and basic interactivity to the structure and content defined by HTML5.
*   JavaScript
    *   This project uses **JavaScript** to provide it with interactivity as well as editing the functionality provided by Materialize.
*   Python
    *   This project uses **Python** to determine the logic of database interactions for the site and to manipulate that data in useful ways.
*   [Materialize](https://materializecss.com/)
    *   This project uses Materialize to simplify and speed up the process of creating an attractive and intuitive front end. It provides access to boilerplate code for various elements on the sight like the nav bar, footer, and form input elements.
*   [Google Fonts](https://fonts.google.com/)
    *   This project uses **Google Fonts** to allow the adding of more interesting fonts to the project.
*   [Font Awesome](https://fontawesome.com/)
    *   This project uses **Font Awesome** to allow the inclusion of icons. 
*   [MongoDB](https://www.mongodb.com/)
    *   This project uses **MongoDB** to host a database that stores all the data that the site uses (user data, project data, and category data)
*   [Flask](https://flask.palletsprojects.com/en/1.1.x/)
    *   This project uses **Flask**, to determine how the project is built by the browser, incorporating data from the database.
*   [Werkzeug](https://werkzeug.palletsprojects.com/en/1.0.x/)
    *   This project uses **Werkzeug** to provide an easy way to hash and salt passwords before storing them in the database.


## Testing

The testing information for this project is viewable in this [document](https://github.com/dudeguythethird/DIYourself/blob/master/TESTING.md).

## Database Structure

This site's database contains the following tables:

* categories - This is a collection of all the categories of DIY method that are available on the site. Each row, or category, consists of two pieces of information: "category_name" and a unique, automatically created "_id". Only administrators can create, edit, or delete these fields.

* methods - This is a collection of all the methods currently on the site. Each row, or method contains 7 pieces of information: a unique "_id", "method_name", "category_name", "method_description", "method_video", "method_steps", and "created_by". "_id" is automatically created. The only optional field is "method_video", which if not filled out, will be populated by a blank string. Any user can create, edit and delete methods. However, they can only edit and delete methods they have created. Admins can delete any method.

* users - This is a collection of all of the site's users. Each row, or user, consists of 4 pieces of information: a unique, automatically created "_id", a "username", a hashed and salted "password", and a boolean "is_admin". By default, "is_admin" is false, this can only be changed about a user from inside the database. Users can be created by any site user. They can only be edited or removed from inside the database.

## Bugs

1. Bug discovered where form validation for confirm password stopped working on sign up page. 
    - This bug was caused by non-functional onclick and onkeyup event handlers which I improved. The code is now as bellow:

    ```javascript
    if (window.location.pathname == '/sign_up') {
    var password = document.getElementById("password")
        , confirm_password = document.getElementById("password_confirm");

    function validatePassword() {
        if (password.value != confirm_password.value) {
            confirm_password.setCustomValidity("Passwords Don't Match");
        } else {
            confirm_password.setCustomValidity('');
        }
    }

    $("#password").change(validatePassword);
    $("#password_confirm").keyup(validatePassword);
    }
    ```

1. Bug discovered where method page does not immediately update after editing, requires reload.
    - Bug squashed by using `return redirect(url_for('method', method_id=method_id))` to redirect to the method page after method editing is complete. This takes new changes into account.

1. Bug discovered where profile page for admins does not 
immediately update after adding a new category. (suspect cause is same as last bug)
    - Bug squashed by using `return redirect(url_for('profile', username=session['user']))` to redirect to the profile page after category editing is complete. This takes new changes into account.
    
1. Bug discovered where " appears at the end of method description strings when read from the DB.
    - Bug squashed by removing a rogue close quote from edit_method.html.

1. Bug discovered where users who are not logged into an account were unable to view method pages. This was caused by the app.py code for rendering the page assuming the existence of a session user. If one were not present, the page is unable to load as it is trying to call a variable that doesn't exist.
    - Fixed with a simple `if session:...`

1. Bug discovered where form validation for signing up was not working properly. The ???pattern??? attribute was not working on the form's input elements, meaning usernames and passwords with special characters or spaces within them were not being stopped. 
   - This bug was caused by an error in the value of the ???pattern??? attribute of the forms input elements. The part where the acceptable length of the input was specified ???{5,15}??? was originally coded ???{5-15}???. Consequently, the whole Regex was not recognised. This has been corrected.

1. Bug discovered where no new methods could be uploaded to the site. 
    - This bug was being caused by a syntax error in the backend validity check function I added. Basically, this line: 
    ```Python
    if not method_name or not method_description or not method_steps:
        return False
    ```
    - Was initially this:
    ```Python
    if not method_name or method_description or method_steps:
        return False
    ```
    - This caused the function to always return `False`, as users rightly included descriptions and steps for their methods. I think the cause of this error was an earlier version of the function that included brackets after the initial `not`. Regardless, it is now fixed.

1. Various bugs discovered around site security/ user verification. In short, users were able to access pages that they were not supposed to. This includes non-registered users being able to access the "add method" page through the url, signed-in users accessing the sign up and login pages in the same way, as well various admin only pages being accessible in this way also.
    - These bugs were fixed with a variety of `if` checks to determine if the user was logged in, as well as a custom check for admin status below:
    ```python
    def is_admin():
    if not session:
        return False
    if session['user'] == os.environ.get('ADMIN_ONE'):
        return True
    if session['user'] == os.environ.get('ADMIN_TWO'):
        return True
    return False
    ```

1. Bug discovered where both the "Incorrect Username and/or Password" and "You are already logged in" messages display when a user tries to log into their account but provides incorrect information.
    - This bug was being caused by `if` checks for having an incorrect password or not having an account in the database resdirecting users through the `login` function. This would cause the initial `if` check in that function (`if request.method == "POST":`) to fail, causing the non post part of the function to run. However, because there is now something stored in session (that being incorrect account information), the part of the function that ran was for already logged in users. This is what caused the display of the message "You are already logged in". 
    - This bug was solved by having the incorrect password and no account `if` checks redirect users through the `get_methods` function, taking them back to the home screen and showing only the correct message.

1. Bug discovered where youtube links got from clicking the "share" button would not properly embed on method pages. 
    - Bug fixed by adding a new `if` check to my `generate_embed_link_from_youtube_link` function, it is below:
    ```python
    videoUrl = yt_link
    share = "tu.be/"
    if share in videoUrl:
        videoUrl = videoUrl.replace(share, "tube.com/embed/")
    return videoUrl
    ```


## Deployment

This project is deployed on Heroku through my GitHub Account. In order to do this I needed both GitHub and Heroku profile. The GitHub profile is used to store the code for the project (to create a local copy of the code and do this yourself with this code, see below). I also am using MongoDB to host my site???s database. This needs a separate account also.

### How to run this project locally
 
1. Create a [GitHub](https://github.com/) account.
1. Using Chrome, install the gitpod [browser extension](https://www.gitpod.io/docs/browser-extension/).
1. Restart the browser after installation.
1. Log in to GitPod with your GitHub account.
1. Go to the project [repository](https://github.com/dudeguythethird/DIYourself) on GitHub.
1. Click the green git pod button, this will trigger a new workspace to be created in GitPod with the project in it.
1. You must install the project requirements by typing ???pip3 install requirements.txt??? in the command line.
1. If you want to do further development on this project and run preview in the browser, through GitPod, you will need to create an env.py file in the project. This will need to be formatted as follows:

```python
import os

os.environ.setdefault("KEY", ???VALUE???)
```
You will need an instance of the line ???os.environ.setdefault("KEY", ???VALUE???)??? for each key value pair. The details of which are below in the ???Deploy this Project??? section You should also make sure that you add the env.py file to a .gitignore file so that it is not uploaded to your public GitHub. This would effectively give the world access to your private database.

 
### Cloning this project
 
Want to make some changes to this project and develop on your own version?
 
1. Got to this GitHub [repository](https://github.com/dudeguythethird/DIYourself).
1. Under the name, click the ???code??? drop down, then clone or download.
1. Copy the URL in the HTTPS section.
1. Go to your local IDE and open the terminal.
1. Navigate to the folder you would like to clone the code in.
1. Type ???git clone ??? then paste the URL you copied in step 3.
1. Press enter!
1. Make sure you install all the requirements detailed in requirements.txt and set up your env.py file. How to do this in GitPod is detailed above.

### Deploy this Project

1. On your local version, you should already have a requirements.txt file, if you are working from my project and haven???t added any new requirements. If not use `pip freeze > requirements.txt`, in the command line, to create one that is up to date for your version of the project.
1. My project files should also come with a Procfile that is appropriate for my version of the project. If you need to create a new one use `echo web: python app.py > Procfile`
1. Create a new app on [Heroku](https://dashboard.heroku.com/) (You will need an account). Press ???new??? on the dashboard and select app. Give it an appropriate name and set the region to your nearest.
1. From your new app???s dashboard, go to the deploy tab and select the deployment method of GitHub. 
1. Select and confirm the correct GitHub repository.
1. Go the Settings tab and click reveal config vars, set the following config vars:

Key | Value
----- | -------
IP | 0.0.0.0
MONGO_DBNAME | <your database???s name>
MONGO_URI | mongodb+srv://<username>:<password>@<cluster_name>.ammug.mongodb.net/<databse_name>?retryWrites=true&w=majority
PORT | 5000
SECRET_KEY | <your secret key (a string you decide on yourself)>

Please refer to mongoDB???s documentation for more information about MONGO_URI [formatting](https://docs.atlas.mongodb.com/).

7. Click ???Deploy???.
1. Back in the ???Deploy??? tab, go to the ???Manual Deployment??? section and make sure the master branch is selected. Click ???Deploy Branch???

Following these steps there will be no differences between deployed and development versions.


## Credits

* This taught me how to import datetime and use that data in my project: https://www.programiz.com/python-programming/datetime/current-datetime
* This alerted me to the ability to reverse lists, so the posts would display in order of upload with the most recent first: https://www.programiz.com/python-programming/methods/list/reverse
* This helped me style the background image on the main page: https://www.dwuser.com/education/content/the-basics-of-overlaying-content/
* This helped me properly format the method steps imported from the DB: https://developer.mozilla.org/en-US/docs/Web/CSS/white-space
* This helped me create a confirm message for deletion of posts and categories: https://stackoverflow.com/questions/9139075/how-to-show-a-confirm-message-before-delete/19973570
* This helped inspire the algorithm I would eventually write to correctly format youtube links for display on a method???s page, regardless of whether the user submits a sharing link or one from the browser???s search bar: https://stackoverflow.com/questions/29781974/convert-youtube-link-into-an-embed-link/29782133
* This generated my table of contents in my readme:https://ecotrust-canada.github.io/markdown-toc/

### Content
* All text content on the site is original.
* Credit to YouTubers [Spawn Wave](https://www.youtube.com/channel/UCoIXnB865l9Ex9zs4OIXTdQ) and [Linus Tech Tips](https://www.youtube.com/channel/UCXuqSBlHAE6Xw-yeJA0Tunw) for the videos that are currently embedded on the site.

### Media
The photos used in this site were obtained from:
* https://unsplash.com/@thdef
* https://unsplash.com/@film2024
* https://unsplash.com/@romankraft
* https://unsplash.com/@drscythe
* https://unsplash.com/@barnimages
* https://unsplash.com/@pjswinburn
* https://unsplash.com/@roselyntirado
* https://unsplash.com/@umby
* https://unsplash.com/@sidekix
* https://unsplash.com/@wardhanaaditya
* https://unsplash.com/@samthewam24
* https://unsplash.com/@honza_kahanek

### Acknowledgements

- I received inspiration for this project from my Code Institute course and a variety of online people (in credits above).
- I am also indebted to my mentor Akshat Garg, who as ever, provided ample, patient feedback on this project. 


