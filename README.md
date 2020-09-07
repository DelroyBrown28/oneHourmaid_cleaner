# <div align="center">oneHourmaid</div>

oneHourmaid is a small project created to post a request containing the users details and home cleaning information. This can then be viewed and replied to over on the Cleaner Account page.

<img align="center" src="static\README_files\readme_heading_img.png">

## User Experience (UX)

The project was designed to lead the user straight to what they're looking for, weather that be to post a request to a cleanerfor Basic or Deep clean, or to view a pending job.

* ### Design
    * ###### Imagery
        - The main background of all pages uses a sunset image taken from [Unsplash.](https://unsplash.com/)
    * ###### Typography
        - The main font throughout is Lato, with Oswald as the as the projects title font and Sans-Serif as a fallback for both.
    * ###### Colour Scheme
        - The colors used are all based off of the main background image. A bright Orange is used for some of the form fields, along with a Dark Slate Grey for the buttons.

* ### Wireframes
    - Main page wireframe - [Here](#)
    - Services wireframe - [Here](#)
    - Basic Clean Wireframe - [Here](#)
    - Deep Clean Wireframe - [Here](#)
    - Cleaner Account Wireframe - [Here](#)

### Features
* #### [Main Page Features](#)
   - On the main page of the project you can choose between making a request or viewing any pending jobs. Making a request will take you to the services page whereas clicking "Cleaner Account" will show any pending jobs.
<img align="center" src="static\README_files\main_readme.png">

#### Future Features
I would like to add a Register and Sign in page so i can target Cleaners with more specific requests.
___

* #### [Services Page Features](#)
  - On the Services page you can choose between requesting a Basic or a Deep clean. Each takes you to a separate form to be filled out to post your request. The mobile view features a carousel instead of the cards seen in the desktop view.
<img align="center" src="static\README_files\services_page_rm.png">

#### Future Features
I would like to add another service called "Moving In/Out", there, you would have the choice of having a full deep clean for the home your moving in to or the property you're moving out of.
___

* #### [Basic Clean Page Features](#)
  - The Basic Clean page contains a simple form to be filled out with the Users information including, address of cleaning location and details of their cleaning needs i.e *"Please can you vacuum throughout."* This form is then posted in the [Cleaner Account](https://onehourmaid-project.herokuapp.com/cleaner_account) section to be viewed and responded to by the cleaner.
<img align="center" src="static\README_files\basic_clean.png">

#### Future Features
On the Basic Clean page I would like to be able to target specific cleaners based on how they registered, eg. if you registered as a Basic Cleaner, you will only receive the requests from the Basic Clean form.
___

* #### [Deep Clean Page Features](#)
  - The Deep Clean page is to post a more in depth request. Here, as in the Basic Clean form, you must fill out the form with your details and a short message containing your cleaning needs, you also have the choice of a requesting a deep Carpet Clean, Floor Steam, White Goods (cleaning behind ovens, fridges etc.) or simply get your Windows cleaned! This request will also be posted in the [Cleaner Account](#) section.
<img align="center" src="static\README_files\deep_clean.png">

#### Future Features
As the same with the Basic Clean page, I would like to be able to target specific cleaners based on the cleaning request.
___

* #### [Cleaner Account Page Features](#)
  - The Cleaner Account page is where you can view any requests made for either a Basic or Deep clean. Each job card will contain a tag reading either "Basic Clean" or "Deep Clean" to identify the type of post. Clicking on a job card will expand to display the rest of the request details including the users address and message. The Deep Clean job card will show the more in depth clean requested, including what they would like deep cleaned i.e Carpets, Windows etc. You also have the options to edit or delete your request. Clicking the "Send Confirmation" button will send a confirmation email to the users address.
<img align="center" src="static\README_files\cleaner_account.png">

#### Future Features
On the Cleaner Account page, I would like the ability for cleaners to only see jobs sent to them based on how they registered. I would also like to implement a better response function instead of a plain confirmation message.
___

### <div align="center">Libraries & Frameworks</div>


##### MaterializeCSS
I used [MaterializeCSS](#) for all of the forms, this helped alot for speed purpose, but does make styling buttons and popups etc. a little tricky. That being said, Materialize is easy to use and great for forms, buttons and grids.

##### Flask & Python3
[Flask](#) and [Python3](#) were used to send and receive data from [MongoDB.](#) ```@app.route``` was used throughout to navigate to pages and to trigger the actions on forms and buttons. The [Jinja2](#) template language was used alongside Flask to add and manipulate data in the HTML files, known to Jinja as "Templates."
- ###### Libraries used in Python3:
  - **flask_pymongo**
    *used to send and receive data from MongoDB*
  - **bson.objectid**
    *used to make changes to the database entries ```_id```*
  - **smtplib**
    *used to send the confirmation email fom the cleaner account*
  - **email.message**
    *used to send the confirmation email fom the cleaner account*