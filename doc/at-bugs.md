# Known AT Bugs

Please document all known AT bugs in this document.

**Contents**
* [1: Screen Readers](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#1-screen-readers)
  * [1.1: General Bugs](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#11-general-bugs)
  * [1.2: JAWS](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#12-jaws)
    * [1.2.1: Firefox Bugs](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#121-firefox-bugs)
  * [1.3: NVDA](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#13-nvda)
    * [1.3.1: Firefox Bugs](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#131-firefox-bugs)
  * [1.4: VoiceOver](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#14-voiceover)
    * [1.4.1: Safari Bugs](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#141-safari-bugs)
    * [1.4.2: Mobile Safari Bugs](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#142-mobile-safari-bugs)
* [2: Keyboard Navigation](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#2-keyboard-navigation)
  * [2.1: General Bugs](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#21-general-bugs)
  * [2.2: Firefox Bugs](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#22-firefox-bugs)
  * [2.3: Safari Bugs](https://github.com/phetsims/QA/blob/master/doc/at-bugs.md#23-safari-bugs)

## 1: Screen Readers

### 1.1: General Bugs

* The screen reader must be turned on and reading before the browser is open for it to work. See https://github.com/phetsims/a11y-research/issues/90.
* The screen reader might focus the last user interface component that had focus on sim load, typically on refresh. This is a "feature". For example, see https://github.com/phetsims/resistance-in-a-wire/issues/139.

### 1.2: JAWS

#### 1.2.1: Firefox Bugs

* Be aware that JAWS may shift keyboard focus with Firefox Quantum. See https://github.com/phetsims/balloons-and-static-electricity/issues/404.
* If you use a slider by pressing and holding an arrow key, you will hear duplicate alerts that read the value when you release the arrow key. See https://github.com/phetsims/john-travoltage/issues/227.
* If you quickly move through slider values with arrow keys and reach the end of the range, JAWS won’t read the final value and it will be silent, see https://github.com/phetsims/john-travoltage/issues/246.
* When using a slider and holding down an arrow key, you might see the thumb move slowly while holding the key down, then move rapidly in one direction when you release a key, see https://github.com/phetsims/john-travoltage/issues/242.
* JAWS might not automatically switch to forms mode for some controls (like sliders and radio buttons). In this case, pressing "enter" should switch to forms mode. See https://github.com/phetsims/resistance-in-a-wire/issues/138.
* When using a slider, if value is at min/max and you press and hold an arrow key to try to move the value beyond the range, JAWS might crash. See https://github.com/phetsims/john-travoltage/issues/242.
* When reading about a slider with the virtual cursor, JAWS might read the min/max value with floating point rounding errors. For example “0.1” might sound like “0.1000...01”. See https://github.com/phetsims/resistance-in-a-wire/issues/177.
* If you click on the Windows taskbar (maybe other things too) pressing arrow keys will have no response from JAWS. Return to the browser and arrow keys should continue to work as expected.
* When focused on draggable objects, using the arrow keys will not move the object when JAWS is enabled because of https://github.com/phetsims/a11y-research/issues/9. WASD keys should still work.

### 1.3: NVDA

So empty. Much goodness.

#### 1.3.1: Firefox Bugs

So empty. Much goodness.

### 1.4: VoiceOver

#### 1.4.1: Safari Bugs

* When closing a dialog with “escape” while the virtual cursor is on a list item, focus might not return to the Keyboard Help button in the navigation bar. See https://github.com/phetsims/ohms-law/issues/114.
* When using VoiceOver and the “Increment” feature on a slider (ctrl+option+spacebar), VoiceOver will sometimes read the previous aria-valuetext instead of the new one. See https://github.com/phetsims/a11y-research/issues/36.
* VoiceOver doesn’t interrupt alerts as aggressively as some other AT, so older alerts might queue and be read read one after the other.

#### 1.4.2: Mobile Safari Bugs

* Sometimes when using VoiceOver, Safari buttons (like “reload” and “new tab” are not clickable by double tapping the screen. Restarting Safari fixes the problem.

## 2: Keyboard Navigation

### 2.1: General Bugs

* When using a slider, if End/Home is pressed at the same time as Home/End, the browser will treat the keypress just like an arrow key and the value won’t be set to max/min. See https://github.com/phetsims/resistance-in-a-wire/issues/163.
* When moving sliders using the keyboard navigation, you can use shift and pg up and pg down to modify the speed of the sliders. However, shift can be pressed at any time during the slider’s motion to slow it. Conversely, the pg up and pg down keys can only be pressed at the start of the slider’s motion to affect it. This difference in behavior is normal.

### 2.2: Firefox Bugs

* To get keyboard navigation to work properly in Firefox: `System Preferences > Keyboard > Shortcuts > All controls`.

### 2.3: Safari Bugs

* To get keyboard navigation to work properly in Safari: `Safari > Preferences > Advanced > Press Tab to highlight each item on a webpage`.
