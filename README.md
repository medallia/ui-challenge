# UI Challenge @ Medallia

The screenshot shows an interface for selecting and downloading reports. Each report has an associated ID, name, type and size (in bytes).

![](screenshot.png?raw=true)

## Instructions

Implement the features below using the included assets. Most of the HTML and CSS assets required have been included for you. You may use whichever open source libraries you feel comfortable with, including jQuery, Backbone and Angular. For this exercise, you will only need to support modern browsers.

The challenge should take on average 2-3 hours. Please record the length of time taken, and submit it to your recruiting contact alongside a zip file containing your solution.

## Features

**Dynamic Rendering**

The data to use for this challenge is included in the reports.json data file. Use the array of reports to render each report to the page, and display the size for each according to the following rules:

* Round the figure to no more than two decimal places
* Do not show trailing zeros if there is a decimal
* Select the appropriate unit of measurement (ie. display 1.2MB instead of 1,228.8Kb)

**Selection Behavior**

When a report is selected, the border should become thicker and turn blue. You can select a report by clicking on it, or add reports to the current selection by holding CTRL/CMD while clicking. You can also remove a report from the current selection by CTRL/CMD clicking on it when it is selected. Clicking on anything other than the reports or the command buttons will deselect all reports.

**Download Icon**

Each report has a download icon. For the purpose of this challenge, simply window.alert the ID of the report being downloaded when the icon is clicked.

**Selection Commands**

"Select All" and "Select None" should perform the appropriate action, and should be disabled when they become irrelevant. In the screenshot, "Select None" has been disabled to show the visual style. In addition, pressing CTRL/CMD+A should select all, and CTRL/CMD+D should deselect all.

**Download Command**

The "Download" command is enabled when any number of reports are selected, and disabled if no reports are selected. When clicked, window.alert a list containing the IDs of the currently selected reports.

**Total Size Summary**

The "Total Size" text is not visible when no reports are selected. If one or more reports are selected, this should display the total size of the selected reports according to the rules above in *Dynamic Rendering*.

