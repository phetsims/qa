<!---

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~ PhET Prototype Release Candidate Test Template ~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Notes and Instructions for Developers:
  1. Comments indicate whether something can be omitted or edited. 
  2. Please check the comments before trying to omit or edit something.
  3. Please don't rearrange the sections.

-->

@relevantPerson1, @relevantPerson2, simulation-name/#.#.#-rc.# is ready for prototype testing. This simulation will be
put on the website as a prototype and will likely have more bugs than a publication-ready simulation. Document issues in 
https://github.com/phetsims/{{REPO}}/issues and link to this issue. **Issues should focus on base usability and pedagogy.**

Assigning to @ariel-phet for prioritization.

<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// Section 1: Prototype Testing [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED]
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<details>
<summary><b>General RC Test</b></summary>

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>What to Test</h3>

- Play with the simulation normally.
- Make sure you can't lose anything.
- Complete the test matrix.
- Try to include version numbers for browsers
- If there is a console available, check for errors and include them in the Problem Description.
- Focus on pedagogy issues and bugs that break the sim. 
- If you find bugs beyond pedagogy/breaking, still document these bugs as github issues.
- If a11y aspects are present, test them, but with an eye for "normal use".

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Focus and Special Instructions</h3>

[Provide further instructions here. Any aspects or requests not included elsewhere can be included here]

<!--- [CAN BE OMITTED, SHOULD BE EDITED IF NOT OMITTED] -->
<h3>Known Issues</h3>

- [ ] [Issue1](link)
- [ ] [Issue2](link)
- [ ] [Issue3](link)

These issues should have the "status:ready-for-qa" label if they are fixed. Check these issues off and close them if they are fixed.
Otherwise, post a comment in the issue saying that it wasn't fixed and link back to this issue. Most of these issues will not be fixed 
at this point, just be aware of them as you test.

<!--- [DO NOT OMIT, CAN BE EDITED] -->
<h3>Link(s)</h3>

- **[Simulation](all_phet_link)**
- **[Test Matrix](link)**

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

  1. Consult the [QA Book](https://github.com/phetsims/QA/blob/master/doc/qa-book.md).
  2. Google it.
  3. Ask Katie.
  4. Ask a developer.
  5. Google it again.
  6. Cry.

  </details>

<br>

<hr>

</details>
