(*@ mention the appropriate parties, including designers*), {{SIM_TITLE}} 1.X.X-dev.X is ready for dev testing.

Before beginning, familiarize yourself with how a screen reader works. Here is a page with information about PhET's supported screen readers and documentation about how to use them:
[Screen reader intro](https://www.colorado.edu/physics/phet/dev/html/jg-tests/reader-intro.html)

**[Link to sim](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/{{VERSION}}/{{REPO}}_en.html)**

The above sim has labels and/or descriptions. They can be "seen" here:
**[Link to a11y view](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/{{VERSION}}/{{REPO}}_a11y_view_html.html)**

This view should assist in seeing what is available to a screen reader user. While testing,  please make sure that all descriptions and alerts accurately describe the state of the simulation. All content in the a11y-view should be readable with a screen reader when one is active.

PhET supports the following platforms for accessibility so please test these:
- [ ] JAWS with latest Windows, latest Chrome
- [ ] NVDA with latest Windows, latest Firefox
- [ ] VoiceOver with latest macOS, latest Safari

If any new issues are found, please note them in https://github.com/phetsims/{{REPO}}/issues and reference this issue. 

**Critical screen reader information**
  We are tracking known AT bugs in https://docs.google.com/document/d/1518zv6F0odExFsodShZxwTmWNQk3civuNwtQUR-rEBs/. If
  you notice a new bug with AT behavior, please check against this list first.
 
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