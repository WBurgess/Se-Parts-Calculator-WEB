Se-Parts-Calculator-WEB
=======================

The Single Page Application Web version of the previous parts calculator, built with HTML and JS using knockout.js.

Unlike the desktop application, this version is feature complete with working input fields and delete buttons.

TL;DR Summary:

  It uses 4 ko.observable Arrays linked by index to determine what parts have been "propped" by the user via buttons, which then determines which componentNames and componentValues to display. Each active part has its own multiplier changed via input fields. 
  
  Since parts share components, their displayed value is the sum of each part's default value * its multiplier. When the multiplier is reduced (ex: from 15 to 1), the default componentValues are multiplied by a negative multiplier which is then still added to the final sum. This effectively subtracts the correct amount per part from the total.
  
  All block names, component data, and images are pulled from: http://spaceengineers.wikia.com/wiki/Category:Blocks
  
Features TODO:

1) I plan on adding a second page to the site as a giant input form for mod-makers that allows them to input partNames, componentNames, and componentValues that will then be added to the JS object that acts as the "database" for the calculator

2) Adding a checkbox at the top that allows users to Select-All small checkboxes. Its a little tedious selecting all of them when building a small ship

3) Finish populating the JS object via JSON queries to the space engineers wikia
