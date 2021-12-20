# QA Book

This is the QA Book. (QA stands for quality assurance.) If you're reading this, you're probably our new QA tester. If
so, welcome! If you're not a PhET employee, (1) thank you for reading this, (2) please let us know how you managed to
find this obscure corner of GitHub, and (3) feel free to read on and learn how we test our simulations. Just about
everything you need to know to test PhET simulations is in this book.

![Cover Comic](https://github.com/phetsims/QA/blob/master/documentation/images/cover-comic.jpg "Funny Comic")

Thanks to Cornel Stefanache and Constantin Orasanu of MonkeyUser.com for their
[humorous comic](https://www.monkeyuser.com/2018/the-struggle/) that Megan "PhETified."

***

## Contents

**[Section 1: Hardware & Software](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#section-1-hardware--software)**

  * [1.1: Devices](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#11-devices)
  * [1.2: Operating Systems](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#12-operating-systems)
  * [1.3: Web Browsers](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#13-web-browsers)
  * [1.4: Updates](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#14-updates)

**[Section 2: Communication & Coordination](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#section-2-communication--coordination)**

  * [2.1: Email](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#21-email)
  * [2.2: Google Groups](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#22-google-groups)
  * [2.3: Google Calendar](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#23-google-calendar)
  * [2.4: Google Drive](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#24-google-drive)
  * [2.5: Slack](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#25-slack)
  * [2.6: Zoom](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#26-zoom)

**[Section 3: GitHub](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#section-3-github)**

  * [3.1: Repositories](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#31-repositories)
  * [3.2: Terminology](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#32-terminology)
  * [3.3: Issues](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#33-issues)
  * [3.4: QA Pipeline](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#34-qa-pipline)

**[Section 4: Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#section-4-testing)**

  * [4.1: Development (Dev) Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#41-development-dev-testing)
  * [4.2: Release Candidate (RC) Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#42-release-candidate-rc-testing)
  * [4.3: PhET-iO Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#43-phet-io-testing)
  * [4.4: Accessibility (a11y) Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#44-accessibility-a11y-testing)
  * [4.5: Online Website Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#45-online-website-testing)
  * [4.6: Offline Website (Installer) Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#46-offline-website-installer-testing)
  * [4.7: Automated (Continuous) Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#47-automated-continuous-testing)
  * [4.8: Memory Leak Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#48-memory-leak-testing)
  * [4.9: Maintenance Release Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#49-maintenance-release-testing)
  * [4.10: PhETTest](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#410-phettest)
  * [4.11: App Testing](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#411-app-testing)

**[Section 5: Translations](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#section-5-translations)**

  * [5.1: Legacy Simulation Translations](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#51-legacy-simulation-translations)
  * [5.2: HTML5 Simulation Translations](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#52-html5-simulation-translations)
  * [5.3: Website Translations](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#53-website-translations)

**[Section 6: Maintenance & Management](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#section-6-maintenance--management)**

  * [6.1: Testing Matrix Management](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#61-testing-matrix-management)
  * [6.2: PhET Test Maintenance](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#62-phet-test-maintenance)
  * [6.3: Website Administration](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#63-website-administration)
  * [6.4: QA Book Maintenance](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#64-qa-book-maintenance)

***

## Section 1: Hardware & Software

We like to make sure our simulations (sims) work on most hardware and most software.

### 1.1: Devices

Check out the
[Asset Inventory](https://docs.google.com/spreadsheets/d/1XqnlW8DAlt2fZHDfDgkTMmMLpJZ1c0equBaPdkn2V08/edit#gid=0)
for a comprehensive list of the devices we own. The "QA Simplified Inventory" is a list of the devices in Ariel's
office (F925) in Gamow Tower.

#### Note on Tablets

If you are testing on a tablet, you might encounter bugs that occur when you use a stylus, but not when you only
use your fingers. Be cognizant of this.

### 1.2: Operating Systems

For a comprehensive list of operating systems (OS's) we support, check out the
[the PhET Help Center](https://phet.colorado.edu/en/help-center/running-sims). (Open the "What are the System
Requirements for running PhET simulations?" details.)

As of 2021-12-16 the operating systems we officially support are:

* Chrome OS
* iOS 13+
* iPadOS 13+
* macOS 10.12+
* macOS 11+
* macOS 12+
* Windows 10
* Windows 11

### 1.3: Web Browsers

For a comprehensive list of browsers we support, check out the
[the PhET Help Center](https://phet.colorado.edu/en/help-center/running-sims). (Open the "What are the System
Requirements for running PhET simulations?" details.)

Browsers probably include:

* Google Chrome
* Firefox
* Safari

### 1.4: Updates

Never update a testing device unless the QA team lead asks you to do so. Be especially careful when dealing with
devices with older versions of iOS or macOS because Apple doesn't let you "un-upgrade" your iOS or macOS version.

***

## Section 2: Communication & Coordination

We try to communicate and coordinate effectively at PhET.

### 2.1: Email

Be sure to check your email frequently as PhET employees often communicate their schedules via email. You'll also
receive GitHub notifications via email.

### 2.2: Google Groups

You should be part of the "PhET Team" Google Group.

### 2.3: Google Calendar

Accurately reflect your availability in the "PhET Student Employees/Researchers" Google Calendar.

### 2.4: Google Drive

We put all sorts of stuff that you'll need to use on Google Drive. You can post videos that you want to use in your
issues to Google Drive. Come up with a good way to organize your videos on Google Drive. You might want to use the
GitHub issue number in the name of your Google Drive video. 

### 2.5: Slack

If you're working, you should be on Slack! Please bother the developers with silly gifs. To do so, type `/giphy hello`.
(Replace "hello" with whatever you want a gif of.) It’s also a good idea to check Slack periodically during the week
for any updates.

### 2.6: Zoom

We occasionally use Zoom to video conference.

***

## Section 3: GitHub

GitHub is a code hosting website. If you use the version control software Git, you can post changes to code you make on
your computer to GitHub. PhET also uses GitHub to document issues with sims.

### 3.1: Repositories

A GitHub repository is like a folder with the code and issues for a specific simulation. It’s important to
familiarize yourself with each repository and its contents.

Some repositories contain code for things that aren’t simulations. The following is a list of those repositories with
brief descriptions:

* a11y-research: Accessibility Research keeps track of accessibility research.
* aqua: Automated Quality Assurance (AQuA) holds code for continuous testing. [PhETTest](https://bayes.colorado.edu/dev/phettest) uses some code in aqua.
* assert: Assert holds code for handling assertions.
* axon: Axon is sort of like the nerve system. Axon holds code for things related to properties, e.g. the value of a
speedometer.
* babel: Babel holds files of translated strings for HTML5 simulations.
* bamboo: Bamboo is a charting library built with Scenery.
* blast: Blast holds code for a simple simulation. This simulation only uses code from axon, joist, and scenery. Blast
diagnoses issues.
* brand: Brand holds assets for each of the three brands. The brands are (1) PhET, (2) PhET-iO, and (3) Adapted from
PhET.
* bumper: Bumper holds code for a simulation that is used to test deployment procedures.
* chains: Chains holds code for a simulation that is used to test string translation tools.
* chipper: Chipper holds code for tools used to develop and build simulations.
* dot: Dot is a mathematics library.
* example-sim: Example Simulation holds code for an example simulation. It is used to show interns and new employees
how the simulations work.
* griddle: Griddle is a charting library.
* joist: Joist holds code for the “framework” of simulations, e.g. the splash screen, home screen, navigation bar,
about dialogue, etc.
* kite: Kite is a library for 2D shapes.
* mobius: Mobius is a library for 3D shapes.
* nitroglycerin: Nitroglycerin holds code for chemistry-related things.
* perennial: Perennial holds, among other things, build server code. It also holds utilities for doing the build.
* phet-core: PhET Core holds code for utilities used by all simulations.
* phet-info: PhET Information is mostly documentation.
* phetcommon: PhET Common contains general purpose common code.
* phetmarks: PhET Marks holds a simulation that contains code that developers use to bookmark URLs.
* phet-office-mix: PhET Office Mix holds Microsoft Office 365 things. Collaboration with Microsoft to make PhET
simulations compatible Microsoft Office applications.
* query-string-machine: Query String Machine holds code that parses query parameters.
* rosetta: Rosetta holds code for the translation of HTML5 simulations.
* scenery-phet: Scenery PhET holds components based on Scenery that are specific to PhET simulations.
* scenery: Scenery is the scene graph library that is used to create all visual aspects of PhET simulations.
* sherpa: Sherpa holds third party libraries.
* shred: Shred holds code used in simulations with subatomic particles.
* simula-rasa: Simula Rasa holds code for a blank simulation.
* sun: Sun holds code for low level user interface components, e.g. buttons and sliders. It uses code from Scenery.
* tambo: Tambo holds code for sonification.
* tandem: Tandem holds code for supporting material for PhET-iO simulations. Used in conjunction with PhET-iO to enable
access to model and user interface components of the simulation.
* tappi: Tappi holds the code for haptics.
* tasks: Tasks is a list of tasks.
* twixt: Twixt is an animation library.
* vegas: Vegas holds code for the components used in games.
* vibe: Vibe holds code for handling audio in simulations.
* webgl-ripples: WebGL Ripples holds code for 2D waves.
* website-meteor: Website Meteor holds code for the Meteor-React upgrade of the PhET website.

### 3.2: Terminology

It is important to familiarize yourself with the correct terminology for the various things you will encounter in a
simulation. The words in quotation marks are the explanatory terms, and the words without quotation marks are the
correct terms. (Some terms are intuitive while others are counterintuitive, hence the list.)

* “tab” = screen
* “loading screen” = splash screen
* “picture of the simulation that directs you to the simulation when clicked” = screen icon
* “screen that loads after the splash screen and has screen icons” = home screen
* “screen icon that exists in the home screen” = home screen icon
* “bar that has screen icons” = navigation bar
* “screen icon that exists in the navigation bar” = navigation bar icon
* “PhET logo that opens a menu when clicked” = PhET menu
* “box in which items that can be dragged and interacted with are stored” = toolbox
* “item that exists in a toolbox” = tool
* “button that resets everything in the simulation” = reset all button 

![reset all button](https://user-images.githubusercontent.com/85511101/146598927-9b443cb5-14e3-4424-bbd2-75bd9e349a7c.jpg)

* “button that resets some things in the simulation” = reset button

![reset button white](https://user-images.githubusercontent.com/85511101/146601028-fec2a211-15d0-4868-9536-a06a0e1fe3ff.jpg)
![reset button yellow](https://user-images.githubusercontent.com/85511101/146599830-2e1eae8f-e47c-45ab-aa93-e23ac8558916.jpg)

* “button in a browser that reloads the page” = refresh button
* “button with a right pointing triangle” = play button

![play button](https://user-images.githubusercontent.com/85511101/146599190-9abf1a22-200a-41a6-9c60-1ca7c1b87365.jpg)

* “button with two bars” = pause button

![pause button](https://user-images.githubusercontent.com/85511101/146599558-780b7302-d0c5-4017-948b-82eedbe6f52f.jpg)

* “button with a bar and a right pointing triangle” = step forward button

![step forward button](https://user-images.githubusercontent.com/85511101/146599578-1b528a92-ff03-4583-8a44-40003e6f0a1a.jpg)

* “button with a square” = stop button

![stop button](https://user-images.githubusercontent.com/85511101/146599592-d372f47c-e194-426b-8edc-f4f65af4e30a.jpg)

* “boxed off area that contains information” = panel
* “red button with minus sign” = collapse button
* “green button with plus sign” = expand button
* “panel with a collapse and expand button” = accordion panel
* “circular button that can be blank or solid” = radio button
* “box in which a check mark can exist” = checkbox
* “bar with button that can be dragged up and down xor left and right” = slider
* “slider button” = thumb
* navigation bar icon != home screen icon
* refresh button != reset button != reset all button
* “pop-up information” = dialogue
* “X button in dialogue” = close button
* “drop down menu” = combo box
* “number adjuster that looks like a spinner”/has floating arrows = number picker

![Number Picker](https://github.com/phetsims/QA/blob/master/documentation/images/number-picker.png "Number Picker")

* “number adjuster that looks like a picker”/has buttons = number spinner

![Number Spinner](https://github.com/phetsims/QA/blob/master/documentation/images/number-spinner.png "Number Spinner")

* “slightly different simulation within a screen” = scene
* “toolbox that has multiple pages” = carousel
* “different pages in carousel” = pages
* “dots that exist under a carousel” = dots
* “using the dots to navigate between pages” = dot navigation
* “clicking and holding” = fire on hold

Check out the [Scenery-PhET demo](https://bayes.colorado.edu/dev/phettest/scenery-phet/scenery-phet_en.html?brand=phet&ea) and the
[Sun demo](https://bayes.colorado.edu/dev/phettest/sun/sun_en.html?brand=phet&ea) for more terminology.

### 3.3: Issues

Most of the issues you’ll create on GitHub will be bug reports. Creating a bug report or general issue is easy. Here
are the steps you need to follow:

1. Before you even think about creating a new issue, comb through existing issues to see if someone already created the
issue. Search all repositories on GitHub for the issue.
2. If someone has created a similar issue, consider commenting in that issue instead of creating a new issue.
3. Otherwise, go to the appropriate repository.
4. Click on the “Issues” tab.
5. Click on the “New Issue” button.
6. If the issue is a bug report for a simulation, use the template below.
7. If the issue is a general issue, simply describe the issue thoroughly and concisely.
8. Try to include versions of browsers etc. Be thorough.
9. Assign the appropriate PhET employee(s) and use relevant labels. This is often the developer who made the test
issue. Design questions go to Amy if they are science, or Amanda if they are math. If you are unsure who to assign, you
might be able to figure it out by reading the 
[Responsible Dev Document](https://github.com/phetsims/phet-info/blob/master/sim-info/responsible_dev.json) on GitHub.
10. Click the “Submit New Issue” button.

#### Issue Template

```
### Test Device

blah

### Operating System

blah

### Browser

blah

### Problem Description

blah

### Steps to Reproduce

blah

### Visuals

blah

<details>
<summary><b>Troubleshooting Information</b></summary>

blah

</details>
```

* Always remember to link the QA issue!
* It is courteous to use screenshots or gifs in the “Visuals” section of the bug report. For Windows,
[ScreenToGif](https://www.screentogif.com/) is recommended. For macOS, [Kap](https://getkap.co/) is recommended.
* Sometimes you'll need to record a video since GitHub only allows gifs that are smaller than 10 megabytes. You can
upload a video to your CU Google Drive and then post a link to the video in the GitHub issue.
* If you make a screen recording using the native iOS or iPadOS screen recording feature, you can use
[ezgif.com](https://ezgif.com/) to convert your mp4 to a gif.
* The troubleshooting information for a simulation comes from the “Report a Problem” link in the
simulation.
* If your issue is related to another issue, link the related issue.
* If there is a console available, check for errors and include them in the Problem Description. The console is a tool
that browsers provide. It shows and allows access to the internal workings of a webpage. It is used often in testing to
make sure that the sim is doing what it should be. To access the console, right click and click on the option which
says “Inspect”, or “Inspect Element”. Then click the console button. The hotkey for macOS is `command + option + i` and
for Windows is `control + shift + i`.

#### When an issue is fixed

When a developer has fixed a bug they will assign it back to QA to ensure that the bug is fixed and that no new bugs 
have arrisen. How this is done depends on the bug and where the simulation is in terms of development. When a bug is 
found during a dev test, the developer will assign the issue to QA (typically the tester the who found and reporeted the bug) 
and put it in the "Issues to Verify" collumn of the QA pipeline. When the issue is confirmed or found off on master, this should be noted 
and the issue assigned back to the developer. When an issue is found during an RC the developer will put in the "Issues to Verify" 
section of the next RC. If it is found to be fixed in that RC it can generally be closed. If it is not fixed it is assigned back.

The labels `status:ready-for-qa` and `status:ready-for-review` should ideally be used as described below, but follow any instructions 
as to whether to close an issue or reassign it. If it is part of an RC it can usually be closed. Otherwise it is usually reassigned. 
It is usually better to reassign if in doubt, and the developer can close the issue if appropriate.

#### A List of Labels and Their Descriptions

* design:a11y - For issues with the design of accessibility-related features, e.g. keyboard navigation, sonification,
etc.
* design:artwork - For issues with the design of artwork.
* design:general - For general design issues.
* design:phet-io - For issues with PhET-iO simulations.
* dev:a11y - For issues related to accessibility development.
* dev:enhancement - For issues related to development improvements.
* dev:phet-io - For PhET-iO development issues.
* dev:sonification - For issues related to sound.
* phet-io:event-stream - For issues related to event wrappers in PhET-iO simulations.
* phet-io:studio - For issues related to studio in PhET-iO branded sims.
* phet-io:record-and-playback - For issues relating to record and playback in PhET-iO simulations.
* phet-io:save-and-load - For issues related to state wrappers and launching from proxies in PhET-iO branded
simulations.
* status:ready-for-qa - For issues ready to be confirmed by QA and then closed. (We're done with this issue, please
confirm that it is fixed.)
* status:ready-for-review - For issues that need to be looked over and reassigned to the developer. (We're not
necessarily done with this issues, we just need some QA feedback.)
* type:automated-testing - For automated testing issues.
* type:bug - For bugs.
* type:duplicate - For duplicate issues.
* type:i18n - For issues related to internationalization.
* type:legacy-bug - For issues that also exist in Java or Flash sims.
* type:multitouch - For issues that require multiple inputs.
* type:performance - For performance issues, e.g. low frame rate, lag, etc.
* type:question - For questions.
* type:suggestion - To make a suggestion for improvements.

### 3.4 QA Pipline

In the QA repo, there is a project called the QA Pipeline. The pipeline contains cards that either correspond to issues 
in the QA repo for tests and sims, or to sims that will soon enter QA. The placement of these cards indicates where in testing 
that particular sim/issue is. It also indicates priority. If a test is in the active tests column then, the higher it is, the 
higher its priority. The pipline is edited primarily by Katie, Mark, and Kathy. When tests are done, they will be moved to their 
appropriate column.

Tests that are in the repo but not high priority, are being created in repo, or are expected to come in soon are kept in the 
section "Upcoming Tests (by priority)" and should be ordered roughly by how urgent they will be when the enter the main testing phase. 
"Issues to Verify" contains issues that were found by QA during testing that have been fixed. They should be checked on master and the 
results of those checks should be added to the issue. The issue should then be assigned back to the developer. "Active Tests" should have 
a max of 5 tests in it and they are ordered by priority. When testing is done the test is dragged to "Ready for Next Steps" and 
eventually "Done."

***

## Section 4: Testing

If it ain't broke, break it! 

### 4.1: Development (Dev) Testing

Development testing is whatever the developer wants it to be. Generally speaking, a development test entails making
sure the simulation behaves as intended. The GitHub issue for a development test will specify what needs to be tested.

When a simulation needs to be tested, a developer will open an issue in the QA repository and they should use
[the template for development tests](https://github.com/phetsims/QA/blob/master/issue-templates/dev-test-template.md).
The template should specify what exactly needs to be tested. The steps you need to follow and the platforms you need to
test for a development test can be found in the template. There should be a link to the simulation in the issue, but if
there isn’t, then you can find it [here](https://phet-dev.colorado.edu/html/).

If the developer has issues they want tested they will either use the labels `status:ready-for-qa` or
`status:ready-for-review`. If it is ready for QA then close the issue if fixed. If ready for review then leave open and
assign back to the developer.

Here's a list of platforms we like to do development tests on:

* Chrome OS
* iOS + Safari
* macOS + Safari
* macOS + Chrome
* Windows + Microsoft Edge
* Windows + Firefox
* Windows + Chrome

It’s a good idea to make sure the sim loads and doesn't break on Internet Explorer.

#### Note on WebGL

WebGL may not run on certain platforms and browsers, such as Chrome on old versions of macOS.

### 4.2: Release Candidate (RC) Testing

Release candidate testing is more thorough than development testing because the simulation undergoing testing is a
“release candidate.” Theoretically, major issues with the simulation will be fixed by the time it undergoes an
RC test.

When a simulation needs to be tested, a developer will open an issue in the QA repository. They should use
[the new template for release candidate tests](https://github.com/phetsims/QA/blob/master/issue-templates/rc-test-template.md).
There should be a link to the simulation in the issue, but if there isn’t, then you can find it
[here](https://phet-dev.colorado.edu/html/). The template should specify what exactly needs to be tested. Here are the
steps you need to follow for a release candidate test:

1. Familiarize yourself with the simulation.
2. If the developer wants you to test previous issues, then test those first. They should be marked with
`status:ready-for-qa` and, if they are fixed, should be checked off and closed.
3. Open the testing matrix.
4. Choose a device and browser combination that hasn’t been tested. Add your initials to indicate that you are testing
that platform.
5. Perform the below tests and fill out the testing matrix.
6. When you find an issue, see if it was in a previously published version if it exists.
7. On at least one platform, run a fuzz test on the debug version of the RC to look for assertions. To do this, add
the query parameter `?fuzz`.

#### RC Test Types

There are four types of rc test types. The first is a full RC, which will not have any extra labels and should follow all instructions. 
Second is the RC-Lite which will have fewer devices/platforms for a faster test. Third is a Spot Check which focuses mostly on 
issue confirmations. Forth is Research, which focuses on the needs and features of a specific research study. Those needs will be
elaborated on in the created issue.

1. Dev: Deep testing on limited platforms
2. RC-full: Deeper testing across more platforms 
3. RC-lite: Less testing, due to time constraints or just less need for testing.
4. RC-research: Light testing. The QA issue will be specific about what to focus on. Focus will be tailored to the needs of the research study. (Specific features, PhET-iO data stream, specific screens,...)
5. RC-spot check: Limited testing on targeted issue fix verification 

#### Full Screen Test

To do the full screen test, do the following:

1. In the PhET menu, there is a “Full Screen” button. Press that button.
2. Make sure the simulation goes into and out of full screen mode easily.
3. Make sure the simulation does not change when the simulation goes into and out of full screen mode.

#### Screenshot Test

To do the screenshot test, do the following:

1. In the PhET menu, there is a “Screenshot” button. Press that button.
2. Make sure the screenshot is exactly the same as the simulation.

#### Query Parameters Test

To do the query parameters test, append the URL with the following query parameters:

* `?showPointerAreas`: shows red touch area and blue mouse area
    * Some things won’t have a pointer area. This is normal.
    * Sometimes pointer areas will look strange, e.g. extending beyond the borders of a carousel. This is normal.
    * Make sure pointer areas do not overlap.
    * This query parameter adversely affects the performance of the simulation.
* `?stringTest=double`: doubles strings
    * Strings should scale down. Nothing should overlap.
    * If there is an issue, then it is an internationalization issue.
* `?stringTest=long`: makes strings 12345678901234567890123456789012345678901234567890
    * Make sure there aren't any layout issues.
    * This query parameter might reveal issues that ?stringTest=double doesn’t.
* `?stringTest=rtl`: makes strings Farsi
    * Make sure everything looks good.
    * Make sure everything functions normally.
* `?stringTest=X`: makes strings X
* `?stringTest=xss`: cross site scripting
    * This query parameter puts JavaScript into every string. The page should not redirect.
    * If the simulation does not redirect to another website, the simulation passes this test.
    * If the simulation crashes or fails to load, the simulation still passes this test.
    
##### Other Useful Query Parameters

* `?fuzz`: makes random clicks and touches
* `?fuzzBoard`: fuzz for keyboard nav inputs
* `?profiler`: shows frame rate of the sim
* `?screens=#`: only shows screens indicated by the number sign
* `?ea`: enables assertions but doesn't work on RC’s
* `?speed=#`: multiples animation speed by the number
* `?dev`: shows bounds of the sim
* `?colorProfile=projector`: starts sim in projector mode if available
* `?a11y`: activates any a11y features that are available but not visible
* `?phetioDebug`: adds and checks for assertions in PhET-iO sims

##### Private Query Parameters

Some Query Parameters may only be used by members of the PhET team. The method of viewing them should not be disclosed.
See [Private Features for PhET Team Members](https://github.com/phetsims/special-ops/blob/master/doc/phetTeamMember.md)
for instructions on how to enable private query parameters. `?showAnswers` is an example of this.

##### Syntax for Multiple Query Parameters

Multiple query parameters can be used at once. It's as simple as adding an ampersand between query parameters.

`?queryParameter1&queryParameter2&queryParameter3`

#### Legends of Learning Test

To test a simulation in the Legends of Learning (LoL) harness, do the following:

1. Go to https://app.legendsoflearning.com/developers/signin.
2. Use the email and password provided by Katie to sign in.
3. Go to the Harness section on the left side of the screen.
4. Upload a dummy language json file like:

```json
{
   "_meta":{
      "maxChars":{
         "welcome":50
      }
   },
   "en":{
      "welcome":"Welcome"
   },
   "es":{
      "welcome":"Bienvenido"
   }
}
```

5. Add `?legendsOfLearning` to the end of the sim url and add it to the test harness.
6. Above the sim frame, verify that you can use "|| Pause" and "|▷ Resume" to pause and play the sim.

#### Game Up/Snap Thought Test

To test the Game Up harness, do the following:

1. Enter `https://phet-dev.colorado.edu/html/gameup/gameup-harness.html` in the url.
2. Add a querry parameter that includes the url of sim being tested `?sim=https://phet-dev.colorado.edu/html/sim/#.#.#-dev.#/phet/sim.html`.
3. Add a second querry parameter (with a second `?` rather than a `&`) that looks like `?gameUpLogging&gameUp&gameUpTestHarness`. Order matters and these should be after step 2.
4. Open the console. It should say: `Enabled Game Up Camera`, `Posted captureReady, number of checks #`, and `GameUpCaptureReady`.
5. The number of checks should be low. If over 5 there is likely an issue.
6. Make sure you can press the capture button and get a screenshot. The console should say `Sent image`.

#### Pan and Zoom testing

You should be able to zoom in and out using the same sorts of methods you would expect for most web pages.

1. Ctrl + +/-/0
2. Ctrl + scrolling
3. Pinch to zoom

You should be able to pan (move the zoomed in screen) by:

1. Dragging the screen with mouse or finger
2. Arrow keys (when not focused on another object)
3. Scrolling (up and down and left and right)

Make sure that all UI components behave normally while zooming in. Dragable objects should behave as expected and not move the screen unless at the edge of the screen.

#### HTML Download Test

To perform the HTML download test, do the following:

1. On an iOS device, open the simulation and add it to your “Reading List.”
2. Disconnect from the internet.
3. Open the simulation and make sure it behaves normally.
4. On a device with Google Chrome installed, save the simulation by right clicking on the link to the simulation in
https://phet-dev.colorado.edu/html/.
5. Disconnect from the internet.
6. Open the simulation and make sure it behaves normally.

For this test, we only care about the `{simulation}_all_phet.html` link.

#### iFrame Test & XHTML Test

To perform the iFrame test or the XHTML test, simply click the link to the iFrame or the link to the XHTML version of
the simulation and make sure the simulation behaves normally.

#### Debug Version

Run the debug version of an RC found [here](https://phet-dev.colorado.edu/html/) with the query parameter `?fuzz` to
see if errors pop up in the console.

#### Maintenance Issues

Check the sim's repo for issues that indicate a maintenance release has occurred. It should be marked Ready-for-QA. If
there is a problem, notify the developers.

#### Screenshots

When a simulation is about to be published, we have to take screenshots of the simulation that will be used on the
website. Usually you have one main screenshot and two to three alt screenshots.

##### Screenshots on Chrome

1. Download Window Resizer.
2. Download Screenshot Capture.
3. In Window Resizer set preset to 1536x1008. In Screenshot Capture set "Adjust to actual size" preset.
4. Resize the viewport.
5. Right click screenshot capture icon, go to options, and make sure the capture method is set to capture viewport.
6. Set up the screenshot.
7. Make sure there are enough pixels. The extension should give a warning if it can't resize properly.
8. Press `alt + s` (this is the default keyboard shortcut) to take the screenshot. (Make sure the download bar from any
previous screenshots is gone.)
9. Check the image to make sure it has the right dimensions (1536x1008).
10. Rename screenshots `sim-name-screenshot.png` or `sim-name-screenshot-alt#.png`.
11. Upload the screenshots to the sim repo's assets folder in GitHub.

##### Screenshots on Firefox

1. Download ResizeIT.
2. Download Easy Screenshot.
3. In ResizeIT set the dimension to 1548x1089.
4. Set up the screenshot.
5. Make sure there are enough pixels. The extension should give a warning if it can't resize properly.
6. Click on the screenshot extension. (Make sure the download bar from any previous screenshots is gone.)
7. Select "capture visible web content".
8. Save the screenshot.
9. Check the image to make sure it has the right dimensions (1536x1008).
10. Rename screenshots `sim-name-screenshot.png` or `sim-name-screenshot-alt#.png`.
11. Upload the screenshots to the sim repo's assets folder in GitHub.

#### General Protocol for Z-Ordering of Tools

Generally speaking, we try to make sure the active, i.e. most recently clicked, tool or item should be on top of other
tools or items. There are, of course, exceptions to this rule, so don't lose your mind if this isn't the case. Consult
the design doc or ask the designer if you think something is wrong with the z-ordering of tools or items.

### 4.3: PhET-iO Testing

PhET-iO simulations are licensed versions of PhET simulations. PhET-iO simulations are not available to the general
public. We charge customers for these simulations because they are highly customizable. When a customer pays for a
PhET-iO simulation, they are provided with the password for the simulation as well as an application program interface
(API) that they can use to customize the simulation. In the PhET-iO issue, there will be, among other things, a link to
a root directory or wrapper index and a link to a testing matrix. The root directory contains all of the wrappers, i.e.
environments, in which the simulation will be tested. The testing matrix is where we document what has been tested and
by whom. There should be a link to the simulation in the issue, but if there isn’t, then you can find it
[here](https://phet-dev.colorado.edu/html/). Here are the steps you need to follow for a PhET-iO test:

1. Open a private tab.
2. Click the link to the wrapper index.
3. Enter the username and password.
4. Familiarize yourself with the simulation.
5. Open the testing matrix.
6. Choose a device and browser combination that hasn’t been tested.
7. Perform the below tests and fill out the testing matrix accordingly.

Before reading about the various tests you’ll perform on a PhET-iO simulation, it should be noted that PhET-iO testing
can be daunting. It will help if you learn what a tandem ID is. You will no doubt encounter them. A tandem ID is an
identifier for a particular behavior of the simulation. For example, you could encounter the following tandem ID while
testing the studio wrapper.

`faradaysLaw.faradaysLawScreen.model.magnet.positionProperty`

The above tandem ID tells you the following: (1) the simulation is Faraday’s Law, (2) the behavior the tandem ID refers
to occurs in the Faraday’s Law screen, (3) model indicates that something is being modeled according to some set of
rules, (4) magnet indicates that the magnet is what is being modeled, and (5) positionProperty states the current
position of the magnet. For a more comprehensive treatment of tandem IDs, read
[this](https://docs.google.com/document/d/1Fr-B66SD-6Xt7egNv9ZeSXdcsK6k8Lkc0nqR853_eJ4/edit?pli=1#heading=h.oz7vdnbiq4ni).

The wrapper index is password protected! The Simulation, phet-io.js, Events:colorized, and Events:json are not password
protected.

When making issues, try to include the specific link you were using when you found the problem. You need to Slack the
link to the developer if the issue is in a public GitHub repository.

There will be links to guides in the wrapper index. One of these guides will include client requests. Make sure to check these 
requests during testing.

#### Wrapper Index Test

* In the Wrapper Index there should be some example code. Copy and paste it into a text editor, save it, and make sure
the resulting html file runs properly.
* Add `/lib` to the end of the wrapper URL. Make sure a file called `phet-io.js` is there. If it is, make sure
it is minified.

#### Login Wrapper Test

* Add this to the end of the link to test:
`/wrappers/login/?wrapper=record&validationRule=validateDigits&&numberOfDigits=5&promptText=ENTER_A_5_DIGIT_NUMBER`.
* Successful login should take you to the record wrapper.
* Make sure login `phettest` successfully loads.
* Make sure a five digit number successfully loads.
* Once on the record wrapper, type `window.sessionStorage` into the console, and make sure the key
`phet.metacog.learner_id` has a value of the login ID you provided it.

#### Offline Test

Test that the sim works offline:
* Go to https://phet-dev.colorado.edu/html/{{sim}}/{{version}}/phet-io/{{sim}}-phet-io-{{version}}.zip
* Download it
* Unzip it to a spot locally
* Open `index.html` by double clicking it on your desktop or in a finder-view.
* It should look like the standalone version of the sim in PhET-iO brand.


#### Simulation Wrapper Test

* *What?* This wrapper is the simulation.
* *How?* To test this wrapper, follow the steps for a development test or a release candidate test depending on
what the issue specifies. A memory test should be included on one platform here.

#### Studio Wrapper Test

* *What?* This wrapper is the simulation alongside a long list of instrumented characteristics. An instrumented
characteristic is some aspect of the simulation that can be modified by a licensed owner of a PhET-iO simulation, e.g.
a property. Not all characteristics of the simulation are instrumented so as to retain the functionality of the
simulation. Using Studio is tested on Mac and Windows Chrome platforms. Other platforms should test html files 
made in this way.
* *How?* To test this wrapper, make sure instrumented characteristics can be modified and make sure charac- teristics
that haven’t been instrumented can’t be modified. Make sure the UI functions as expected. Also, do the following:
  1. Periodically launch the simulation to make sure it works using the “Launch” button.
  2. Periodically copy and paste the HTML into a text editor, save the file, and open it in a browser to make sure the
  modifications you made are still there using the “Generate HTML” button.
  3. When doing the above, make sure that the resulting sim resets to the state it launched in, rather than the default
  sim's original state, when you hit reset all.
  4. Check that the changes documented in the Client Request form can be done properly.
 
 One random platform combination should use the `?phetioDebug` query parameter.

#### Data: Colorized Wrapper Test

* *What?* This wrapper is the simulation, but when you open the console, you are able to view a colorized event stream.
* *How?* To test this wrapper, manipulate the simulation and make sure the events you see in the event stream match the
manipulations. This test should be done lightly to make sure the data stream prints out to the console as it should.

#### Data: JSON Wrapper Test

* *What?* This wrapper is the simulation, but when you open the console, you are able to view the event stream in
JavaScript object notation.
* *How?* To test this wrapper, manipulate the simulation and make sure the events you see in the event stream match the
manipulations. This test should be done lightly to make sure the data stream prints out to the console as it should.

#### Data: Text Area Wrapper Test

* *What?* This wrapper is the simulation with the event stream below. There is a limit to the number of events that can
be displayed below the simulation.
* *How?* To test this wrapper, manipulate the simulation and make sure the events you see in the event stream match the
manipulations. This test should be a bit more in depth than the colorized and JSON tests. Performance should also be 
acceptable.

#### Data: Recording Wrapper Test

* *What?* This wrapper allows you to record your actions in the simulation.
* *How?* To test this wrapper, do the following:
  1. Open the console. (This is an important step! If you don't open the console prior to recording,
  `window.saveLogToFile` will not work!)
  2. In the URL, replace `&console` with `&localFile`. (If `&console` doesn’t exist, then you should still add
  `&localFile`.)
  3. Record your actions in the simulation. (Remember what you did.)
  4. Follow the directions in the console to download a copy of the recording.
  5. View the recording in the Events: Playback wrapper and make sure your actions were recorded accurately.
  6. If a previous recording wrapper exists and is provided, make a recording in that wrapper and test with the current
  playback method.
  7. If this sim is outfitted with alternative input (such as keyboard navigation), then also test it to make sure
  those input events work as well.
  8. Not supported on iPad or IE.
  9. This should not be done in a private window (won't work in some browsers.)
  10. Make sure that you are in the "top" context rather than the "sim" context in the console.
  
#### Data: Metacog Cycle Test
  
* *What?* This test exercises the full recording and playback process used for PhET studies. This includes recording
data to and retrieving data from our data back end partner, Metacog.
* *How?* 
  * First generate the link for testing. From the version directory of the RC, add the following: `/wrappers/login/?wrapper=record&validationRule=validateDigits&numberOfDigits=5&promptText=Enter%20a%205%20Digit%20ID&publisher_id={{PUBLISHER_ID}}&key_name=testing&widget_id={{SIM}}-{{VERSION}}-qaTest&metacog`. @KatieWoe should have the publisherID that goes with the key_name provided. Please note that these two values version together, so not any publisher_id will work. Make sure to change the `widget_id` based on each test. This is the unique identifier used to get back a collection of tests. We change this each sim/version to make sure you don't get back recording sessions from other test issues. Make your recording using this link. 
  * Make sure you are recording to Metacog by looking in the
console. You should see the following: `Recorder initialized, sending data to: ["metacog"]`. 
  * When you are done, press
either the back arrow or close the tab. You should be prompted to stay while the process finishes. Do not leave!
Instead, press cancel and wait for the go-ahead to leave. (Firefox may not show the dialog if you use the back arrow.)
  * Wait for thirty minutes before moving to the next step. 
  * Use this
[link](https://bayes.colorado.edu/dev/phettest/phet-io-website/root/metacog/request-data.html) or [link](https://phet-io.colorado.edu/metacog/request-data.html) to retrieve the data. Paste the
provided URL (just the query parameter part) into the URL box, the ID into the Application ID (this will not be given
in the issue, but @katieWoe will have it), and the email you want to receive the logs in into the email box. Nothing else needs to be entered. If you have the console open when you hit submit you will get an ID number you can
use if something goes wrong with the retrieval. 
  * The email will take about 20 minutes. Make sure the `.gz` file is
uncompressed. 
  * Use the playback link in the wrapper index to test the recording.
[This](https://github.com/phetsims/phet-io/blob/master/doc/metacog.md) may be helpful.
  * This test should be done on two platforms. iPadOS + Safari, and one other random platform that should change with each test.

#### State Wrapper Test

* *What?* This is a wrapper that contains a simulation, a mirror of the simulation that is updated once every given amount of time
(which is determined by a slider). The slider can also be set to 0 and the state set with a particular button. The bottom sim will 
interact and play forward until the next state update, at which point it should match the top sim and this behavior repeats.
There is also a condensed list of instrumented characteristics. This maps well to how the state is done in Studio.
* *How?* To test this wrapper, simply play with the simulation and make sure your actions are mirrored accurately. Note
that some actions like opening menus aren't transmitted. This applies to studio launches as well. One random platform combo should 
use the `?phetioDebug` query parameter. Check particular states by setting the state update rate to 0 and setting the state manually. 
You can further control behavior by making it so the sims are not active during the update.

#### Input Record and Playback Wrapper Test

* *What?* This is a wrapper that contains a simulation and a mirror of the simulation that is updated with every user
input. This maps well to what is done in the recording wrapper.
* *How?* To test this wrapper, make sure your actions are mirrored accurately. Spend plenty of time testing this
wrapper.

#### Screenshot Wrapper Test

* *What?* This is a wrapper in which you can take a screenshot of the simulation.
* *How?* To test this wrapper, test screenshots as you normally would by pressing the “Take Screenshot”
button in the wrapper, not the “Screenshot” button in the simulation.

#### Active Wrapper Test

* *What?* This is a wrapper that allows you to toggle between an active simulation and an inactive simulation.
* *How?* To test this wrapper, simply make sure you can interact with the simulation when it is active and
cannot interact with the simulation when it is inactive. Animations should resume without “jumping.”

#### Diff Wrapper Test

* *What?* This is a wrapper that allows you to compare the differences between a previous build and the current build.
* *How?* To test this wrapper you will need to test two different cases by entering a URL into the box. The first URL
should be the wrapper index URL, which should be /simulation/version/phet-io/ currently being tested, and it should
show no differences. The second URL will be provided in the issue (and it should be the wrapper index URL, which should
be /simulation/version/phet-io) and should show some difference. The simulation HTML file or phet-io.js lib file should
also work.

##### Michael Kauzmann's Detailed Diff Wrapper Instructions

1. Make sure it says the APIs are the same when comparing to itself, type
https://phet-dev.colorado.edu/html/{{sim}}/{{version}}/phet-io/ into the comparison input text.
2. If the sim has been published before on phet-io.colorado.edu, compare the most recent version there. Ask the dev to
run (or run yourself) `cd perennial; grunt print-phet-io-links` to see if the sim is in the list.
3. If not, see if there is a previous dev version for phet-io that you can compare to. It will likely have lots of changes
in it, and that's OK! It is expected that each phet-io version being published has been thoroughly designed, and that it
is as expected (including prior use of the diff wrapper by designers to see if anything suspicious has changed between
versions).

#### Multi Wrapper Test

* *What?* This wrapper demonstrates how to embed multiple PhET-iO simulations in the same page.
* *How?* To test this wrapper, make sure the active toggle works on both sims. Make sure to property toggle has the
expected effect based on its language for each. If the sim is not active, property changes will not appear until the sim is active again.

### 4.4: Accessibility (a11y) Testing

One of PhET’s goals is to make our simulations available to everyone. This, of course, includes people with
disabilities. There are three features to unique to accessibility testing: keyboard navigation compatibility, screen
reader compatibility, and sound effects (sonification). Keyboard navigation compatibility allows the user to play with
the simulation using the keyboard, i.e. they don’t have to use the mouse. Keyboard navigation can be tested on any
device with a physical keyboard and in any browser. Screen reader compatibility allows the user to hear a description
of what is happening in the simulation. On Windows devices, we test the NVDA and JAWS screen readers. On macOS devices,
we test the VoiceOver screen reader, which is installed by default. JAWS is tested on Chrome, NVDA is tested on Firefox,
and VoiceOver is tested on Safari. To familiarize yourself with a screen reader, use the screen reader to read
[this](http://htmlpreview.github.io/?https://github.com/phetsims/a11y-research/blob/master/reader-intro.html). In an
issue for a test of a simulation with accessibility feature(s) you will find, among other things, a link to the
simulation, perhaps a link to a testing matrix (if the test is an RC test), and a link to the a11y view. The a11y view,
is a page with the simulation on the left and the description of the simulation in plain text (the parallel document
object model or PDOM) on the right. Below the simulation are real-time alerts that will be announced by the screen
reader.

Please read through this
[list of known a11y bugs](https://drive.google.com/open?id=12kTs-g-iKEIH1dyG7Q41_W_oNL4gUKbkW-IQgZjMUBw) before doing
any testing.

To test the accessibility features of a simulation, follow the steps below:
1. Start the screen reader before you open a browser.
2. Familiarize yourself with the simulation.
3. If the developer wants you to test previous issues, then test those first.
4. Perform the below tests.

#### Keyboard Navigation Test

To test keyboard navigation, make sure keyboard navigation functions as described in the “Keyboard Shortcuts” dialogue. 
If keyboard navigation does not seem to work on Mac Safari, it is likely that you will need to change the settings 
to have Full Keyboard Access.

#### Screen Reader Test

To test a screen reader, do the following:

1. Make sure you know how to use screen readers. (If you don't, ask Katie.)
2. Carefully read the a11y view.
3. Quit your browser.
4. Start your screen reader.
5. Make sure "audio ducking" is off in screen reader settings.
6. Open the sim.
7. Read everything in the simulation with the screen reader using keyboard nav.
8. Make sure all possible alerts are given.
9. Make sure all possible descriptions match the state of the simulation.
10. Make sure the alerts and descriptions make sense.

#### Voicing and Interactive Highlights
##### What is "Voicing"?
Voicing is a new accessibility feature developed by PhET. The feature produces speech that comes directly from the
simulation instead of using third party screen reading software. The speech can describe objects within the simulation,
contextual changes while the simulation changes, and hints that guide the user. Speech is driven by user interaction
and you will hear spoken content as you focus and activate UI components with mouse and keyboard. Because the speech only happens on interaction, the type of input (mouse/touch or keyboard/gesture) can determine what content is voiced and when it is voiced. The Voicing feature is disabled by default, and it can be enabled from the Preferences dialog.

Voicing is independent from screen reader descriptions, and we expect that a user will not be using a screen reader
while Voicing is enabled. Voicing and screen reader do not need to work well together in combination.

##### What are "Reading Blocks"?
Reading Blocks are a sub-set of the Voicing feature. When Voicing is enabled Reading Blocks are added to the sim
around elements that are not usually interactive or focusable. Reading Blocks usually surround Text, but can surround
other graphical objects. Reading blocks are added to the focus order. When the mouse is over a Reading Block a highlight
should surround the content. Moving focus to a Reading Block with keyboard or gesture or clicking on the Reading Block with mouse or touch will activate it and start speech for the content. While speaking, a yellow highlight should appear in the Reading Block highlight.

![Reading Block](https://github.com/phetsims/QA/blob/master/documentation/images/reading-block.png "Reading Block")

##### What are "Interactive Highlights"?
Interactive Highlights are another new accessibility feature. They are highlights (like focus highlights) that surround
interactive components in the sim while the mouse is over them. They serve to assist the user by clearly indicating
what is important and interactive on the screen. Voicing and Interactive Highlights are totally independent, each 
should work on their own without the other. They are disabled by default, but can be enabled from the Preferences
dialog.

![Interactive Highlights](https://github.com/phetsims/QA/blob/master/documentation/images/interactive-highlights.png "Interactive Highlights")

##### Sim Voicing Options
The Voicing feature is layerable in that the user can select what categories of content they want to hear (or have voiced out loud). These
settings should **only** apply to components within the simulation Screens. All Voicing content within dialogs,
toolbar, navigation bar, and the PhET menu should not be changed by these settings.

![Sim Voicing Options](https://github.com/phetsims/QA/blob/master/documentation/images/sim-voicing-options.png "Sim Voicing Options")

- Voice Direct object details and changes
    - This checkbox enables/disables hearing interactive object names and details when they receive focus or activation from mouse/keyboard.
- Voice other sim changes as objects change
    - This checkbox enables/disables hearing contextual changes as you interact with components in the simulation screen.
- Voice helpful hints on sim interactions
    - This checkbox will enable or disable hearing about hints for particular interactions on focus or input with mouse/keyboard. Note that not all interactions will have a hint. For example, the Reset All button does not have a hint. 

The words and phrases that are describe by the above categories are strung together and then voiced (i.e., spoken out loud) through interaction. The more checkboxes that are checked, the more a user will hear.

##### Voicing Toolbar
When Voicing is enabled, the sim can include a Toolbar that should appear on the left side of the screen. It can be 
enabled and disabled separately from Voicing from the Preferences Dialog, but it should always be disabled when
Voicing is disabled.

![Voicing Toolbar](https://github.com/phetsims/QA/blob/master/documentation/images/voicing-toolbar.png "Voicing Toolbar")

- Sim Voicing
    - The "Sim Voicing" toggle is a control that quickly enables/disables Voicing without going through the Preferences
dialog. When "Sim Voicing" is off, no Voicing content should be heard and you should not be able to find or use
any Reading Blocks. The only exception is the "Quick Info" buttons in the Toolbar. Clicking these while "Sim Voicing"
is off should still produce voicing content.

#### Additional Notes about Voicing:
- Voicing should only be available in the "en" locale. It should not be possible to enable Voicing in any other locale from Preferences.
- Voicing does not work in the Android App. In this platform, it should not be possible to enable Voicing form Preferences.

#### Sound Test

If a simulation includes sound, here are some recommendations of what to test:
- Verify that all basic UI controls create some sort of sound.
- Verify that sound is produced for all the major actions that occur in a sim.  This is unavoidably vague, since sims have so much variation, but the basic idea is to make sure that something major wasn't missed or is malfunctioning in the implementation of the sound design.
- Verify that none of the sounds produced are disproportionately loud compared to the others, i.e. the balance is good.  Note that the sound designers often use the Reset All button's sound as the volume reference.
- Play all sounds on multiple platforms and verify that there are no crackles, glitches, or anything that seems broken or significantly different on one platform versus the others.
- If the simulation supports "Enhanced Sound", test with it on and off and verify that the enhanced sounds play when this is on and don't when it is off.  You may need to consult the sound design document or ask the developer to figure out which sounds are in the "Enhanced" category.
- The sound design has gone through numerous iterations by the time it is in testing, so the sound design team is past the point of soliciting general feedback, but if a QA tester encounters something with the sound design that truly strikes them as misleading, frustrating, distracting, or otherwise problematic, it is okay to log an issue.

### 4.5: Online Website Testing

The developers may occasionally ask you to test various parts of the website. They should provide details.
Theoretically, all of the steps you follow to test the offline website could be followed for the online website.
(Obviously, some things would be different, as the website would be online instead of offline.) The
[section on website administration](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md#63-website-administration)
may contain pertinent information.

Much of this testing may be done on the ox-dev website. This way new features or large changes can be tested before
they go live on the main website. There are also three test accounts made with emails specifically for testing the
website if seperate accounts are needed. These are available on the credentials sheet. Ask Katie if you need access to
these accounts.

Things to include in website testing:
* Existing test accounts and where to get their credentials.
* Using temporary emails to test making an account.
* Ox-dev is typically used as the testing platform.
* Changes (such as submitted activities and changed/created accounts) on ox-dev do not carry over to the main site.
* Test multiple platforms and window sizes. Note the differences between mobile site layout and standard site layout.
* Test navigation using the supported screen readers and keyboard navigation.
* Make sure links work and lead to the right location.
* Make sure the animations associated with buttons, dropdown menus, and other animating features are correct.
* Make sure to test in at least 3 different languages. English, another ltr language, and an rtl language.


### 4.6: Offline Website (Installer) Testing

The offline website installers are (typically) built every Sunday morning. Test the offline website every Monday. To
test the offline website, follow the steps below:

1. Go to whichever of the following links is appropriate for the test being done.
  * https://phet.colorado.edu/installer/PhET-Installer_windows.exe
  * https://phet.colorado.edu/installer/PhET-Installer_osx.zip
  * https://phet.colorado.edu/installer/PhET-Installer_linux.bin
  * https://phet.colorado.edu/installer/PhET-Installer-with-activities_windows.exe
  * https://phet.colorado.edu/installer/PhET-Installer-with-activities_osx.zip
  * https://phet.colorado.edu/installer/PhET-Installer-with-activities_linux.bin
  * https://phet.colorado.edu/installer/PhET-Installer_cdrom.zip
  * https://phet.colorado.edu/installer/PhET-Installer_dvdrom.zip
2. Make sure the date on which the installer was built is correct, e.g. if you’re testing the simulation on a Monday,
and the installer builder was built on Sunday morning, then the date should be Monday’s date minus one day.
3. If this is not the case, then stop testing and inform the developer.
4. Otherwise, make sure the file sizes aren’t too large or too small. As of 2019-05-05, the installer without activities
is approximately 484 MB and the installer with activities is approximately 1700 MB. If these numbers are drastically
different, then stop testing and inform the developer.
  * You should alternate between Windows and macOS on a weekly basis.
  * You should alternate between browsers on a weekly basis.
  * You should alternate between the installer without activities and the installer with activities on a weekly basis.
  That is, you should not test both in one week.
  * If you download the installer with activities, index.html should exist in the `PhET` folder and in the `en` folder.
  * If you download the installer without activities, index.html should exist in the `PhET` folder and not in the `en`
  folder.
  * If you are testing the website while disconnected from the internet, the offline website should not be trying to
  connect to the internet. (There are some exceptions to this.)
  * You should have one offline website for every month of the year.
  * If you want to get rid of an offline website, delete it. Do not use the uninstaller.
5. Download the installer builder. (This is why it’s called installer testing.)
6. Install the offline website. During installation, append the file name with `_YYYY-MM-DD`
(the [correct numeric date format](https://xkcd.com/1179/)).
7. Open the offline website every way you can. (On a Windows device, the installer will create a desktop shortcut and an
application shortcut. This does not occur on macOS.)
8. Make sure the update date on the offline website matches the update date on the online website.
9. If this is not the case, then stop testing and inform the developer.
10. Otherwise, disconnect from the internet and test applicable items in the below list. (Translated Java simulations
will redirect to the website.)
  * For all versions of the installer, make sure two HTML5 simulations open.
  * For all versions of the installer, make sure two translated HTML5 simulations open.
  * For all versions of the installer, make sure two Flash simulations open.
  * For all versions of the installer, make sure two Java sims open.
  * For all versions of the installer, make sure two translated Flash sims open.
  * For all versions of the installer, make sure two translated Java sims direct to the website if you are connected to
  the internet.
  * For the installer without activities, make sure that activity links redirect you to the website if you are
  connected to the internet.
  * For the installer with activities, make sure two activities open.
  * For the installer with activities, make sure two translated activities open.
  * For the installer with activities, make sure one teacher tip opens.
11. Reconnect to the internet and test applicable items in the above list again.

You might encounter issues with Java simulations. If you are having issues with a `.jlnp` file and the developer asks
you to check the permissions of the file, then open the file with a text editor and check the permissions. If you are
having issues with a `.jar` file and the developer asks you to check the permissions, then use 
`7-Zip > Open archive > META > MANIFEST > Check permissions` to check the permissions.

If you encounter problems installing a linux installer, it is possible that it is due to the installer being 32-bit and
the computer being 64-bit. If so, follow documentation found in
[this issue](https://github.com/phetsims/installer-builder/issues/197).

### 4.7: Automated (Continuous) Testing

Open [this](https://bayes.colorado.edu/continuous-testing/aqua/html/continuous-report.html) in a private window. (You
should always use a private window when viewing automated testing results because of caching issues.) Read the
description at the top of the page. (The test number can increase because tests aren’t counted until the simulation
is built.)

The name of the server that hosts the website for automated testing is called Bayes. Automated testing is commonly
referred to as Continuous Testing (CT). When you load the website for automated testing, Bayes is always running tests
on simulations in a headless browser, i.e. a browser without a page. Bayes will pick a simulation and a test randomly.
Each test gets 40 seconds from start to finish. If the simulation takes 20 seconds to load, then it will only be tested
for 20 seconds. If the simulation takes 1 second to load, then it will be tested for 39 seconds. Once every simulation
has undergone every test, Bayes does more tests randomly. If someone makes a commit, then Bayes detects the commit,
pulls it, and takes a snapshot of the PhET codebase. This is not instantaneous. The creation of a snapshot takes
approximately 15 minutes.

The numbers and colors of the cells are important:

* Let *n* be a natural number in one of the cells.
* If *n* = 100, then there are two cases:
  * Case 1: The cell is dark green. This implies that the simulation passed all tests.
  * Case 2: The cell is light green. This implies that the simulation has passed all tests thus far.
* If 0 < *n* < 100, then some tests have failed.
  * If this is the case, then the cell is some shade of orange.
* If *n* = 0, then all tests have failed.
  * If this is the case, then the cell is red.

The color of a named cell corresponds to the color of the cell that was tested most recently in that row. If a cell is
outlined, then there are results to see. Click on the cell to view the results.

The following run unit tests. They will always have results. If they do not have results, then you should notify a
developer.

* Axon
* All PhET-iO simulations
* Balloons and Static Electricity
* Circuit Construction Kit Common
* Dot
* Kite
* PhET Core
* PhET-iO
* PhET Common
* Query String Machine
* Scenery
* Tandem

There are some common errors you should be aware of. If a simulation does not load in 40 seconds, an error is given.
If a window location changes, an error is given. If this occurs frequently, notify a developer. For other errors, make
an issue in the appropriate repository with the "type:automated-testing" and "type:bug" labels. Lint errors can be
fixed easily!

If Bayes restarts, then it takes the automated testing page a long time to show anything. Similarly, if someone tells
Bayes to start or stop doing something, then it takes a long time for things to show up on the automated testing page.
In this case, they will show up one at a time.

If you see an error, check GitHub to see who has been comitting to that repository. Notify the developer.

### 4.8: Memory Leak Testing

Memory leak testing is sometimes performed on simulations that are undergoing a development test or a release candidate
test. They should also be done for any rc.1 testing. To do a memory leak test, follow these steps:

1. Open an Incognito Window in Google Chrome.
2. Open the simulation.
3. Once the simulation has loaded, open development tools to the “Memory” tab.
4. Take a heap snapshot.
5. Append the URL with `?fuzz`.
6. Have a stopwatch ready for when you reload the simulation with the new query parameter, `?fuzz`.
7. Reload the simulation.
8. Once the simulation gets past the splash screen, start the stopwatch.
9. Every minute, for 10 minutes, take a heap snapshot.
10. While the simulation is paused and the heap snapshot is being taken, pause the stopwatch.
11. Once the simulation resumes, press resume on the stopwatch.
12. After you’ve taken 11 heap snapshots, start taking heap snapshots every 10 to 20 minutes.
13. Stop taking heap snapshots when you feel you have collected sufficient data.

### 4.9: Maintenance Release Testing

This type of test is done when a relatively small change needs to be made to multiple sims. What needs to be tested will
vary depending on the change, and is determined by the developer in charge of the release. Generally, there will be a
list of links to sims to test. Each will involve a short check to make sure nothing was broken by the change, and other
tests that will be described in the issue. For the PhET-iO sims, older versions labeled "instance proxies" may not work,
particularly when looking at the “launch” button. Exploring changes to the sim should still work.

Be aware of what sims are being tested. If anything looks out of place, be sure to notify the developers. In particular,
sims currently in RC testing may need special attention.

### 4.10: PhETTest

[PhETTest](https://bayes.colorado.edu/dev/phettest/) contains up-to-date versions of the sim with latest code changes made by the
developers. When a developer asks for something to be checked on master, this is where you will go to do that for the
most part. PhETMarks serves a similar purpose with more options in case you need to test something more involved like
PhET-iO. When you open the website, do so in incognito mode to ensure you aren’t looking at an old version of a sim.
Make sure all of the common code repos are up to date, as well as the sim you want to look at. You can press the "pull"
button to update one repo, or the "Pull All" button at the top to update everything. To quickly check a sim, click the
link with the sim in the title. To build a version of the simulation, click "build", and then click "Built
Version" when the process finishes.

### 4.11: App Testing

PhET has an iOS app, and as of 2020-07-01, we're developing an Android app.

#### iOS App Testing

There isn't a rigorous process for testing the app. We try to manually test each feature and look for anything out of
ordinary, kind of like a dev test for a simulation.

##### App Translation Testing

Add steps for translating the app here!

#### Android App Testing

We haven't had to test the Android app yet, but the process will probably be similar to the process for testing the iOS

***

## Section 5: Translations

One of PhET’s goals is to make our simulations available to everyone in the world. It wouldn’t be possible to do this
without the help of volunteers who translate our simulations and the website.

### 5.1: Legacy Simulation Translations

We have lots of old simulations that use Adobe Flash Player or Java. People still use these translations, so they’re
still being translated. To translate a Flash or Java simulation, do the following:

1. Log in to Gmail as phethelp@gmail.com on Hanson.
2. Download all `.xml` (Flash) and `.properties` (Java) files.
3. Move these files to the “Translations” folder.
4. Open
[this spreadsheet](https://docs.google.com/spreadsheets/d/10co5pwJI6HaJq6RD7fX2xVm3Ks1WpYfXei9scnPGKxM/edit?pli=1#gid=0).
5. Enter relevant information into the spreadsheet.
6. Open the Git Bash shortcut on Hanson's Desktop.
7. Wait for it to load.
8. Click the “Translations” tab.
9. Click “Deploy Simulation Translations" and read each message that you see after this step carefully.
10. Enter your CU IdentiKey credentials.
11. Enter the file path for the “Translations” folder.
12. Commit the files that are not updated.
13. Copy and paste the relevant information from the spreadsheet into each commit message.
14. Click the “OK” button.
15. Wait for it to complete.
16. Click the "OK" button. 
17. Copy the URL from Git Bash and paste it into a browser.  URL should look like
`https://phet.colorado.edu/admin/deploy-translation?dir=`...
18. Wait for it to load.
19. Test the English version and the translated version of each simulation. (Make sure the strings look normal.)
20. If the strings look normal, then press the "Publish Now" button.
21. Send an email to the translator with a link to the page on the PhET website where their newly translated
simulations can be found.
22. Delete the contents of the “Translations” folder.
23. Send the translator a thank-you email.

Note:

* This process will not work if Matt hasn't done some wizardry to make it so that you can do it.
* If something goes wrong at any point in the process, the best course of action is to start over.

### 5.2: HTML5 Simulation Translations

HTML5 simulation translations are submitted to the website by trusted translators. The new translation of the simulation
is then automatically uploaded to the website.

Rosetta is the program we use to translate HTML5 simulations. A trusted translator logs in to the website, does all of
his or her translations in the browser, and then he or she clicks submit. Rosetta then sends these string files to
Babel. Babel then builds a new simulation with the new strings.

### 5.3: Website Translations

#### Update Case

A translator submits an update of an existing translation. Go to the Translations page and click the update button next
to the corresponding language. Send the translator a thank-you email.

#### Creates New Language Case

Send this email:

"Dear Translator,

I've noticed that you recently started a Divehi (dv) translation of our website and wanted to check in with you to see
if you have any questions about the process. Please let me know if you have any questions about how this works and of
course please read the full instructions page prior to starting your translation:

https://phet.colorado.edu/en/for-translators/website

As I'm sure you've realized at this point translating the website is not a small task. We estimate it will probably
take about 50 - 100 hours to fully make a website translation. Because of this, and because we will only provide one
public translation per language, we encourage translators to collaborate on a translation for their language. We want
translators to work together to move any partial translations to one "master" translation as only one translation will
go public.

Thank you for your efforts to make PhET sims available worldwide.

Sincerely,

PhET Help"

#### Submits New Language Case

First, check to see how many strings the new translation has. We generally only will publish translation that have more
than 1000 strings translated.

If it has more than 1000, make the translation visible. Make sure no one else is working on the translation. It would
likely be better if approaches 2000.

Otherwise tell the translator we don’t normally publish incomplete translations and to submit once they have translated
more than 1000 strings:

"Dear Translator,

I've noticed that you recently started a Gujarati (gu) translation of our website and wanted to check in with you to
see if you have any questions about the process. Please let me know if you have any questions about how this works and
of course please read the full instructions page prior to starting your translation:

https://phet.colorado.edu/en/for-translators/website

As I'm sure you've realized at this point translating the website is not a small task. We estimate it will probably
take about 50 - 100 hours to fully make a website translation. Because of this, and because we will only provide one
public translation per language, we encourage translators to collaborate on a translation for their language. We want
translators to work together to move any partial translations to one "master" translation as only one translation will
go public.

Also, we typically only publish translations once they reach at least 1000 strings because before that point they
aren't completely usable. You do not need to submit your translation to save your work. All changes are automatically
saved to our servers.

Thank you for your efforts to make PhET sims available worldwide.

Sincerely,

PhET Help"

#### Delete Case

The translator creates or submits an English translation. This should never happen because our website is already in
English. Delete the (en) copy they created. Be careful not to delete the original English for the website.

Send this email:

"Dear translator,

I noticed that you recently started an English (en) translation of our website. Since our website is written in
English, we will delete this translation. If you meant to create a translation in another language, please see here for
instructions:

https://phet.colorado.edu/en/for-translators/website

Best,

PhET Help"

#### Created Copy Case

The translator creates a copy an existing translation.

Email them informing them of the existing translation:

"Dear Translator,

I've noticed that you recently started an Arabic (ar) translation of our website and wanted to check in with you to see
if you have any questions about the process.  Please let me know if you have any questions about how this works and of
course please read the full instructions page prior to starting your translation:

https://phet.colorado.edu/en/for-translators/website

As I'm sure you've realized at this point translating the website is not a small task. We estimate it will probably
take about 50 - 100 hours to fully make a website translation. Because of this, and because we will only provide one
public translation per language, we encourage translators to collaborate on a translation for their language. We want 
translators to work together to move any partial translations to one "master" translation as only one translation will
go public.

Since there are already multiple Arabic (ar) translations being worked on, I would encourage you to send a request to
collaborate on the translation by clicking "request to collaborate". This will allow you to send an email to the
translators with your email address, so they can contact you about collaboration.

Thank you for your efforts to make PhET sims available worldwide.

Sincerely,

PhET Help"

#### Submitted Clone Case

The translator submits a clone of an existing translation.

Email the translator letting them know that we already have a translation in that language (provide URL) and ask them
to instead “Request Collaboration” on the existing translation.

#### Other Possible Cases

If you feel that a translation does not fit one of these cases for one reason or another, ask Katie. Oliver may also be
able to help, especially if a decision about publishing needs to be made.

***

## Section 6: Maintenance & Management

There are a couple miscellaneous tasks related to maintenance and management that QA gets to deal with.

### 6.1: Testing Matrix Management

Every time we do a release candidate test, you have to make a testing matrix. To do so, follow these steps:

1. If the simulation hasn’t undergone a release candidate test, then you’ll need to create a new testing matrix. Go to
Google Drive and then `PhET Files > PhET QA > Testing Matrices` to find example matrices. Make a copy of the correct
testing matrix by clicking `File > Make a copy...`. Do not copy and paste the test matrix.
2. Otherwise, create a new tab in the existing spreadsheet for the simulation for the release candidate test.
3. Copy and paste URLs into the testing matrix.
4. Do the “Yes” or “No” for Legends of Learning, Keyboard Navigation, and Screen Reader.
5. Edit the URLs in the GitHub issue.

When platforms are added or dropped the testing matrix needs to be updated to reflect the new support. To do so, keep
these things in mind:

1. Many of the parts of the matrix depend on condition formatting and functions.
2. Before making edits, make a copy of the old test matrix in case something goes wrong (by right clicking the sheet
tab).
3. Do some tests filling out the matrix to make sure everything adds up correctly.

### 6.2: PhET Test Maintenance

PhETTest runs on bayes, see https://github.com/phetsims/phetmarks/blob/master/phettest/README.md for notes about maintaining the associated processes. This
requires the ability to ssh into bayes with the `phet-admin` account. If you see something like 
”failed to pull,” then look through bayes logs to see if you can find the culprit. Every time a new repository
is made, press the “Refresh Perennial” button. (Perennial is the list of simulations.) Press the ”Pull All” button
every 5 hours.

Here is a list of helpful commands:

* `$ pm2 stop phettest-server`
* `$ pm2 start phettest-server`
* `$ pm2 logs phettest-server`

Since phettest now runs on bayes, rather than the Turing computer, you are generally better off asking a developer 
for help in using these commands and/or troubleshooting.

### 6.3: Website Administration

Do not delete English versions of simulations!

There are three servers:

1. [Ox-Dev](https://ox-dev.colorado.edu/): This is the development server. It’s kind of like a playground. You can do
whatever you want to the website on this server.
  * Ox-Dev has to be manually synced with the website. (This is not something that you will have to do.)
  * Because Ox-Dev has to be manually synced with the website, it might be missing certain things.
  * Accounts created on Ox-Dev are deleted when Ox-Dev gets synced with the website, so make as many accounts as you’d
  like.
2. [Bayes](https://bayes.colorado.edu/): This server has multiple functions. It is the disaster recovery server and it
does automated testing, among other things.
3. [Figaro](https://phet.colorado.edu/): This server is also known as phet-server. This is the server on which
https://phet.colorado.edu runs.

To get to the administrative page of the website, sign in and click the “Administration” button in the upper-right
corner.

* “Help Center” is where helpful information that we post on the website is added, removed, or edited.
* “Edit Content Page” is where English strings for the website and the simulations can be edited.
* “Team Page” is where team members and their descriptions can be added, removed, or edited.
* “Asks Data Page” is to be ignored.
* “Simulations” is where flavors, projects, and simulations are listed. Do not click the remove link! Once a simulation
is published, ask the relevant designer(s) to fill in the flavor information for that simulation. Each flavor has a
checkbox for visibility. Do not check this checkbox without permission from the relevant designer(s).
* “Projects” is the same thing as the list of projects in “Simulations.”
* “Categories” is to be ignored.
* “Activities” is a comprehensive list of activities. It also contains activities that are pending approval.
* To test “Activities,” make all sorts of different files to submit, and submit them. If you aren’t logged in as a team
member or if you aren’t an administrator, then you shouldn’t be able to see the activities you’ve submitted. Make sure
this is the case. Make sure you can download and use all activities.
* If you are testing “Activities” and you are logged in as a team member, then you should see the red box. If you are
testing “Activities” and you are not logged in, you should not see the red box.
* “Notifications” is a list of notifications for updated activities.
* “Users” is where user accounts can be added, removed, or edited.
* “Metadata” is to be ignored.
* “Translations” is for translations.
* “FAQs” is to be ignored.
* “Strings” is to be ignored.
* “Caches and Search Index” is to be ignored.
* “Statistics” is where we record useful statistics.
* “Documentation and Help” is to be ignored.
* “Schools” is where our list of schools maintained.
* “Organizations” is where our list of organizations is maintained.

### 6.4: QA Book Maintenance

Please keep this book up-to-date so that it can be a useful resource!

Use this [Markdown File](https://github.com/phetsims/QA/blob/master/doc/qa-book-maintenance.md) to record things that
need to be added and to view dates for scheduled maintenance.

***

