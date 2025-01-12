# TESTING


## Compatibility

In order to confirm the correct functionality, responsiveness, and appearance:

+ The website was tested on the following browsers: Chrome, Firefox, Brave.

    - Chrome:

    ![Chrome](documentation/chrome-testing.gif)

    - FireFox:

    ![FireFox](documentation/firefox-testing.gif)

    - Edge:

    ![Edge](documentation/edge-testing.gif)

## Responsiveness


+ The website was checked by devtools implemented in Firefox and Chrome browsers.

    - Main Page:

    ![Main Page](documentation/responce-testing.gif)

    - Response Page:

    ![Response Page](documentation/responce-page-testing.gif)

+ The website was checked with [Responsive Website Design Tester](https://responsivedesignchecker.com/).

    - Desktop Screens:

    ![Desktop](documentation/desktop-screen.gif)
    

    - Tablet Screens:

    ![Tablet](documentation/tablet-screen.gif)

    - Mobile Screens:

    ![Mobile](documentation/mobile-screen.gif)

+ The functionality of the links in the website was checked as well by different users.

## Manual testing

| feature | action | expected result | tested | passed | comments |
| --- | --- | --- | --- | --- | --- |
| Navbar | | | | | |
| Home | Click on the "Home" link | The user is redirected to the top of the page | Yes | Yes | - |
| Education | Click on the "Education" link | The user is redirected to the Education section | Yes | Yes | - |
| Employment | Click on the "Employment" link | The user is redirected to the Employment section | Yes | Yes | - |
| Contact | Click on the "Contact" link | The user is redirected to the Contact section | Yes | Yes | - |
| Contact page | | | | | |
|  Name input | Enter the Name| The name is entered | Yes | Yes | If user doesn't enter the first name, the error message appears |
| Email input | Enter the email | The email is entered | Yes | Yes | If user doesn't enter the email, the error message appears. If user enters not valid email, the error message appears |
| Message input | Enter the message | The message is entered | Yes | Yes | If user doesn't enter the email, the error message appears. If user enters nothing, the error message appears |
| "Submit" button | Click on the "Submit" button | The user is redirected to the response page | Yes | Yes | - |
| Response page | | | | | |
| Response message | The user can return to home page by clicking Home link | The user is redirected to the home page | Yes | Yes | - |

---
## Validator testing
+ ### HTML
  #### Home Page
    - some errors were found when passing through the official W3C validator.

    ![Home Page HTML Validator](documentation/main-page-validate.png)
    ![Home Page HTML Validator](documentation/main-page-validate2.png)
  
  #### Response Page
    - No errors or warnings were found when passing through the official W3C validator.

    ![Response Page HTML Validator](documentation/response-validate.png)
    
+ ### CSS
  No errors or warnings were found when passing through the official W3C (Jigsaw) validator except:
    
    - 3 errors regarding *all: unset*: "Property all doesn't exist. The closest matching property name is fill : unset".

    - Even though this error is present, I don't believe it is 100% accurate, and more information can be found [here](https://developer.mozilla.org/en-US/docs/Web/CSS/all)

  ![CSS Validator errors](documentation/w3_validator_css_errors.png)
  
    - 43 warning regarding the use of *:root variables*: "Due to their dynamic nature, CSS variables are currently not statically checked".
    
  ![CSS Validator errors](documentation/w3_validator_css_warnings.png)


+ ## LightHouse report

    - Using lighthouse in devtools I confirmed that the website is performing well, accessible and colors and fonts chosen are readable.
    
  ### Home page

  ![Home Page Lighthouse](documentation/lighthouse_home_page.png)

  ### Gallery page

  ![Gallery Page Lighthouse](documentation/lighthouse_gallery_page.png)

  ### Contact page

  ![Contact Page Lighthouse](documentation/lighthouse_contact_page.png)

  ### Response page

  ![Response Page Lighthouse](documentation/lighthouse_response_page.png)

---
​
## Bugs
+ ### Solved bugs
    1. The testimonials pictures had a square shape in Brave browser on a mobile phone when the border radius had been set to 50%. It was due to the outline properties settings instead of the border
    
        *Solutions:* Outline was replaced with border properties.
    
    1. The gallery image descriptions were not appearing on the picture when hovering it as the position of the .image_content was set to fixed.
        
        *Solution:* The .image_content position was set to absolute, with the top: 0, left: 0, and added padding on the .image_content. 

    1. Footer on the contact page was reducing the size of the screen and shrank the contact form as the height of the background image was set to calc(100vh-the size of the footer)
        
        *Solution:* The height of the image was set to 100hv, and the display of the footer was set to fixed.
    ---
+ ### Unsolved bugs
    - None.
+ ### Mistakes
    - Mistakes were made while committing changes. I used past simple tense in commits due to the habit when I just started working on this project.
    - While progressing in my code I learned to use present simple tense in commits.

---
