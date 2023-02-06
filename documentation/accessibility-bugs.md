# Known Accessibility Bugs

Please document all known AT bugs in this document.

**Contents**

* [1: Screen Readers](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#1-screen-readers)
    * [1.1: General Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#11-general-bugs)
    * [1.2: JAWS](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#12-jaws)
        * [1.2.1: Firefox Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#121-firefox-bugs)
        * [1.2.2: Chrome Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#122-chrome-bugs)
    * [1.3: NVDA](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#13-nvda)
        * [1.3.1: Firefox Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#131-firefox-bugs)
    * [1.4: VoiceOver](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#14-voiceover)
        * [1.4.1: Safari Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#141-safari-bugs)
        * [1.4.2: Mobile Safari Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#142-mobile-safari-bugs)
* [2: Keyboard Navigation](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#2-keyboard-navigation)
    * [2.1: General Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#21-general-bugs)
    * [2.2: Firefox Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#22-firefox-bugs)
    * [2.3: Safari Bugs](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#23-safari-bugs)
* [2: Voicing](https://github.com/phetsims/QA/blob/master/doc/accessibility-bugs.md#3-voicing)

## 1: Screen Readers

### 1.1: General Bugs

* The screen reader must be turned on and reading before the browser is open for it to work. See
  https://github.com/phetsims/a11y-research/issues/90.
* The screen reader might focus the last user interface component that had focus on sim load, typically on refresh. This
  is a "feature". For example, see https://github.com/phetsims/resistance-in-a-wire/issues/139.
* If the sim contains abbreviations (chemical formulas or other) the screen reader may try to read phonetically.
We decided to accept this. See https://github.com/phetsims/molarity/issues/215.

### 1.2: JAWS

#### 1.2.1: Firefox Bugs

* Be aware that JAWS may shift keyboard focus with Firefox Quantum. See
  https://github.com/phetsims/balloons-and-static-electricity/issues/404.
* If you use a slider by pressing and holding an arrow key, you will hear duplicate alerts that read the value when you
  release the arrow key. See https://github.com/phetsims/john-travoltage/issues/227.
* If you quickly move through slider values with arrow keys and reach the end of the range, JAWS won’t read the final
  value and it will be silent, see https://github.com/phetsims/john-travoltage/issues/246.
* When using a slider and holding down an arrow key, you might see the thumb move slowly while holding the key down,
  then move rapidly in one direction when you release a key, see https://github.com/phetsims/john-travoltage/issues/242.
* JAWS might not automatically switch to forms mode for some controls (like sliders and radio buttons). In this case,
  pressing "enter" should switch to forms mode. See https://github.com/phetsims/resistance-in-a-wire/issues/138.
* When using a slider, if value is at min/max and you press and hold an arrow key to try to move the value beyond the
  range, JAWS might crash. See https://github.com/phetsims/john-travoltage/issues/242.
* When reading about a slider with the virtual cursor, JAWS might read the min/max value with floating point rounding
  errors. For example “0.1” might sound like “0.1000...01”.
  See https://github.com/phetsims/resistance-in-a-wire/issues/177.
* If you click on the Windows taskbar (maybe other things too) pressing arrow keys will have no response from JAWS.
  Return to the browser and arrow keys should continue to work as expected.
* When focused on draggable objects, using the arrow keys will not move the object when JAWS is enabled because of
  https://github.com/phetsims/a11y-research/issues/9. WASD keys should still work.

#### 1.2.2: Chrome Bugs

* If you use a slider by pressing and holding an arrow key, you will hear duplicate alerts that read the value when you
  release the arrow key. See https://github.com/phetsims/john-travoltage/issues/227.
* When using a slider and holding down an arrow key, you might see the thumb move slowly while holding the key down,
  then move rapidly in one direction when you release a key, see https://github.com/phetsims/john-travoltage/issues/242.
* If there is a list in a dialog, when the dialog is first opened JAWS will read the list items as "bullet, bullet, ..."
  instead of reading the names of the items. See https://github.com/phetsims/a11y-research/issues/185.  

### 1.3: NVDA

So empty. Much goodness.

#### 1.3.1: Firefox Bugs

* When changing screens from the Home Screen, NVDA may read the page title several times and then the first line in the new screen before the first item in the new screen. See https://github.com/phetsims/ratio-and-proportion/issues/321
* When the values of sliders are read out sometimes NVDA will read out the wrong value.  Adjusting those sliders seems to fix the issue.  Likely an “AT caching” issue.  https://github.com/phetsims/resistance-in-a-wire/issues/202
* NVDA will read through the Sim Screen Overview when exiting a dialog
* NVDA may say name of WASD keys when pressed

### 1.4: VoiceOver

#### 1.4.1: Safari Bugs

* When closing a dialog with “escape” while the virtual cursor is on a list item, focus might not return to the Keyboard
  Help button in the navigation bar. See https://github.com/phetsims/ohms-law/issues/114.
* When using VoiceOver and the “Increment” feature on a slider (ctrl+option+spacebar), VoiceOver will sometimes read the
  previous aria-valuetext instead of the new one. See https://github.com/phetsims/a11y-research/issues/36.
* VoiceOver doesn’t interrupt alerts as aggressively as some other AT, so older alerts might queue and be read one after
  the other.
* In iOS 14, VoiceOver has a setting to describe images, which is on by default, and it is really bad at doing it for
  PhET Sims! To turn off this setting (as of 1/19/21), Settings -> Accessibility -> VoiceOver -> Verbosity -> Scene
  Descriptions -> switch off. See https://github.com/phetsims/ratio-and-proportion/issues/256 for more details.
* After a bit of use, VoiceOver may stop speaking alerts related to the slider value (aria-valuetext). Tabbing away
  from the component then returning to it will cause VoiceOver to speak its content again.
  See https://github.com/phetsims/sun/issues/508 and https://github.com/phetsims/ohms-law/issues/141
* When using a slider, "Home" and "End" keys will both change the value AND move the cursor to a different place in the
  document. See https://github.com/phetsims/a11y-research/issues/164.
* When using a combo box, Safari may say "Text" after reading each item in the combo box list. See https://github.com/phetsims/greenhouse-effect/issues/178.
* Safari will duplicate alerts when the sim is embedded in an iFrame. See https://github.com/phetsims/friction/issues/286

#### 1.4.2: Mobile Safari Bugs

* Sometimes when using VoiceOver, Safari buttons (like “reload” and “new tab” are not clickable by double tapping the
  screen. Restarting Safari fixes the problem.
  
* iOS VoiceOver may skip over dynamic content in the PDOM when reading with swipe gestures. See https://github.com/phetsims/a11y-research/issues/175

## 2: Keyboard Navigation

### 2.1: General Bugs

* When using a slider, if End/Home is pressed at the same time as Home/End, the browser will treat the keypress just
  like an arrow key and the value won’t be set to max/min. See
  https://github.com/phetsims/resistance-in-a-wire/issues/163.
* When moving sliders using the keyboard navigation, you can use shift and pg up and pg down to modify the speed of the
  sliders. However, shift can be pressed at any time during the slider’s motion to slow it. Conversely, the pg up and pg
  down keys can only be pressed at the start of the slider’s motion to affect it. This difference in behavior is normal.

### 2.2: Firefox Bugs

* To get keyboard navigation to work properly in Firefox: `System Preferences -> Keyboard -> Shortcuts -> All controls`.

### 2.3: Safari Bugs

* To get keyboard navigation to work properly in Safari:
  `Safari -> Preferences -> Advanced -> Press Tab to highlight each item on a webpage`.
  
## 3: Voicing

### 3.1 General Bugs
* For some of the non-default Voices, it takes some time to render the information and performance of the sim may be reduced.
At this time this is acceptable and there is nothing we can do to improve this. Acceptable performance is subjective, in general
please create an issue if there are any questions about performance.

### 3.2 ChromeOS Bugs
* Voicing and SpeechSynthesis can be slower to start on ChromeOS. Especially when switching tabs or turning it on 
for the first time. If Voicing doesn't start for ~8 seconds after you enable it or play with the sim that is expected.
If it takes longer to start or never starts that is probably an issue. See https://github.com/phetsims/number-play/issues/138

### 3.3 iOS Safari Bugs
* Changing voices on iOS Safari is broken. The control for selecting voices have been removed on this platform. See https://github.com/phetsims/utterance-queue/issues/74. 
