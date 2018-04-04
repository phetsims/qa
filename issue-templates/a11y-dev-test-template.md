(*@ mention the appropriate parties, including designers*), {{SIM_TITLE}} 1.X.X-dev.X is ready for dev testing.

Before beginning, familiarize yourself with how a screen reader works. Here is a page with information about PhET's supported screen readers and documentation about how to use them:
[Screen reader intro](https://www.colorado.edu/physics/phet/dev/html/jg-tests/reader-intro.html)

**[Link to sim](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/{{VERSION}}/{{REPO}}_en.html)**

The above sim has labels and/or descriptions. They can be "seen" here:
**[Link to a11y view](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/{{VERSION}}/{{REPO}}_a11y_view_html.html)**

This view should assist in seeing what is available to a screen reader user. While testing,  please make sure that all descriptions and alerts accurately describe the state of the simulation. All content in the a11y-view should be readable with a screen reader when one is active.

PhET supports the following platforms for accessibility so please test these:
- [ ] JAWS with latest Windows, latest Firefox
- [ ] NVDA with latest Windows, latest Firefox
- [ ] VoiceOver with latest macOS, latest Safari

If any new issues are found, please note them in https://github.com/phetsims/{{REPO}}/issues and reference this issue. 

**Critical screen reader information**
 - JAWS might complain about Firefox Quantum. If that is the case, please test with https://www.mozilla.org/en-US/firefox/organizations/
 - The screen reader must be turned on and reading before the browser is open for it to work. See https://github.com/phetsims/a11y-research/issues/90
 - JAWS might not automatically switch to forms mode for some controls (like sliders and radio buttons). In this case, pressing "enter" should switch to forms mode. For example, see https://github.com/phetsims/resistance-in-a-wire/issues/138
 - The screen reader might focus the last UI component that had focus on sim load, typically on refresh. This is a "feature". For example, see For example, see phetsims/resistance-in-a-wire#139
 
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