<!---
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

DEVELOPERS: 

* title for this issue = MR Test: {Brief Description}
* replace {{MENTIONS}} with @mentions for team members who should receive GitHub notifications about this issue
* Delete things that are not relevant, e.g. PhET-iO links for non-PhET-iO tests.
* QA kickoff meeting may be appropriate.
* assign the issue to @KatieWoe and @kathy-phet

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-->

<h1>Maintance Release</h1>

**Mentions**: {{MENTIONS}}

**Focus and Instructions**
<!---
Things to include here:
A description of the test being done. Include the issue that was fixed. Range of platforms to test on, 
and potential related issues to check. Include where and how to report issues found (slack, specific repo, etc.)
Include circumstances in which to halt testing. Include important deadlines.
--->

**Issues to Confirm**
<!---
A checklist of links to the issues involved.
--->
- [ ] {Issue one}
- [ ] {Issue two}

**Instructions and Steps**
<!---
Bullet Points with the steps for specific tests and requested coverage
--->
* Click on the Sim RC Link Below and Verify that the Sim Launches
* {Step two}
* {ETC.}

<!---
Example Instructions:
- IF HYDROGEN AND HAS A PREVIOUS MINOR VERSION THAT SUPPORTS MIGRATION: Load the Migration wrapper and test against the previous published minor version (SEE VERSION CHECKLIST BELOW)
- In the old (top) version, open the About dialog, then click Migrate Now.
- Change a string value, click Migrate Now.
- Hide an element, then click Migrate Now.
- Load the Migration wrapper and test against the previous published maintenance version: https://phet-io.colorado.edu/sims/concentration/1.8.0-rc.1/wrappers/migration/?oldVersion=1.8 (modify this url for the sim version being tested)
- In the old (top) version, open the About dialog, then click Migrate Now.
- Change a string value, click Migrate Now.
- Hide an element, then click Migrate Now.
--->

**Links**
<!---
Links to the built simulations to test. Checklist.
If seperate testing processes are required, please split lists appropriately. 
--->
- [ ] {Sim One}
- [ ] {Sim Two}
- [ ] {ETC.}
