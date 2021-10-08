<!---

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~ PhET Research Release Candidate Test Template ~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Notes and Instructions for Developers:
  1. Comments indicate whether something can be omitted or edited. 
  2. Please check the comments before trying to omit or edit something.
  3. Please don't rearrange the sections.

-->

@relevantPerson1, @relevantPerson2, simulation-name/#.#.#-rc.# is ready for RC Research testing. [List deadlines and whether
this will be shared with a client.] Document issues in https://github.com/phetsims/{{REPO}}/issues and link to this
issue. [If this rc is delayed until QA is more open, state that here.]

[Use this section to describe research focus and what aspects need QA focus.]

[Use this section to describe what platforms, if different from norm, should be tested.]

Assigning to @kathy-phet and @KatieWoe for prioritization.

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 1: General RC Testing [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>General RC-research Test</b></summary>

<!--- [DO NOT OMIT, SHOULD BE EDITED] -->
<h3>What to Test</h3>

[Specify a bullet list for things that are relevant for the research study.]

[Identify query parameters that will be used in the research.]

- Click every single button.
- Test all possible forms of input.
  - Test all mouse/trackpad inputs.
  - Test all touchscreen inputs.
- If there is sound, make sure it works.
- Make sure you can't lose anything.
- Play with the sim normally.
- Try to break the sim.
- When making an issue, check to see if it was in a previously published version
- Try to include version numbers for browsers
- If there is a console available, check for errors and include them in the Problem Description.
- As an RC begins and ends, check the sim repo. If there is a maintenance issue, check it and notify developers if
there is a problem.

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested,
list them here. Any behaviors you want QA to pay special attention to should be listed here.]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have the "status:ready-for-qa" label. Check these issues off and close them if they are fixed.
Otherwise, post a comment in the issue saying that it wasn't fixed and link back to this issue. If the label is
"status:ready-for-review" or "status:fixed-pending-deploy" then assign back to the developer when done, even if fixed.

<!--- [CAN BE OMITTED, CAN BE EDITED] -->
<h3>Platforms and Browsers to Be Tested</h3>

[ideally test the platforms that are relevant to the research study, otherwise use this default list]
- [ ] Windows 10 + Latest Chrome (Time = )
- [ ] Windows 10 + Latest Firefox (Time = )
- [ ] macOS + Safari (Time = )
- [ ] macOS + Chrome (Time = )
- [ ] iOS + Safari (Time = )
- [ ] ChromeOS + Chrome (Time = )

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>Link(s)</h3>

- **[Simulation](all_phet_link)**
- **[iFrame](all_iframe_link)**
- **[XHTML](link)**

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 2: PhET-iO RC Test [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>PhET-iO RC-research Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

[Specify which wrappers to test.]
[Specify if links should be public if they are normally private.]
[Often PhET-iO research studies involve Metacog recording, use this bullet if applicable: Conduct a recording test to Metacog, further instructions in the QA Book.]

- Make sure standalone sim is working properly.
- Make sure the wrapper index is working properly.

<!--- [CAN BE
OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested,
list them here. Any behaviors you want QA to pay special attention to should be listed here. This includes if any substantial, 
untested work has been implemented in PhET-iO wrappers or in the PhET-iO Engine since last PhET-iO test.]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have the "status:ready-for-qa" label. Check these issues off and close them if they are fixed.
Otherwise, post a comment in the issue saying that it wasn't fixed and link back to this issue. If the label is
"status:ready-for-review" or "status:fixed-pending-deploy" then assign back to the developer when done, even if fixed.

<!--- [DO NOT OMIT, SHOULD BE EDITED] -->
<h3>Link(s)</h3>

- **[Wrapper Index](link)**
[Insert study links here]

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 3: For Accessibility (a11y) RC Test [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>Accessibility (a11y) RC-research Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Specific instructions can be found below.
- Make sure the accessibility-related feature that is being tested doesn't negatively affect the sim in any way. Here is a list of features to supported in this test: <!--- PRUNE THIS LIST AS APPROPRIATE -->
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

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested,
list them here. Any behaviors you want QA to pay special attention to should be listed here.]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have the "status:ready-for-qa" label. Check these issues off and close them if they are fixed.
Otherwise, post a comment in the issue saying that it wasn't fixed and link back to this issue. If the label is
"status:ready-for-review" or "status:fixed-pending-deploy" then assign back to the developer when done, even if fixed.

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>Link(s)</h3>

- **[a11y View](link)**
- **[Simulation](all_phet_link)**

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
