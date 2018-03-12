(*@ mention the appropriate parties, including designers*), {{SIM_TITLE}} 1.X.X-rc.X is ready for RC testing.

**[Link to sim](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/phet/1.X.X-rc.1/{{REPO}}_all_phet.html)**

**[Link to iFrame](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/phet/1.X.X-rc.1/{{REPO}}_all_iframe_phet.html)**

**[Test Matrix]({{TEST_MATRIX_LINK}})**

**Before beginning**, please familiarize yourself with how a screen reader works. Here is a page with information about PhET's supported screen readers and documentation about how to use them:
[Screen reader intro](https://www.colorado.edu/physics/phet/dev/html/jg-tests/reader-intro.html)

The simulation to test has labels and/or descriptions. They can be "seen" here:
**[Link to a11y view](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/phet/1.X.X-rc.1/{{REPO}}_a11y_view.html)**

This view shows what is available to a screen reader user. The sim is on the left side in an iframe, while the right side has all of the accessible descriptions. Beneath the sim are real-time alerts that will be announced by the screen reader. Please make sure that the descriptions on the right accurately describe the simulation at all times.

PhET supports the following platforms for accessibility so please test these:
*(These should be in the test matrix)*
- [ ] JAWS with latest Windows, latest Firefox
- [ ] NVDA with latest Windows, latest Firefox
- [ ] VoiceOver with latest macOS, latest Safari

**Please also verify**
- [ ] stringTest=double (all strings doubled)
- [ ] stringTest=long (exceptionally long strings)
- [ ] stringTest=X (short strings)
- [ ] stringTest=rtl (right-to-left)
- [ ] stringTest=xss (test passes if sim does not redirect, OK if sim crashes or fails to fully start)
- [ ] showPointerAreas (touchArea=red, mouseArea=blue)
- [ ] Full screen test
- [ ] Screenshot test
- [ ] Does AR need to be notified for any LOL updates?

Accessibility strings that are not visible should not be translatable yet, do not worry if these do not change with string tests.

If any new issues are found, please note them in https://github.com/phetsims/{{REPO}}/issues and reference this issue. 

**Critical screen reader information**
- JAWS might complain about Firefox Quantum. If that is the case, please test with https://www.mozilla.org/en-US/firefox/organizations/
- The screen reader **must** be turned on and reading before the browser is open for it to work. See https://github.com/phetsims/a11y-research/issues/90
- JAWS might not automatically switch to forms mode for some controls (like sliders and radio buttons). In this case, pressing "enter" should switch to forms mode.
 
**(Other potentially useful items)**  

Sim-specific query parameters useful for testing:  
(*examples from function builder*)  
• `?populateOutput` - puts 1 of each card in the output carousel  
• `?slow` - reduces animation speed to 25% of normal, useful for testing multitouch  

Sim-specific terminology:  
(*examples from function builder*)  
• builder - the apparatus in the center of the screen  
• slots - places where you can drop functions in the builder  
• input carousel - vertical carousel on the left  

@ariel-phet please assign and prioritize
