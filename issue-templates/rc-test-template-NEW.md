<!---
DEVELOPERS: 
* Fill in the placeholders that look like {{TOKEN}}.
* Delete things that are not relevant, e.g. PhET-iO links for non-PhET-iO tests.
-->

<h1>RC Test</h1>

<h3>Simulation links</h3>

- [GitHub repository for issues]({{GITHUB_REPOSITORY_LINK}})
- [phet directory]({{PHET_DIRECTORY_LINK}})
- [all.html]({{ALL_HTML_LINK}})
- [phet-io directory]({{PHET_IO_DIRECTORY_LINK}})
- [Wrapper Index]({{WRAPPER_INDEX_LINK}})

<h3>Test Matricies</h3>

- [General Test Matrix](FILLED_IN_BY_QA)
- [PhET-iO Test Matrix](FILLED_IN_BY_QA)

<h3>Features included</h3>

- [ ] PhET-iO
- [ ] Alternative Input
- [ ] Sound
- [ ] Description
- [ ] Voicing

<h3>Focus and Special Instructions</h3>

<!---
Things to include here:
* purpose/focus of the test
* milestones
* specific things to test
* specific platforms to test
* instructions for any non-standard tests
* If you want PhET-iO diff wrapper tested against a prior version, provide details and link to prior version.
-->

<h3>Issues to Verify†</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

†These issues should have the "status:ready-for-review" label. Unless the issues says to close after verifying, 
assign the issue back to the developer. 

---
<h2>For QA...</h2>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// General RC Testing instructions
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>General features</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Click every single button.
- Test all possible forms of input.
  - Test all mouse/trackpad inputs.
  - Test all touchscreen inputs.
