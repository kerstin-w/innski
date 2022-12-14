# Testing

## Contents

- [Functional Testing](#functional-testing)
- [Validator Testing](#validator-testing)
  - [HTML](#html)
  - [CSS](#css)
- [WAVE](#wave)
- [LightHouse](#lighthouse)
  - [Destop Results](#desktop-results)
  - [Mobile Results](#mobile-results)
- [Browser Compatibility](#browser-compatibility)
- [Responsivity](#responsivity)
- [User Stories](#user-stories)
- [Site Owner Goals](#goals)
- [Issues/ Bugs Found & Resolved](#issues-bugs)
- [Unresolved](#unresolved)

## <a name="functional-testing">Functional Testing</a>

---

| Page | Test | Completed successfully |
| :----| :----| :---------------------:|
| All | Navigation links to relevant pages | Yes |
| All | Navigation hover effect | Yes |
| All | Navigation collpases to a hamburger menu on mobile | Yes |
| All | Logo links back to homepage | Yes |
| All | Social media icons in the footer link to the correct external link and open in new tab | Yes |
| Homepage| Call to action button links to singup page | Yes |
| Homepage | Images and text flex responsively | Yes |
| Location | Images and text flex responsively | Yes |
| Schedule| Text flex responsively | Yes |
| Sign Up | User can only input the email address in the correct form | Yes |
| Sign Up | User can only submit when all required fields are filled in | Yes |


## <a name="validator-testing">Validator Testing</a>

---

### <a name="html">HTML</a>

[W3C Markup Validator](https://validator.w3.org/)

The initial test returned an error for the Youtube iFrame, a warning for the Gallery section and errors for the hamburger menu. 

<details>
<summary>Initial test</summary>

![HTML Validator first results](assets/testing/w3c-html1.jpg)

![HTML Validator first results](assets/testing/w3c-html2.jpg)
</details>
<details>
<summary>Homepage</summary>

![Screenshot of WC3 testing for InnSki homepage](assets/testing/w3c-index.jpg)
</details>
<details>
<summary>Location Page</summary>

![Screenshot of WC3 testing for Location page](assets/testing/w3c-location.jpg)
</details>
<details>
<summary>Schedule Page</summary>

![Screenshot of WC3 testing for Schedulen page](assets/testing/w3c-schedule.jpg)
</details>
<details>
<summary>Signup Page</summary>

![Screenshot of WC3 testing for Signup page](assets/testing/w3c-signup.jpg)
</details>

### <a name="css">CSS</a>

[W3C CSS Validator](https://jigsaw.w3.org/css-validator/) 

This test returned no errors.
Results of the CSS test of style.css:

![Screenshot of WC3 testing](assets/testing/jigsaw.jpg)

## <a name="wave">WAVE</a>

---

[WAVE](https://wave.webaim.org/)

The WAVE WebAIM web accessibility evaluation tool was used to check for accessibility standards.

The first result gave an error for a missing form label button on the Sign up page and an empty form label for the hamburger menu on the homepage.
- The missing form label button on the Sign up page was due to a typo. 
- Since the hamburger menu could only be created with HTML and CSS (rather than JavaScript which would be the better and accessibility better solution) the HTML symbol for hamburger menu has been added here to fix the bug. 

Afterwards, all pages passed with zero error. 

![WAVE Validator Results](assets/testing/wave.jpg)

## <a name="lighthouse">LightHouse</a>

---

Lighthouse was used (accessed through Developer Tools in Chrome) to analyse for the following:  

  - Performance
  - Accessibility
  - Best practice
  - SEO

The initial result was 90 but pointed out that loading time could be improved by properly sizing some images. Therefore, I converted all images from gallery section to .webp format. Even so, the images were still fairly large and I followed my mentor's advice and resized the images.

### Desktop Results

<details>
<summary>Homepage</summary>

![Screenshot of Lighthouse Desktop Validator Results for InnSki homepage](assets/testing/lh-desktop-homepage.jpg)
</details>
<details>
<summary>Location Page</summary>

![Screenshot of Lighthouse Desktop Validator Results for Location page](assets/testing/lh-desktop-location.jpg)
</details>
<details>
<summary>Schedule Page</summary>

![Screenshot of Lighthouse Desktop Validator Results for Location page](assets/testing/lh-desktop-schedule.jpg)
</details>
<details>
<summary>Signup Page</summary>

![Screenshot of Lighthouse Desktop Validator Results for Location page](assets/testing/lh-desktop-signup.jpg)
</details>

### Mobile Results 

<details>
<summary>Homepage</summary>

![Screenshot of Lighthouse Desktop Validator Results for InnSki homepage](assets/testing/lh-mobile-homepage.jpg)
</details>
<details>
<summary>Location Page</summary>

![Screenshot of Lighthouse Desktop Validator Results for Location page](assets/testing/lh-mobile-location.jpg)
</details>
<details>
<summary>Schedule Page</summary>

![Screenshot of Lighthouse Desktop Validator Results for Location page](assets/testing/lh-mobile-schedule.jpg)
</details>
<details>
<summary>Signup Page</summary>

![Screenshot of Lighthouse Desktop Validator Results for Location page](assets/testing/lh-mobile-signup.jpg)
</details>

## <a name="browser-compatibility">Browser Compatibility</a>

---

This website was tested on Chrome, Microsoft Edge, and Firefox for desktop. 

The website was tested on Safari for mobile and tablet. 

* The pseudo-element ::marker with content:"* " was added to a list on the schedule page. As it was found out during testing, the content wasn't supported by Safari. I decided to resolve this issue with a <span>. This was not an appropriate fix either and I solved it with a list style type and marker. Solution found [here](https://css-tricks.com/list-markers-and-string-styles/) 

## <a name="responsivity">Responsivity</a>

---

Responsiveness was tested through Chrome Developer tools. The devices tested include:

- iPhone SE
- iPhone XR
- iPhone 12 Pro
- Pixel 5
- Samsung Galaxy S8+ 
- Samsung Galaxy S20 Ultra
- iPad Air
- iPad Mini
- Surface Pro 7
- Surface Duo
- Galaxy Fold 
- Samsung Galaxy A51

I was able to directly test the website on an iPhone 13 mini and an iPad.

## <a name="user-stories">User Stories</a>

---

*As a user, I want to understand what the site is about.*

This was achieved through the hero banner, the brief explanation on the homepage and the "What to expect??? section. The user gets further and detailed information on the subpages "Location" and "Schedule".

*As a user, I want to easily navigate through the site even on the first visit.*

This was achieved through a common menu type, repeating patterns through the whole website and self-explanatory links. 

*As a user, I want to find Information on what the event contains and what I can expect.*

This was achieved through the ???What to expect??? section on the homepage, the subpage "Schedule" as well as the imagery throughout the whole page. 

*As a user, I want to find where the event takes place.*

This was achieved through the "Location" subpage and through the Youtube video on the homepage.

*As a user, I want to sign up for the event.*

This was achieved through the form on the "Sign Up" subpage. 

## <a name="goals">Site Owner Goals</a> 

---

*As a site owner, I want to inform about the event.*

This was achieved through the ???About??? and ???What to expect??? section on the homepage as well as through the "Schedule" subpage. 

*As a site owner, I want to inspire users to go freeride skiing.*

This was achieved through the video and gallery on the homepage and through the imagery throughout the whole page.

*As a site owner, I want people to sign up for the event.*

This was achieved through a sign up button in the hero banner and the sign up from. 

*As a site owner, I want to increase my reach and visits of the site.* 

This was achieved by creating an appealing website and event and through a good Lighthouse score which indicates a better Google ranking. 

## <a name="issues-bugs">Issues/ Bugs Found & Resolved</a>

---

During the development and testing phase, several bugs were identified and were resolved with the help of either Google, the Tutors, the Slack community, or my mentor.

### Navigation
Originally, I created the navigation on mobile without hamburger menu and the menu items listed in a block. However, this was a bit too delicate for mobile and it became apparent during testing that it was easy to click on the wrong menu item. I found a helpful [page](https://alvarotrigo.com/blog/hamburger-menu-css/) how to create hamburger menu even without JavaScript/Bootstrap and added this to the navigation.

### The pseudo-element
The pseudo-element ::marker with content:"* " was added to a list on the schedule page. As it was found out during testing, the content wasn't supported by Safari. I decided to resolve this issue with a <span>. This was not an appropriate fix either and I solved it with a list style type and marker. Solution found [here](https://css-tricks.com/list-markers-and-string-styles/) 

### Animation Hero Text
After my decision to move the text in the hero banner from the right side to the center, I had problems with the animation bouncing at the end to a position I didn't intend. I removed the Top % and Left % and centered the Hero text with Text Align. After that the animation behaved as expected. 

### Validation Issue
The initial test returned an error for the Youtube iFrame, a warning for the Gallery section and errors for the hamburger menu. The Youtube iFrame included an obsolete element <frameborder> which I ereased. Since the Gallery was set up as section, but wihtout text, the validation gave out a warining about missing headings for this section. Therefore I have changed the section into a div. Alternatively, the section could have used a hidden heading. The hamburger menu had an empty label and therefore I added a <span> to the menu-botton.

### Wave Issue
The first result gave an error for a missing form label button on the Sign up page and an empty form label for the hamburger menu on the homepage. The missing form label button on the Sign up page was due to a typo.The HTML symbol for hamburger menu has been added here to fix the bug for the hamburger menu label.

### Hover on "What you can expect"
During testing, I received feedback that the hover effect added to the boxes for the "What you can expect" section is misleading and implies that if you click on the boxes, something will happen. Therefore, this effect was deleted.

## <a name="unresolved">Unresolved</a>

---

### Page Speed
The Lighthouse score for "Performance" on mobile is not satisfying. Since the page uses several images, which were also obtained in rather high quality, this made the page quite slow. Compressing the images did not bring the desired success. I converted all pictures to .webp and I resized the images from the gallery at the advice of my mentor, since they do not have to be displayed in the highest quality due to their smaller size. Still, the performance is low.

### Parallax Scroll on mobile:
Unfortunately, the Parallax Effect is not yet well supported on mobile and the [W3C](https://www.w3schools.com/howto/howto_css_parallax.asp) solution turned out to be less than ideal when tested on an iPhone device. However, I have already found good approaches for the future. For example [here](https://stackoverflow.com/questions/57219561/background-attachment-fixed-in-firefox-or-edge-versus-chrome/).