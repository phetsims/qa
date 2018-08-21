<!---

~~~~~~~~~~~~~
~~ QA Book ~~
~~~~~~~~~~~~~

-->

<h1>QA Book</h1>

This is the QA Book. (QA stands for quality assurance.) If you're reading this, you're probably our new QA tester. If so, welcome! If you're not a PhET employee, 1) thank you for reading this, 2) please let us know how you managed to find this obscure corner of GitHub, and 3) feel free to read on and learn how we test our simulations. Just about everything you need to know to test PhET simulations is in this book.

[Insert cover comic here.]

Thanks to Cornel Stefanache and Constantin Orasanu of MonkeyUser.com for their [humorous comic](https://www.monkeyuser.com/2018/the-struggle/) that Megan "PhETified."

<hr>

<h2>Contents</h2>

**[Section 1: Hardware & Software](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#section-1-hardware--software)**
  - [1.1: Devices](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#11-devices)
  - [1.2: Operating Systems](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#12-operating-systems)
  - [1.3: Web Browsers](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#13-web-browsers)
  - [1.4: Updates](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#14-updates)

**[Section 2: Communication & Coordinization](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#section-2-communication--coordinization)**
  - [2.1: Email](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#21-email)
  - [2.2: Google Groups](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#22-google-groups)
  - [2.3: Google Calendar](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#23-google-calendar)
  - [2.4: Google Drive](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#24-google-drive)
  - [2.5: Slack](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#25-slack)
  - [2.6: Zoom](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#26-zoom)

**[Section 3: GitHub](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#section-3-github)**
  - [3.1: Repositories](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#31-repositories)
  - [3.2: Issues](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#32-issues)
  - [3.3: Terminology](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#33-terminology)

**[Section 4: Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#section-4-testing)**
  - [4.1: Development (Dev) Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#41-development-dev-testing)
  - [4.2: Release Candidate (RC) Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#42-release-candidate-rc-testing)
  - [4.3: PhET-iO Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#43-phet-io-testing)
  - [4.4: Accessibility (a11y) Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#44-accessibility-a11y-testing)
  - [4.5: Online Website Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#45-online-website-testing)
  - [4.6: Offline Website (Installer) Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#46-offline-website-installer-testing)
  - [4.7: Automated (Continuous) Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#47-automated-continuous-testing)
  - [4.8: Memory Leak Testing](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#48-memory-leak-testing)

**[Section 5: Translations](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#section-5-translations)**
  - [5.1: Legacy Simulation Translations](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#51-legacy-simulation-translations)
  - [5.2: HTML5 Simulation Translations](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#52-html5-simulation-translations)
  - [5.3: Website Translations](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#53-website-translations)

**[Section 6: Maintenance & Management](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#section-6-maintenance--management)**
  - [6.1: Testing Matrix Management](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#61-testing-matrix-management)
  - [6.2: PhET Test Maintenance](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#62-phet-test-maintenance)
  - [6.3: Website Administration](https://github.com/phetsims/QA/blob/master/doc/qa-book.md#63-website-administration)
  - [6.4: QA Book Maintenance](link)

<hr>

<!---
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\ Section 1: Hardware & Software
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
-->

<h2>Section 1: Hardware & Software</h2>
<h3>1.1: Devices</h3>
<h3>1.2: Operating Systems</h3>
<h3>1.3: Web Browsers</h3>
<h3>1.4: Updates</h3>

<hr>

<!---
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\ Section 2: Communication & Coordinization
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
-->

<h2>Section 2: Communication & Coordinization</h2>

<h3>2.1: Email</h3>
<h3>2.2: Google Groups</h3>
<h3>2.3: Google Calendar</h3>
<h3>2.4: Google Drive</h3>
<h3>2.5: Slack</h3>
<h3>2.6: Zoom</h3>

<hr>

<!---
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\ Section 3: GitHub
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
-->

<h2>Section 3: GitHub</h2>

<h3>3.1: Repositories</h3>
<h3>3.2: Issues</h3>
<h3>3.3: Terminology</h3>

<hr>

<!---
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\ Section 4: Testing
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
-->

<h2>Section 4: Testing</h2>

<h3>4.1: Development (Dev) Testing</h3>
<h3>4.2: Release Candidate (RC) Testing</h3> <!--- Add screenshots. -->
<h3>4.3: PhET-iO Testing</h3>
<h3>4.4: Accessibility (a11y) Testing</h3>
<h3>4.5: Online Website Testing</h3>
<h3>4.6: Offline Website (Installer) Testing</h3>
<h3>4.7: Automated (Continuous) Testing</h3>
<h3>4.8: Memory Leak Testing</h3>

<hr>

<!---
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\ Section 5: Translations
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
-->

<h2>Section 5: Translations</h2>

<h3>5.1: Legacy Simulation Translations</h3>
<h3>5.2: HTML5 Simulation Translations</h3>
<h3>5.3: Website Translations</h3>

<hr>

<!---
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\ Section 6: Maintenance & Management
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
-->

<h2>Section 6: Maintenance & Management</h2>

<h3>6.1: Testing Matrix Management</h3>
<h3>6.2: PhET Test Maintenance</h3>
<h3>6.3: Website Administration</h3>
<h3>6.4: QA Book Maintenance</h3>

<hr>
