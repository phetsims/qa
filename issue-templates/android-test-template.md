# Android App QA Test

## Links and dates

- Sim release for testing the online update system: {{ App Developer provides this info }}
- Sim release for testing the offline update system: {{ App Developer provides this info }}
- App Previous Version: {{ App Developer provides this info }}
- App Test Version: {{ App Developer provides this info }}
- Play Store: https://play.google.com/store/apps/details?id=edu.colorado.phet.androidApp
- Internal Test Page: https://play.google.com/apps/internaltest/4697762600441754675/

## OS versions to test

For Android, test the earliest and latest versions of the OS that are in the QA arsenal, and make a note of the version you test if it is different from the one mentioned.

- [ ] Latest Android, Version 12 (Time = ) (Actual Version tested = )
- [ ] Earliest Android, 5.0 Lollipop (Time = ) (Actual Version tested = )
- [ ] Chrome OS, Latest (Time = )

## Form Factors to test

Only necessary if the test includes user interface features.

- [ ] Android Phone or Tablet, landscape and portrait (Time = )
- [ ] Chromebook, touchscreen (Time = )
- [ ] Chromebook, no touchscreen (Time = )

## Specific Test Cases

{{ The App Developer provides details on what has changed and needs testing. }}


## Simulation Update Test Cases

These should be tested for every update.


<details>
<summary>
<h3>New releases are fetched.</h3>
</summary>

1. Follow the steps for <a href="#testing-an-initial-play-store-installation">Testing an initial Play Store installation</a>
2. Open the app, making sure that internet access is enabled on the device.
3. Within 2 hours, the app should have the *Sim release for testing the online update system* in <a href="#links-and-dates">Links and dates</a>.
</details>


<details>
<summary>
<h3>New translations in the app locale are fetched.</h3>
</summary>

1. Switch the device to a non-English locale - preferably a language that uses upper/lower case
2. Follow the steps for <a href="#testing-an-initial-play-store-installation">Testing an initial Play Store installation</a>
3. Open the app, making sure that internet access is enabled on the device.
4. Identify a word that can change from upper to lower case and publish a translation with rosetta.
5. Wait 24 hours at least.
6. The app should now have the case change from step 4. Reverse step 4 and publish the translation.
</details>


<details>
<summary>
<h3>New translations in unused locales are NOT fetched.</h3>
</summary>

1. Switch the device to the English locale.
2. Follow the steps for <a href="#testing-an-initial-play-store-installation">Testing an initial Play Store installation</a>.
3. Open the app, making sure that internet access is enabled on the device.
4. Identify a word that can change from upper to lower case and publish a translation with rosetta.
5. Wait 24 hours at least, DO NOT open the app during this period.
6. Put the device in airplane mode.
7. Switch the device to the locale for the translation from step 4.
8. Open the app, it should NOT have the translation change present. Revert the step 4 translation and publish the translation.
</details>


<details>
<summary>
<h3>A Play Store update triggers simulation updates in offline contexts</h3>
</summary>

One use case for our app is offline use.  The typical story here is a rural school with no internet access in the class room.  An IT support person regularly takes a teacher's classroom devices somewhere there is internet and runs play store updates, without running the PhET App itself.  In this situation the app is only opened in the absence of an internet connection, so the online sim update system never has a chance to work.  Thus, when a Play Store update happens, the app should use the sims packaged with the app.
  
Testing this use case is very similar to testing a play store update (see above), except whenever the app is open the device should be in airplane mode.

1. Uninstall the PhET Android App.
2. Visit https://play.google.com/apps/internaltest/4697762600441754675/ and switch to the google account you use on the Play Store. If there is a button called "Leave Program" then click it.
3. <a href="#clear-the-play-store-cache">Clear the Play Store cache</a>.
4. Verify the [Play Store](https://play.google.com/store/apps/details?id=edu.colorado.phet.androidApp) is offering the <a href="#links-and-dates">previous version</a> of the app install it.
5. Put the device in airplane mode.
6. Open the app (important!).
7. Force stop the app.
8. Take the device out of airplane mode.
9. Visit https://play.google.com/apps/internaltest/4697762600441754675/ and switch to the google account you use on the Play Store. Click Accept Invite.
10. Clear the Play Store cache.
11. Verify that the [Play Store](https://play.google.com/store/apps/details?id=edu.colorado.phet.androidApp) is offering an *upgrade* (not installation) to the <a href="#links-and-dates">test version</a> and click Upgrade.
12. Put the device in airplane mode.
13. Open the app again, it should have the *Sim release for testing the offline update system* in <a href="#links-and-dates">Links and dates</a>.
</details>


## Common Procedures


<details>
<summary>
<h3>Clear the Play Store cache</h3>
</summary>

This should allow you to instantly switch to your selected track for your Play Store user.

1. On your Android device go to Settings > Apps > Google Play Store. (Shortcut: long tap on the play store and click App Info)
2. Click Force Stop.
3. Click Storage and click Clear Cache (no need to click Clear Data)
4. Open https://play.google.com/store/apps/details?id=edu.colorado.phet.androidApp in the Play Store on your device.
</details>



<details>
<summary>
<h3>Testing an initial Play Store installation</h3>
</summary>

1. Uninstall the PhET Android App.
2. Visit https://play.google.com/apps/internaltest/4697762600441754675/ and switch to the Google account you use on the Play Store. If there is a button called "Accept Invite" then click it.
3. <a href="#clear-the-play-store-cache">Clear the Play Store cache</a>.
4. Visit the [Play Store](https://play.google.com/store/apps/details?id=edu.colorado.phet.androidApp) and verify that it is offering the <a href="#links-and-dates">test version</a>, then click Install.
</details>


<details>
<summary>
<h3>Testing a Play Store Update</h3>
</summary>

1. Uninstall the PhET Android App.
2. Visit https://play.google.com/apps/internaltest/4697762600441754675/ and switch to the google account you use on the Play Store. If there is a button called "Leave Program" then click it.
3. <a href="#clear-the-play-store-cache">Clear the Play Store cache</a>.
4. Verify the [Play Store](https://play.google.com/store/apps/details?id=edu.colorado.phet.androidApp) is offering the <a href="#links-and-dates">previous version</a> of the app install it.
5. Open the app (important!).
6. Visit https://play.google.com/apps/internaltest/4697762600441754675/ and switch to the google account you use on the Play Store. Click Accept Invite.
7. <a href="#clear-the-play-store-cache">Clear the Play Store cache</a>.
8. Verify that the [Play Store](https://play.google.com/store/apps/details?id=edu.colorado.phet.androidApp) is offering an upgrade to the <a href="#links-and-dates">test version</a> and click Upgrade.
9. Open the app again and conduct upgrade specific testing.
</details> 
