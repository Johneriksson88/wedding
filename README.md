# John and Helenas wedding site

John and Helenas wedding site is a digital and interactive form of wedding invitation to our wedding. It's a place where the invited wedding guests can find information about the wedding, RSVP and look at inspirational pictures of the couple.

![Responsive Mockup](https://github.com/Johneriksson88/wedding/blob/main/assets/images/screenshots/wedding-screenshots.png?raw=true)

## Features 

In this section, you should go over the different parts of your project, and describe each in a sentence or so. You will need to explain what value each of the features provides for the user, focusing on who this website is for, what it is that they want to achieve and how your project is the best way to help them achieve these things.

### Existing Features

- __Navigation Bar__

  - Featured on all three pages, the full responsive navigation bar includes links to the Home page, Wedding info, RSVP and Gallery page and is identical in each page to allow for easy navigation.
  - This section will allow the user to easily navigate from page to page across all devices without having to revert back to the previous page via the ‘back’ button. 
  - The clickable "hamburger" type menu appears at screen widths at 520px or smaller and was created after watching [this](https://www.youtube.com/watch?v=8QKOaTYvYUA&t=1394s&ab_channel=KevinPowell) tutorial by YouTuber Kevin Powell.

![Nav Bar](https://github.com/Johneriksson88/wedding/blob/main/assets/images/screenshots/nav-screenshot.png?raw=true)

- __Landing page__

    - The landing page image is a photograph of John and Helena lovingly staring into each others eyes, with a nice tile background with a heart in it. It represents the love that will be celebrated at the wedding, and is intended to put the visitor in a good mood for going to our wedding.
    - Under the landing page image is the most important information: a "Welcome to our wedding!", a short introductory text and date and location under it.
    - Under that are three images to neatly frame the invitation information and add some more color to the otherwise black and white page.

![Landing Page](https://github.com/Johneriksson88/wedding/blob/main/assets/images/screenshots/landing-page-screenshot.png?raw=true)

- __Info page__

  - The info page contains all the information about the wedding, divided under the three sections of When, Where and How.
  - The Where section has clickable embedded Google Maps-links for the location of the bus stop and the wedding location.
  - The How section has every bit of practical information the guests need for preparation, along with a short schedule in a table format.

![Info Page](https://github.com/Johneriksson88/wedding/blob/main/assets/images/screenshots/info-page-screenshot.png?raw=true)

- __RSVP Page__

  - This page contains a simple form for the guests to RSVP to the wedding.
  - Required fields are name, email and number of guests. All other fields are optional.

![RSVP Form](https://github.com/Johneriksson88/wedding/blob/main/assets/images/screenshots/rsvp-screenshot.png?raw=true)

- __The Footer__ 

  - The footer section includes links to all pages on the website, as well ass the relevant social media sites for John. The links will open to a new tab to allow easy navigation for the user. 
  - The footer is valuable to the user as it encourages them to keep connected via social media, and lets them navigate when they've scrolled all the way down.
  - The footer has a small copyright text to inform the user of the author.

![Footer](https://github.com/Johneriksson88/wedding/blob/main/assets/images/screenshots/footer-screenshot.png?raw=true)

- __Gallery__

  - The gallery shows a bunch of different pictures of John and Helena together to inspire them for e.g. gifts, outfits or a speech. The image masonry style layout was inspired by the Love Running Gallery.

![Gallery](https://github.com/Johneriksson88/wedding/blob/main/assets/images/screenshots/gallery-screenshot.png?raw=true)


### Features Left to Implement

- A future idea is to add a page with a story timeline, where the user can see a timeline with pictures of events through the couples relationship, from the first date to the wedding.

## Testing 

Apart from the two validator tests, the most continuous testing of the project has been testing different screen widths to make sure the website is responsive all along different screen widths. I opened the finished project on my iPhone and made sure it looked good in Safari as well as Chrome.

Since this is my first website project you could say the whole thing was a bit of a test. Testing different ways to display my content, images, using flexbox etc.

### Lighthouse test ###

I used the Lightouse test in Google Devtools mainly to ensure the accessibility of the website. The performance part could have been improved by changing image sizes. Had this been a project for a customer i would take time to improve this, but since this will not be viewed by that many people, i don't think that is that important.

![Lighthouse test](https://github.com/Johneriksson88/wedding/blob/main/assets/images/screenshots/lighthouse-test-screenshot.png?raw=true)

### Responsiveness ###

As i build the website i continuously fooled around with the screen width to ensure the content i added was displayed correctly on all screen widths. I added media queries here and there, where there was a breaking point in the displaying of the content. Mainly i found the pictures needed media queries, and in the places where i used flexbox i simply changed the flex-direction from row to column where needed.

### Interesting bugs/errors ###

While putting the index.html through the W3C Validator I got these errors:

- Start tag body seen but an element of the same type was already open.
- End tag for body seen, but there were unclosed elements.
- Unclosed element div.
- Saw an end tag after body had been closed.

These errors are due to the canvas look of the page. The "paper" in which the content is confined is a div, so the body tag is within that div. The validator considers that an error. In discussions with my mentor he confirmed that i could do this without problems, so i chose to not change that since the canvas style is part of the design i strived for.

After i put the styles.css through the Jigsaw Validator i got these warnings:
- Family names containing whitespace should be quoted. If quoting is omitted, any whitespace characters before and after the name are ignored and any sequence of whitespace characters inside the name is converted to a single space.

These warnings appeared on all lines where i declared a font family containing a space in the font family name. After a bit of googling i learned that these errors were harmless and unneccesary, however i chose to add single quotes to the font family names to get a clean validation.

### Validator Testing 

- HTML
  - Apart from the above mentioned, no errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fjohneriksson88.github.io%2Fwedding%2Findex.html)
- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fjohneriksson88.github.io%2Fwedding%2Fassets%2Fcss%2Fstyles.css&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)

### Unfixed Bugs

Apart from the aforementioned error message regarding the body tag, no apparent unfixed bugs appear.

## Deployment

- The site was deployed to GitHub pages. The steps to deploy are as follows: 
  - In the GitHub repository, navigate to the Settings tab 
  - From the source section drop-down menu, select the Master Branch
  - Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment. 

The live link can be found here - https://johneriksson88.github.io/wedding/index.html


## Credits 

In this section you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 

You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign up page are from This Open Source site
- The images used for the gallery page were taken from this other open source site


Congratulations on completing your Readme, you have made another big stride in the direction of being a developer! 

## Other General Project Advice

Below you will find a couple of extra tips that may be helpful when completing your project. Remember that each of these projects will become part of your final portfolio so it’s important to allow enough time to showcase your best work! 

- One of the most basic elements of keeping a healthy commit history is with the commit message. When getting started with your project, read through [this article](https://chris.beams.io/posts/git-commit/) by Chris Beams on How to Write  a Git Commit Message 
  - Make sure to keep the messages in the imperative mood 

- When naming the files in your project directory, make sure to consider meaningful naming of files, point to specific names and sections of content.
  - For example, instead of naming an image used ‘image1.png’ consider naming it ‘landing_page_img.png’. This will ensure that there are clear file paths kept. 

- Do some extra research on good and bad coding practices, there are a handful of useful articles to read, consider reviewing the following list when getting started:
  - [Writing Your Best Code](https://learn.shayhowe.com/html-css/writing-your-best-code/)
  - [HTML & CSS Coding Best Practices](https://medium.com/@inceptiondj.info/html-css-coding-best-practice-fadb9870a00f)
  - [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html#General)

Getting started with your Portfolio Projects can be daunting, planning your project can make it a lot easier to tackle, take small steps to reach the final outcome and enjoy the process! 