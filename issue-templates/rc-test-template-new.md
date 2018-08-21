<!---

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~ PhET Release Candidate Test Template ~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Notes and Instructions for Developers:
  1. Comments indicate whether something can be omitted or edited. 
  2. Please check the comments before trying to omit or edit something.
  3. Please don't rearrange the sections.

-->

@relevantPerson1, @relevantPerson2, simulation-name/#.#.#-rc.# is ready for RC testing. [List deadlines and whether this will be shared with a client.] Document issues in https://github.com/phetsims/{{REPO}}/issues and link to this issue.

Assigning @ariel-phet for prioritization.

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////// Section 0: FAQs for QA Members [DO NOT OMIT, DO NOT EDIT]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>FAQs for QA Members</b></summary>

<br>
  
  <!--- Subsection 0.1: There are multiple tests in this issue... What should I test first? [DO NOT OMIT, DO NOT EDIT] -->

  <details>
  <summary><i>There are multiple tests in this issue... Which test should I do first?</i></summary> 
  
  Test in order! Test the first thing first, the second thing second, and so on.

  </details>

  <br>

  <!--- Subsection 0.2: How should I format my issue? [DO NOT OMIT, DO NOT EDIT] -->

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

  <!--- Subsection 0.3: Who should I assign? [DO NOT OMIT, DO NOT EDIT] -->

  <details>
  <summary><i>Who should I assign?</i></summary>
  
  We typically assign the developer who opened the issue in the QA repository.

  </details>
  
  <br>

  <!--- Subsection 0.4: My question isn't in here... What should I do? [DO NOT OMIT, DO NOT EDIT] -->

  <details>
  <summary><i>My question isn't in here... What should I do?</i></summary>
  
  You should:

  1. Consult the [QA Book](link).
  2. Google it.
  3. Ask Katie.
  4. Ask a developer.
  5. Google it again.
  6. Cry.

  </details>

<br>

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////// Section 1: General RC Testing [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>General RC Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Click every single button.
- If there is sound, make sure it works.
- Make sure you can't lose anything.
- Play with the sim normally.
- Try to break the sim.
- Test all query parameters on all platforms. (See QA book for a list of query parameters.)
- Download HTML on Chrome and iOS.
- Make sure the iFrame version of the simulation is working as intended on all platforms.
- Make sure the XHTML version of the simulation is working as intended on all platforms.
- Complete the test matrix.
- Don't forget to make sure the sim works with Legends of Learning.

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested, list them here. Any behaviors you want QA to pay special attention to should be listed here.]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have the "status:fixed-pending-testing" label. Check these issues off and close them if they are fixed. Otherwise, post a comment in the issue saying that it wasn't fixed.

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>Link(s)</h3>

- **[Simulation](link)**
- **[iFrame](link)**
- **[XHTML](link)**
- **[Test Matrix](link)**
- **[Legends of Learning Harness](harness.legendsoflearning.com)**

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////// Section 2: PhET-iO RC Test [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>PhET-iO RC Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Make sure that public files do not have password protection. Use a private browser for this.
- Make sure that private files do have password protection. Use a private browser for this.
- Make sure standalone simulation is working properly.
- Make sure the wrapper index is working properly.
- Make sure each wrapper is working properly.
- For newer PhET-iO wrapper indicies, save the "basic example of a functional wrapper" as a .html file and open it. Make sure the simulation loads without crashing or throwing errors.

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested, list them here. Any behaviors you want QA to pay special attention to should be listed here.]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have the "status:fixed-pending-testing" label. Check these issues off and close them if they are fixed. Otherwise, post a comment in the issue saying that it wasn't fixed.

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>Link(s)</h3>

- **[Wrapper Index](link)**
- **[Test Matrix](link)**

<hr>

</details>

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////// Section 3: For Accessibility (a11y) RC Test [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>Accessibility (a11y) RC Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Specific instructions can be found below.
- Make sure the a11y feature doesn't negatively affect the sim in any way.

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. If you have any further tests you want done or specific platforms you want tested, list them here. Any behaviors you want QA to pay special attention to should be listed here.]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Issues to Verify</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have the "status:fixed-pending-testing" label. Check these issues off and close them if they are fixed. Otherwise, post a comment in the issue saying that it wasn't fixed.

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>Link(s)</h3>

- **[a11y View](link)**
- **[Simulation](link)**
- **[Test Matrix](link)**

<!--- [CAN BE OMITTED, DO NOT EDIT] -->
<h3>Screen Readers</h3>

This sim supports screen readers. Look over the a11y view before opening the simulation. Once you've done that, open the simulation and make sure alerts and descriptions work as intende
<!--- [CAN BE OMITTED, CAN BE EDITED] -->
<h3>Platforms and Screen Readers to Be Tested</h3>

- [ ] Windows 10 + Latest Firefox + Latest JAWS
- [ ] Windows 10 + Latest Firefox + Latest NVDA
- [ ] macOS + Safari + VoiceOver

<!--- [CAN BE OMITTED, CAN BE EDITED] -->
<h3>Critical Screen Reader Information</h3>

We are tracking known screen reader bugs in [this Google Document](https://docs.google.com/document/d/1518zv6F0odExFsodShZxwTmWNQk3civuNwtQUR-rEBs/). If you find a screen reader bug, please check it against this list.

<!--- [CAN BE OMITTED, CAN BE EDITED] -->
<h3>Keyboard Navigation</h3>

This sim supports keyboard navigation. Please make sure it works as intended on all platforms by itself and with a screen reader.

<hr>

</details>
