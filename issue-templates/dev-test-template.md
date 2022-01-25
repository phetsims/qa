<!---

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~ PhET Development Test Template ~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Notes and Instructions for Developers:
  1. Comments indicate whether something can be omitted or edited.
  2. Please check the comments before trying to omit or edit something.
  3. Please don't rearrange the sections.

-->

@relevantPerson1, @relevantPerson2, simulation-name/#.#.#-dev.# is ready for dev testing. [List deadlines and whether
this will be shared with a client.] Document issues in https://github.com/phetsims/{{REPO}}/issues and link to this
issue. [If the test is delayed until QA is more open, state that here.]

Assigning @kathy-phet and @KatieWoe for prioritization.


<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 1: General Dev Testing [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>General Dev Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Click every single button.
- If there is sound, make sure it works.
- Make sure you can't lose anything.
- Play with the sim normally.
- Try to break the sim.
- Try to include browser version numbers
- If there is a console available, check for errors and include them in the Problem Description.
- Run through the string tests on at least one platform, especially if it is about to go to rc.
- Check the Game Up harness on one platform.


<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested,
list them here. Any behaviors you want QA to pay special attention to should be listed here.]

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>General Dev Test Platforms</h3>
  
  Please include (non-screen reader) a11y testing in these records if applicable.

- [ ] Latest macOS, Safari (Time = )
- [ ] Windows 10, Chrome (Time = )
- [ ] Windows 10, Firefox (Time = )
- [ ] Latest iOS, Safari (Time = )
- [ ] Windows 11, Chrome (Time = )

Light testing, or optionally skip if time crunch: 
- [ ] Latest macOS, Chrome (Time = )
- [ ] Latest Chrome OS, Chrome (Time = )

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have either use the labels "status:ready-for-qa" or "status:ready-for-review." If it is ready for
QA then close the issue if fixed. If ready for review then leave open and assign back to the developer.

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>Link(s)</h3>

- **[Simulation](all_phet_link)**

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 2: PhET-iO Dev Test [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>PhET-iO Dev Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Make sure that public files do not have password protection. Use a private browser for this.
- Make sure that private files do have password protection. Use a private browser for this.
- Make sure standalone sim is working properly.
- Make sure the wrapper index is working properly.
- Make sure each wrapper is working properly.
- Launch the simulation in Studio with ?stringTest=xss and make sure the sim doesn't navigate to youtube
- For newer PhET-iO wrapper indices, save the "basic example of a functional wrapper" as a .html file and open it. Make
sure the simulation loads without crashing or throwing errors.

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>General Dev Test Platforms</h3>

- [ ] Latest macOS, Safari (Time = )
- [ ] Latest iOS, Safari (Time = )
- [ ] Windows 10, Chrome (Time = )
- [ ] Windows 10, Firefox (Time = )
- [ ] Windows 11, Chrome (Time = )
- [ ] Latest Chrome OS, Chrome (Time = )

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested,
list them here. Any behaviors you want QA to pay special attention to should be listed here. This includes if any substantial, 
untested work has been implemented in PhET-iO wrappers or in the PhET-iO Engine since last PhET-iO test.]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have either use the labels "status:ready-for-qa" or "status:ready-for-review." If it is ready for QA
then close the issue if fixed. If ready for review then leave open and assign back to the developer.

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>Link(s)</h3>

- **[Wrapper Index](link)**

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 3: For Accessibility (a11y) Dev Test [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>Accessibility (a11y) Dev Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Specific instructions can be found below. Please include time in the general section and check those off when a11y testing has also been done.
- Make sure the accessibility-related feature that is being tested doesn't negatively affect the sim in any way. Here is a list of features to supported in this test: <!--- PRUNE THIS LIST AS APPROPRIATE -->
  - Alternative Input
  - Interactive Description
  - Sound and Sonification
  - Pan and Zoom
  - Mobile Description
  - Voicing
  - Load the a11y view and make sure that interacting with all elements in the simulation updates the appropriate descriptions in the PDOM.

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested,
list them here. Any behaviors you want QA to pay special attention to should be listed here.]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have either use the labels "status:ready-for-qa" or "status:ready-for-review." If it is ready for
QA then close the issue if fixed. If ready for review then leave open and assign back to the developer.

<!--- [DO NOT OMIT, SHOULD BE EDITED] -->
<h3>Link(s)</h3>

- **[a11y View](link)**
- **[Simulation](all_phet_link)**

<!--- [CAN BE OMITTED, DO NOT EDIT] -->
<h3>Screen Readers</h3>

This sim supports screen readers. If you are unfamiliar with screen readers, please ask Katie to introduce you to screen
readers. If you simply need a refresher on screen readers, please consult the
[QA Book](https://github.com/phetsims/QA/blob/master/documentation/qa-book.md), which should have all of
the information you need as well as a link to a screen reader tutorial made by Jesse. Otherwise, look over the a11y view
before opening the simulation. Once you've done that, open the simulation and make sure alerts and descriptions work as
intended.

<!--- [CAN BE OMITTED, CAN BE EDITED] -->
<h3>Platforms and Screen Readers to Be Tested</h3>

- [ ] Windows 10 + Latest Chrome + Latest JAWS (Time = )
- [ ] Windows 10 + Latest Firefox + Latest NVDA (Time = )
- [ ] macOS + Safari + VoiceOver (Time = )
- [ ] iOS + Safari + VoiceOver (May or may not be supported) (Time = )

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

- [ ] If this sim is being tested for a11y we may want to do some testing on Talkback to check on latest behavior of
that screen reader. Please comment in the issue asking if Talkback should be tested. See
https://github.com/phetsims/a11y-research/issues/144.

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
