<p align="center"><img src="documentation/logo1.png" alt="Water Stations Ireland logo" width="70%"/></p>

 # <p align="center">**MS1: Water Stations Ireland**</p>

 ### View the live project [here.](https://loftusn13.github.io/ms1-waterstationsireland/)
 ### View the main README file [here.](./README.md)

---

## Contents
- [**Testing**](#testing)
    - [Code Validation](#code-validation)
    - [Links](#links)
    - [Navigation](#navigation)
    - [Contact](#contact)
    - [Initial Testing](#initial-testing)
    - [Accessibility](#accessibility)
    - [Device Testing](#device-testing)
    - [Browser Testing](#browser-testing)
    - [Known Bugs](#known-bugs)
    - [Testing User Stories](#testing-user-stories)

---

## <p align="center">**Testing**</p>
For the testing of this website I needed to ensure that it was fully functional and responsive across different browsers, devices and screen sizes. It is essential that users can easily find and see all 
content and images contained on the site without any elements overlapping and becoming illegible. It is important that the overall design, layout and purpose of the site are not compromised when being viewed on 
different devices. 

### **Code Validation**
- All HTML code on every page was validated through [W3C Markup Validator](https://validator.w3.org/) - no warnings or errors reported.
<p align="center"><img src="documentation/testing/html-validator.png" alt="HTML Validation Screenshot, shows no errors" width="70%"/></p>


- All CSS code was validated through [W3C CSS Validator](https://jigsaw.w3.org/css-validator/) - no warnings or errors reported.
<p align="center"><img src="documentation/testing/css-validator.png" alt="CSS Validation Screenshot, shows no errors" width="70%"/></p>

### **Links**
- I manually tested every link contained within the website to ensure none were broken and to ensure each one would lead the user to the correct place.
- All links correctly change colour when hovered over to alert users that they are links.
- Each link on each page works correctly; bringing you to the expected location. 
- External links on every page open in new tabs, bringing you to the expected location.
- The exception to this are the *Terms* and *Privacy Policy* links located in the footer on every page; these are not currently operational as explained in the [main README file](./README.md) under **Features Left to Implement**.

### **Navigation**
- I manually tested the navigation bar across different devices to ensure navigation ease in both the full and collapsed menus.
- Initial test had the header logo appearing too large on mobile devices, causing the collapsed menu to appear beneath the logo rather than beside.
    - This was **fixed** by reducing the size of the logo on mobile and scaling it up on larger devices using a media query.
- Collapsed hamburger menu correctly comes into effect on tablet and mobile devices, creating a cleaner design while still being clear that it is a means of navigating through the site.
- The correct styling (increase font weight and colour change) appears on the navigation link for each page when that page is **active**, making it clear to the user which page they are currently visiting.

### **Contact**
- I manually tested the contact form located on the *Contact Page* to ensure functionality across devices.
- The following steps were followed:
    - Navigate to the *Contact Page* via the navigation bar or the footer link.
    - Try to submit the form with a different field left empty each time.
    - Note the error message that pops up upon clicking the **Submit button** (see image below).
    - Try to submit the form with an incorrect *Email Address* format; without the "@" and with the "." in the wrong place.
    - Note the error message that pops up upon clicking the **Submit button** (see image below).
    - Try to submit the form with letters entered into the *Phone Number* field.
    - Note the error message that pops up upon clicking the **Submit button** (see image below).

<p align="center"><img src="documentation/testing/form-empty.jpg" width="90%"/></p>
<p align="center"><img src="documentation/testing/form-error.jpg" width="80%"/></p>

### **Initial Testing**
- I used [Google Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools) as my initial testing in order to see how well the website responded across different devices.
- This allowed me to see that some headings and elements, which looked great on mobile, appeared too small on larger screens and so I was able to implement media queries to increase 
    the sizes and adjust the paddings when the screen goes above certain dimensions.

<p align="center"><img src="documentation/testing/lighthouse.jpg" alt="Lighthouse DevTools Test Results" width="90%"/></p>

### **Accessibility**
- All images contain an *alt* attribute.
- Social media icons contain a description for screen-readers.
- I tested with [Lighthouse](https://developers.google.com/web/tools/lighthouse) in [DevTools](https://developers.google.com/web/tools/chrome-devtools). I noted that the contrast in the footer could be improved.
- In the future I will discuss changing the main blue colour of ***Water Stations Ireland*** with the company for improved contrast.  

<p align="center"><img src="documentation/testing/accessibility.png" alt="Accessibility results screenshot, shows 98%" width="50%"/></p>

### **Device Testing**
- I manually tested this website across a variety of devices to ensure responsivity.
- As mentioned above in **Initial Testing**, I also used [DevTools](https://developers.google.com/web/tools/chrome-devtools), in order to view the site on different screen sizes corresponding to different devices.
- As I had a limited option of devices available to me, I reached out to friends, family and the Slack community in order to test a larger sample.
- Devices the website was tested on include:
    - Amazon - 
        - **Kindle:** Fire.
    - Android mobile - 
        - **Huawei:** P10, P20 Lite, P30 and P30 Lite. 
        - **OnePlus:** 6T, 8 and Nord. 
        - **Samsung:** Galaxy A40 and Galaxy A5.
    - Android tablet - 
        - **Samsung:** Galaxy Tab A 10.1" 2018. 
    - Apple mobile - 
        - **iPhone:** 6, 8, 11 and X.
    - Apple tablet - 
        - **iPad:** 3rd Gen (iOS 9.3.5) and 4th Gen (iOS 10.3.3)
- During this testing a bug was found on Apple **iPhone** and **iPad** models where the hero video on the *Home Page* did not play and the opaque overlay and heading were gone, as seen in the image below.
    - Upon researching what would cause this glitch I discovered the following [article](https://developer.apple.com/documentation/webkit/delivering_video_content_for_safari).
    - This allowed me to figure out the issue which was to add the *muted* attribute to the **video element**. 
    - This **solved the bug** on the Apple devices as the video now plays as normal with the opaque overlay and heading in place.  
    - One exception to this can be found in [Known Bugs](#known-bugs).

<p align="center"><img src="documentation/testing/iphone-video.jpg" width="40%"/></p>

- During this testing, I was also alerted to something noticed on the **iPhone 11** device; details of which can be found in [Known Bugs](#known-bugs).
- I did further testing using [Google's Mobile-Friendly Test](https://search.google.com/test/mobile-friendly) and received positive results:

<p align="center"><img src="documentation/testing/mobile-friendly.png" width="40%"/></p>

- Overall, from my own device testing and from feedback received from others who viewed the website, I found:
    - The site was fully functional and responsive on all tested devices.
    - Design and layout remained consistent and flowing.
    - All written content and images are correctly laid out for optimal reading and viewing.
    - The site is easy and straightforward to navigate through.

### **Browser Testing**
- I manually tested this website across multiple browsers to ensure that all elements continued to function as normal.
- As the hero video on the *Home Page* is the only active element on the site I needed to ensure that it played as normal across browsers, i.e. that it wouldn't stop playing or require a user to do anything in order to play.
- **Opera, Mozilla Firefox** and **Microsoft Edge** were each tested on an Apple Macbook Pro.
- **Amazon Silk** was tested on a Kindle Fire.
- **Google Chrome** was tested on PCs, Apple Macbooks, multiple mobile devices and tablet devices.
- **Safari** was tested on Apple Macbooks and various iPhone and iPad models. The following was noted:
    - *Home Page* hero video seems to have the slightest delay in autoplaying on **Safari** but once started, it loops as normal.

### **Known Bugs**
- I was made aware of a slight bug on the **iPhone 11**:
    - As seen in the image below (red outline), the ***Water Stations Ireland*** logo in the footer has some image distortion on the right; obscuring the last letters of the word 'Station'.  
    - As seen in the image below (yellow outline), the image corrects itself when you zoom in closer to the footer, but then returns to its distorted form when you zoom back out. 
    - In an attempt to figure out this bug: 
        - I entered the dimensions of the **iPhone 11** into [DevTools](https://developers.google.com/web/tools/chrome-devtools) but the bug is not visible there.
        - I reached out to two other friends who also have the **iPhone 11** to ensure this was a model bug and not limited to just one device; they confirmed the same bug was present on their phones.
        - I asked them to open the site on both *Safari* and *Google Chrome* browsers to try and rule out if the bug was due to a browser but they reported that the bug is present across both browsers.
    - From my testing across all other devices as mentioned previously, this bug was not found on any other **iPhone** models or devices.
    - Further testing will be required to attempt to solve this bug.

<p align="center"><img src="documentation/testing/bug-iphone11.jpg" width="80%"/></p>

- Another bug presents on the **iPad 3rd Gen.** (iOS 9.3.5):
    - Upon landing on the *Home Page* the hero video does not autoplay.
    - The opaque overlay and heading are in place but the video appears as though it is a still image and does not play at any time.
    - From my testing across all other devices as mentioned previously, this bug was not found on any other device, including the other **iPad** model.
    - The cause of this bug may be that the model in question is an older one which runs an older iOS system, however further testing will be required to attempt to solve this bug.

### **Testing User Stories**
- "**As a potential customer, I want to learn about the company, their values and their goals.**"
    - Upon landing on the site, the user can scroll down on the *Home Page* to see both **Who We Are** and **What We Do** sections.
        - These sections provide the user with an introduction into who the company is and what they do; information the user would expect from reading those section headings.
        - The user can also click on *Home* in the navigation menu from all pages on the site to go directly there to find the above information.
    - The user can click on *About* in the navigation menu from all pages on the site to go directly there to find more of the information they're looking for.
        - The user can scroll down this page to find **Our Stations**, **Our Promise** and **Our Mission** sections.
        - These sections provide the user with information about the company's values and mission; content the user would expect from reading those section headings.
    - All of the above points are true across all devices; mobile, tablet, desktop etc.

- "**As a potential customer, I want to find detailed descriptions and clear images of the Water Stations the company offers.**"
    - The user can click on *Products* in the navigation menu from all pages on the site to go directly there to find this information. Upon scrolling down the user will:
        - find detailed information about the different options of Water Stations available; each option with its own heading explaining the type of Water Station it is, followed by a description.
        - find clear images of the Water Stations offered by the company.
    - The user can also find their way to the information they're looking for by clicking the link in the *Home Page*.
        - The user can scroll down the *Home Page* until they reach the **What We Do** section.
        - This link is within a message stating *"More details about our Water Stations can be found **here.**"*, which tells the user that information about the products 
        will be found upon following this link.
    - The user will also find a clear image of the Water Stations on both the *Home* and *About* pages.
    - All of the above points are true across all devices; mobile, tablet, desktop etc.

- "**As a potential customer, I want to easily be able to contact the company for further information.**"
    - The user is provided with several different ways of contacting the company.
    - The user can click on *Contact* in the navigation menu from all pages on the site to go directly there for contact information;
        - The user can find the company's email address, phone number and location.
        - The user will find the phone number acts as a link which, when clicked, will automatically dial the number in on whatever means of making a call is available on the device they're using.
        - The user will find links to the company's social media accounts, **Facebook, Twitter** and **Instagram** in the form of icons. These icons will change colour when hovered over and, when clicked,
        will open a new tab bringing the user to the correct social media page.
    - The user will also find a contact form to fill out on the *Contact Page*.
        - This form allows the user to enter their enquiry/question as well as providing their name, phone number and email address for the company to respond to them.
        - At this time, as there is no JavaScript in this release, this form will not actually be sent to the company.
        - The user will be alerted if they try to submit the form with a blank field or if a field is filled incorrectly.
        - Full details of the testing involved for this contact form can be found [**here**](#contact).
    - The user can also find the company's email address, phone number and social media links in the footer on every page.
    - The user can click on a link located in the footer to bring them to the *Contact Page*. The link is within a message stating "*Send us an enquiry* **here**.",
    which tells the user that this link will bring them to a place to make contact.
    - All of the above points are true across all devices; mobile, tablet, desktop etc.

<p align="center"><img src="documentation/testing/user-contact.jpg" width="80%"/></p>

- "**As a potential customer, I want to easily navigate through the website."**
    - Regardless of what page the user is on, they can always see the navigation bar fixed to the top of each page even if they have scrolled to the bottom (see image below).
    - The user can always click on the logo image at the top of every page to return them to the *Home Page*.
    - The user can always see clear names of each page, *Home, About, Products* and *Contact* so they know where to navigate to for the information or content
    they're looking for (see image below).
    - The user can easily identify a link, as a means of navigation, by the colour change of the font/icon when hovered over (see image below).
    - The user can always easily navigate straight to the *Contact Page* via the link which is present in the footer on every page.
    - The user can easily navigate straight to the *Products Page* via the link present on the *Home Page*.
    - All of the above points are true across all devices; mobile, tablet, desktop etc.

<p align="center"><img src="documentation/testing/user-nav.jpg" width="80%"/></p>

- "**As a potential customer, I want the website to be responsive on whichever device I’m viewing it on.**"
    - The user will find the website responsive across all devices.
    - The user can see all content clearly on any device.
    - The user can navigate easily through the site on any device.
    - The user can contact the company via various methods easily on any device.

<p align="center"><img src="documentation/testing/user-responsive.jpg" width="90%"/></p>

- "**As a potential customer, I want to explore a clean and professional website.**"
    - The user will not see any flashy or bold imagery to disrupt the crisp flow of the site.
    - The user will find all written content to be grammatically correct with a professional tone.
    - The user will find all content laid out in a clear and consistent manner throughout the site.