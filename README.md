# Prevent

A student project to create a single page website introducing the British Government's Prevent programme.

[See the website here](https://ctr-code.github.io/prevent/).

![The website on four different devices](docs/prevent.png)

## Design Brief

### External User’s Goal

The user wants a basic introduction to the Prevent strategy, including how to recognize signs of radicalisation and how to report concerns presented in a simple, easy-to-navigate format.

### Site Owner’s Goal

The site owner’s goal is to create an informative webpage that introduces the Prevent strategy. The content should be well-organised and easy to digest, with a focus on simplicity and clarity through the use of HTML and CSS with Bootstrap.

### Potential Features

* Introduction Section: A Bootstrap Jumbotron or header that briefly explains the Prevent strategy and its importance, with a background colour or image that conveys safety and community.
* Information Grid: Use Bootstrap’s grid system to create a well-organised layout for sections like “What is Prevent?” “Recognizing Risks” and “Reporting Concerns.”
* Lists of Signs: Present the signs of radicalisation using Bootstrap’s list group or bullet points to make the information easy to read.
* Action Buttons: Use Bootstrap’s button classes to create clear call-to-action buttons for reporting concerns or accessing additional resources.

## Design & Planning

### User Stories and Acceptance Criteria

1. **As a visitor, I want a clear introduction to the Prevent strategy so I can quickly understand its purpose.**
   - The page includes a short introductory section near the top.
   - The introduction explains Prevent in plain language.
   - It states the overall aim of Prevent clearly and positively.

2. **As a visitor, I want information about radicalisation so I can understand what to look out for.**
   - The page includes a dedicated section about radicalisation.
   - The section explains what radicalisation means and why it matters.
   - The content is framed in a way that is easy to understand and not alarmist.

3. **As a visitor, I want warning signs presented in a simple, readable format so I can scan them easily.**
   - Warning signs are listed in bullet points, list groups, or similar.
   - The language is concise and straightforward.
   - Related signs are grouped logically (e.g. susceptibility, behavior, process).

4. **As a visitor, I want clear guidance on how to report concerns so I know what action to take if needed.**
   - The page has a section on reporting concerns with a link to the government's official site.

5. **As a visitor, I want the page to feel calm, clear, and welcoming so I can engage with the content comfortably.**
   - The wording is reassuring and non-judgmental.
   - The layout avoids clutter and uses whitespace for readability.
   - The visual tone supports a calm, welcoming experience.

6. **As a visitor, I want to contact the site so I can leave feedback and ask questions.**
   - A contact option or section is clearly visible.
   - It explains how visitors can leave feedback or ask questions.
   - Contact information is easy to find and access.

7. **As a site owner, I want the content to be organised into clear sections so the page is easy to navigate and understand.**
   - The page is broken into distinct sections with clear headings.
   - Each section covers one main idea or action.
   - The structure is logical and easy to scan.

8. **As a site owner, I want the design to use simple Bootstrap styling so the webpage is informative, accessible, and visually clear.**
   - Bootstrap classes are used for layout and typography.
   - The page remains responsive on mobile and desktop.
   - The styling supports accessibility and a clean visual hierarchy.

### Wireframes

As the design evolved I realised I needed a section on contacting the authorities, which is missing from the wireframes.

Mobile/Tablet | Desktop | Confirmation Popup
-- | -- | --
![Wireframe for a mobile/tablet](docs/wireframe_small.png) | ![Wireframe for a laptop/desktop](docs/wireframe_big.png) | ![Wireframe for a confirmation window](docs/wireframe_confirm.png)

### Typography

For headers I have used the Rubik font, with the main header in bold.  It is an authoritative sans-serif font.  For everything else I used Inter, which is a very legible sans-serif.

### Colour Scheme

I chose a simple blue palette to reflect the water theme of the hero image.

![image of simple blue palette](docs/palette.png)

## Features

### Navigation
The site will have a fixed navigation bar with the logo and links to each of the sections.  On small screens the links will collapse into a hamburger menu.

### Hero Image
The project title and a slogan in front of a large image.

### Overview Section
A brief introduction to the Prevent programme.

### Radicalisation Section
A section with three cards:
* Susceptibility - life situations that make people susceptible to radicalisation
* Behaviours - behaviours indicative of radicalisation
* Process - the process that leads to radicalisation

### Report Section
Describing how to contact the authorities.

### Contact Us Section
A form to send a message to the site operators.

### Confirmation Modal
The confirmation modal is displayed when a message is submitted.  It explains that the message will **not** be read by anyone.

### Footer
The footer is not fixed.  It has a copyright message and social media icons.

## Copilot AI Assistance

Copilot came up with:

* The hero image of hands.  This required a lot of work (and several day's worth of free tokens!) to get something natural looking.
* The user stories and acceptance criteria.  I edited them down.
* The idea to use a shield for the logo.  Copilot provided some examples from around the web.  I asked it to render the shield emoji from the Google Noto font as an svg but it did a poor job, so I asked it for advice on a better conversion tool.  The online tools weren't happy with emoji fonts so I searched for a pre-converted svg and hand-edited it to match the site's palette.
* Code for the Radicalisation section.  The code worked but Copilot added a bunch of gratuitous styles, which I cleaned up.
* The meta description and keyword content.

My takeaway is that Copilot is good at coming up with a bunch of ideas, but if you have something in mind it is hard to get exactly what you want.

## Technologies Used

* HTML
* CSS
* JavaScript
* Bootstrap
* Font Awesome
* GitHub hosting and GitHub Pages
* Bunny CDN

## Testing

### Google Lighthouse Performance

Desktop | Mobile
-- | --
![Lighthouse for desktop](docs/lighthouse-desktop.png) | ![Lighthouse for mobile](docs/lighthouse-mobile.png)

### Browser Compatibility

Firefox | Chromium
:--: | :--:
![browser screenshot for firefox](docs/firefox-1200.png) | ![browser screenshot for chromium](docs/chromium-1200.png)

### Responsiveness

320px | 576px | 1200px
:--: | :--: | :--:
![responsiveness screenshot for 320px](docs/responsive-320.png) | ![responsiveness screenshot for 576px](docs/responsive-576.png) | ![responsiveness screenshot for 1200px](docs/responsive-1200.png)

### Code Validation

index.html | style.css
-- | --
![validation screenshot for html](docs/validate-html.png) | ![validation screenshot for css](docs/validate-css.png)

The CSS warnings are harmless.  They explain that imports and variables are not validated.

### Manual Testing user stories or/and features

| # | User Story | Test | Result |
| - | -------------------- | -------------------- | :------------------: |
| 1 | As a visitor, I want a clear introduction to the Prevent strategy so I can quickly understand its purpose. | Check that there is an introductory section that introduces Prevent and states its purpose. | &check; ![user story 1 test result](docs/u1tr.png) |
| 2 | As a visitor, I want information about radicalisation so I can understand what to look out for. | Check that there is dedicated, easy to understand section about radicalisation that is not alarmist. | &check; ![user story 2 test result](docs/u2tr.png) |
| 3 | As a visitor, I want warning signs presented in a simple, readable format so I can scan them easily. | Check that the warning signs appear in a bulleted list using straightforward language. | &check; ![user story 3 test result](docs/u3tr.png) |
| 4 | As a visitor, I want clear guidance on how to report concerns so I know what action to take if needed. | Check that there is a section with a clear link to the government's official site. | &check; ![user story 4 test result](docs/u4tr.png) |
| 5 | As a visitor, I want the page to feel calm, clear, and welcoming so I can engage with the content comfortably. | Check that the page uses calm language, has plenty of whitespace and a calm visual appearance. | &check; ![user story 5 test result](docs/u5tr.png) |
| 6 | As a visitor, I want to contact the site so I can leave feedback and ask questions. | Check that the site has an easy to find contact form inviting questions and comments. | &check; ![user story 6 test result](docs/u6tr.png) |
| | | Check that the name field is validated. | &check; ![user story 6 name test result](docs/u6tr-name.png) |
| | | Check that the email field is validated. | &check; ![user story 6 email test result](docs/u6tr-email.png) |
| | | Check that the phone field is validated. | &check; ![user story 6 phone test result](docs/u6tr-phone.png) |
| | | Check that the message field is validated. | &check; ![user story 6 message test result](docs/u6tr-message.png) |
| | | Check that the confirmation modal is displayed. | &check; ![user story 6 confirm test result](docs/u6tr-confirm.png) |
| 7 | As a site owner, I want the content to be organised into clear sections so the page is easy to navigate and understand. | Check that there are distinct, logical sections with clear headings | &check; ![user story 7 test result](docs/u7tr.png) |
| 8 | As a site owner, I want the design to use simple Bootstrap styling so the webpage is informative, accessible, and visually clear. | Check that the site looks right on different devices. | &check; See the responsiveness tests above. |

**Other Tests**

| Test | Result |
| -- | -- |
| External links open in a new tab | &check; |
| Internal links navigate correctly | &check; |
| The hamburger menu closes after navigating | &check; |
| The WAVE accessibility checker reports no real errors. (It complains that an img with an alt tag lacks one, and it complains about adjacent links with the same url.  One of these links is a button for emphasis.) | &check; |


## Bugs

* The hero image displayed repeatedly across the screen after I added the background gradient.  I read the [MDN page on using multiple backgrounds](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Backgrounds_and_borders/Using_multiple_backgrounds) to understand that I needed to double-up the background image properties.
* Copilot wrote the code to display the confirmation modal but it attached it to the wrong event so it didn't work.  I read the [MDN page on form submission using javascript](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Sending_forms_through_JavaScript) and fixed the problem.
* Following the advice in the project statement I used a Jumbotron for the header without realising it was a Bootstrap 4 feature and didn't do anything.  Unfortunately, the boilerplate that came with it introduced an unwanted margin but when I noticed that I fixed it and removed the Jumbotron cruft.
* After clicking on an internal link the heading was hidden under the navbar.  I added `scroll-margin-top` using the browser dev tools and it fixed the problem, but when I added it to the project it didn't.  After reading this [Stack Overflow question and answer](https://stackoverflow.com/questions/72581132/how-does-the-css-property-scroll-margin-top-and-scroll-padding-top-really-wo) I realised that I had initially tested it with javascript disabled, but it didn't work in production because the navbar collapser handles the scrolling.  Using the Firefox javascript debugger I found a bug in the code to obtain the height of the navbar and fixed it, which fixed the scrolling.  Later on I realised the scrolling was *still* broken on mobile, so I added a CSS variable to provide a consistent navbar height everywhere, and modified the code to use it.
* The default bootstrap link colour had contrast problems against the light section background so I used the darker blue from the palette.
* Lighthouse complained that the 40x40 logo was too low-res for high DPI screens so I re-rendered it at 80x80.
* The W3C validator completed about a skipped heading level so I changed the `<h4>` to `<h3>`.

## Deployment

#### To Create a Fork of this Repository on GitHub

* Sign into [Github](https://github.com/) and navigate to [this project](https://github.com/ctr-code/prevent).
* Click on the Fork button.  Then click on the green Create Fork button.  This creates a new repository for you with a copy of the project.
* Make a note of your fork's GitHub url.  Retrieve a local copy of the project with the command `git clone <url>`, substituting your fork's url.

#### Deploying on Github

* Open the repository you created in the previous section.
* Click on the Settings button to open the project settings.
* Click on the Pages section in the section list on the left.
* Under Build and Deployment the Branch will be set to None.  Choose master and click Save.  Your repository will deploy.

## Credit and Thanks

* [Code Institute](https://codeinstitute.net/) and its tutors for teaching, support and the navbar collapser
* [West Midlands Combined Authority](https://www.wmca.org.uk/) for funding the course
* [Tim Berners-Lee](https://www.w3.org/People/Berners-Lee/) *et al* for the web
* [GitHub](https://github.com/) for hosting the repository, the project plan and the site
* [Bootstrap](https://getbootstrap.com/) for the CSS framework
* [Font Awesome](https://fontawesome.com/) for icons
* [Fort Awesome](https://github.com/FortAwesome/Font-Awesome/releases) for collating the Font Awesome assets
* [Bunny CDN](https://fonts.bunny.net/) for font hosting
* [The Rubik Authors](https://github.com/googlefonts/rubik) for the Rubik font
* [The Inter Project Authors](https://github.com/rsms/inter) for the Inter font
* [Microsoft](https://www.microsoft.com/) for [Visual Studio Code](https://code.visualstudio.com/)
* [Copilot](https://copilot.microsoft.com/) for various tasks as described above
* [W3C](https://www.w3.org/) for the [HTML and CSS validator](https://github.com/validator/validator/)
* [Inkscape](https://inkscape.org/) for rendering the logo and favicons
* [GIMP](https://www.gimp.org/) for cropping many screenshots
* [Google](https://github.com/googlefonts/noto-emoji) for the Noto Emoji font, which provided the basis for the shield logo
* [Action Counters Terrorism](https://actearly.uk/) for Prevent guidance
* [His Majesty's Government](https://www.gov.uk/government/publications/prevent-duty-guidance/prevent-duty-guidance-for-england-and-wales-accessible#prevents-objectives) for the Prevent objectives
* [Balsamiq](https://balsamiq.com/) for trying to upsell me export after I had completed the wireframes
* [Coolors](https://coolors.co/) for the palette generator
* [Fireship](https://fireship.dev/amiresponsive) for the multi-device screenshot