- If there is sound, make sure it works.
- Make sure you can't lose anything.
- Play with the sim normally.
- Try to break the sim.
- Test all query parameters on all platforms. (See [QA Book](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md) for a list of query parameters.)
- Download HTML on Chrome and iOS.
- Make sure the iFrame version of the simulation is working as intended on all platforms.
- Make sure the XHTML version of the simulation is working as intended on all platforms.
- Complete the test matrix.
- Don't forget to make sure the sim works with Legends of Learning.
- Test the Game Up harness on at least one platform.
- Check [this](https://docs.google.com/spreadsheets/d/1umIAmhn89WN1nzcHKhYJcv-n3Oj6ps1wITc-CjWYytE/edit#gid=0) LoL
spreadsheet and notify AR or AM if it not there.
- If this is rc.1 please do a memory test.
- When making an issue, check to see if it was in a previously published version.
- Try to include version numbers for browsers.
- If there is a console available, check for errors and include them in the Problem Description.
- As an RC begins and ends, check the sim repo. If there is a maintenance issue, check it and notify developers if there is a problem.

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// PhET-iO RC Test instructions
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>PhET-iO features/b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Make sure that public files do not have password protection. Use a private browser for this.
- Make sure that private files do have password protection. Use a private browser for this.
- Make sure standalone sim is working properly.
- Make sure the wrapper index is working properly.
- Make sure each wrapper is working properly.
- Launch the simulation in Studio with ?stringTest=xss and make sure the sim doesn't navigate to youtube
- For newer PhET-iO wrapper indices, save the "basic example of a functional wrapper" as a .html file and open it. Make sure the simulation loads without crashing or throwing errors.
- Load the login wrapper just to make sure it works. Do so by adding this link from the sim deployed root: 
  ```
  /wrappers/login/?wrapper=record&validationRule=validateDigits&&numberOfDigits=5&promptText=ENTER_A_5_DIGIT_NUMBER
  ```   
  Further instructions in QA Book
- Conduct a recording test to Metacog, further instructions in the QA Book. Do this for iPadOS + Safari and one other random platform.
- Conduct a memory test on the stand alone sim wrapper (rc.1).
- Test one platform combination with `?phetioDebug` on the Studio and State wrapper.
- If Pan/Zoom is supported, make sure that it works when set with PhET-iO State.
- Test that the sim works offline:
  * Download the `SIM-phet-io-VERSION.zip` file from `phet-io` directory link above.
  * Unzip it to a spot locally.
  * Open `index.html` by double clicking it on your desktop or in a Finder-view.
  * It should look like the standalone version of the sim in PhET-iO brand.

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 3: For Accessibility (a11y) RC Test [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>Accessibility features</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Specific instructions can be found below.
- Make sure the accessibility (a11y) feature that is being tested doesn't negatively affect the sim in any way. Here is a list of features to supported in this test: <!--- PRUNE THIS LIST AS APPROPRIATE -->
  - Alternative Input
  - Interactive Description
  - Sound and Sonification
  - Pan and Zoom
  - Mobile Description
  - Voicing
- Test all possible forms of input.
  - Test all mouse/trackpad inputs.
  - Test all touchscreen inputs.
  - Test all keyboard navigation inputs (if applicable).
  - Test all forms of input with a screen reader (if applicable).

<!--- [CAN BE OMITTED, DO NOT EDIT] -->
<h3>Screen Readers</h3>

This sim supports screen readers. If you are unfamiliar with screen readers, please ask Katie to introduce you to
screen readers. If you simply need a refresher on screen readers, please consult the
[QA Book](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md), which should have
all of the information you need as well as a link to a screen reader tutorial made by Jesse. Otherwise, look over the
a11y view before opening the simulation. Once you've done that, open the simulation and make sure alerts and
descriptions work as intended.

<!--- [CAN BE OMITTED, CAN BE EDITED] -->
<h3>Platforms and Screen Readers to Be Tested</h3>

- [ ] Windows 10 + Latest Chrome + Latest JAWS
- [ ] Windows 10 + Latest Firefox + Latest NVDA
- [ ] macOS + Safari + VoiceOver
- [ ] iOS + Safari + VoiceOver (only if specified in testing issue)

<!--- [CAN BE OMITTED, CAN BE EDITED] -->
<h3>Critical Screen Reader Information</h3>

We are tracking known screen reader bugs in
[this Google Document](https://drive.google.com/open?id=12kTs-g-iKEIH1dyG7Q41_W_oNL4gUKbkW-IQgZjMUBw). If you find a
screen reader bug, please check it against this list.

<!--- [CAN BE OMITTED, CAN BE EDITED] -->
<h3>Keyboard Navigation</h3>

This sim supports keyboard navigation. Please make sure it works as intended on all platforms by itself and with a
screen reader.

<h3>Magnification</h3>

This sim supports magnification with pinch and drag gestures on touch screens, keyboard shortcuts, and mouse/wheel controls. Please test magnfication and make sure
it is working as intended and well with the use cases of the simulation. Due to the way screen readers handle user input, magnification is NOT expected to
work while using a screen reader so there is no need to test this case.

<h3>Final Requests</h3>

- [ ] If this sim is not in [this list](https://phet.colorado.edu/en/accessibility/prototypes) or up to date there, make an
issue in [website](https://github.com/phetsims/website) to ask if PhET research page links need updating. Please assign
to @terracoda and @emily-phet.

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 4: FAQs for QA Members [DO NOT OMIT, DO NOT EDIT]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>FAQs for QA Members</b></summary>

<br>
  
  <!--- [DO NOT OMIT, DO NOT EDIT] -->

  <details>
  <summary><i>There are multiple tests in this issue... Which test should I do first?</i></summary> 
  
  Test in order! Test the first thing first, the second thing second, and so on.

  </details>

  <br>

  <!--- [DO NOT OMIT, DO NOT EDIT] -->

  <details>
  <summary><i>How should I format my issue?</i></summary>
  
  Here's a template for making issues:

      <b>Test Device</b>

      blah

      <b>Operating System</b>

      blah

      <b>Browser</b>

      blah

      <b>Problem Description</b>

      blah

      <b>Steps to Reproduce</b>

      blah

      <b>Visuals</b>

      blah

      <details>
      <summary><b>Troubleshooting Information</b></summary>

      blah

      </details>

  </details>

  <br>

  <!--- [DO NOT OMIT, DO NOT EDIT] -->

  <details>
  <summary><i>Who should I assign?</i></summary>
  
  We typically assign the developer who opened the issue in the QA repository.

  </details>
  
  <br>

  <!--- [DO NOT OMIT, DO NOT EDIT] -->

  <details>
  <summary><i>My question isn't in here... What should I do?</i></summary>
  
  You should:

  1. Consult the [QA Book](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md).
  2. Google it.
  3. Ask Katie.
  4. Ask a developer.
  5. Google it again.
  6. Cry.

  </details>

<br>

<hr>

</details>