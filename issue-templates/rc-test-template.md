(*@ mention the appropriate parties, including designers*), {{SIM_TITLE}} 1.X.X-rc.X is ready for RC testing.

**[Link to sim](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/1.0.0-rc.1/{{REPO}}_en.html)**

**[Link to iFrame](http://www.colorado.edu/physics/phet/dev/html/{{REPO}}/1.0.0-rc.1/{{REPO}}_en-iframe.html)**

**[Test Matrix]({{TEST_MATRIX_LINK}})**

**Issues to Verify**
(*all should be marked "status:fixed-pending-testing"*)  
Please test the following issues and check them off after addressing. If they are resolved, close them.  If not, they should be updated.

- [ ] https://github.com/phetsims/{{REPO}}/issues/##
- [ ] https://github.com/phetsims/{{REPO}}/issues/##

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

If any new issues are found, please note them in https://github.com/phetsims/{{REPO}}/issues and reference this issue.  

 
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
