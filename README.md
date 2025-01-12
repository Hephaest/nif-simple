# GcoTimer

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 14.0.0.

For the analysis of odors emitted from a Gas Chromatograph - [Gas Chromatography-Olfactometry](https://en.wikipedia.org/wiki/Gas_chromatography-olfactometry).

Most of the action is around the large green button in the middle of the app.  It has 3 states:
1. Inject
2. Start
3. Stop

On initial running of the app (or after the Reset button is pressed) the button state is, "Inject".
At the time the sample is injected into the GC-O, this button should be pressed. The button state changes to "Start" and the Date/Time of the injection is displayed beneath the button.

When an odor is detected by the user, then Start is pressed.  This logs the time from injection that the odor starts to appear.  The button state changes to "Stop".
When the odor can no longer be detected by the user, then "Stop" is pressed.  This records the end time of odor detection.  The button state returns to "Start".

Optionally (if 'simple' flag is unset), after "Stop" has been pressed, the user is presented with a list of odor descriptors to choose from. After this selection is made, the user is presented with a further dialog-box to select the strength of the odor.

The data of the event is logged in the table below the button.  Odor Descriptor, Intensity, Start Time (minutes), End Time (minutes) and Duration (minutes) are recorded.

Each time a new odor is detected the Start/Stop sequence above is actioned.

At the end of the session, when all odors have been detected, the data can be exported as CSV, XLSX, or PDF. Click on the appropriate icon at the top of the table.
The filename of the data export is made up of the date/time of injection for uniqueness and as a record of the date/time.

Use in measuring NIF (Nasal Impact Frequency) and SNIF (Surface of Nasal Impact Frequency). See "Hyphenated Headspace-Gas Chromatography-Sniffing Technique:  Screening of Impact Odorants and Quantitative Aromagram Comparisons", Pollien p, et al, Journal of Agricultural and Food Chemistry 1997 45 (7), 2630-2637, DOI: [10.1021/jf960885r](https://sci-hub.st/10.1021/jf960885r)

The project was initiated to help [Aidan F Kirkwood](https://www.researchgate.net/profile/Aidan-Kirkwood-2) at Nottingham University with his PhD research.