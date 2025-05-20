Cat Info Viewer
This project provides a simple web interface to view and analyze data about cat breeds, fetched from TheCatAPI. Users can filter cats by health issues, display weights in imperial or metric units, view intelligence and child-friendliness ratings, and calculate average intelligence.

Features
Display All Cat Names: Shows a list of all cat breed names.
Filter by Health Issue: Filters and displays cat names based on a specified health issue numerical rating.
Show Weights: Toggles between imperial and metric weight units for all cat breeds.
Show Intelligence & Child-Friendliness: Displays the intelligence and child-friendliness ratings for each cat.
Average Intelligence: Calculates and displays the average intelligence across all cat breeds.
Average Intelligence for Child-Friendly Cats: Calculates the average intelligence for cats that meet a specified child-friendly rating threshold.
How to Use
Save the Code: Save the provided HTML code as an .html file (e.g., index.html).
Open in Browser: Open the index.html file in your web browser.
Interact: Use the buttons and input fields to explore the cat data.
Code Description
The HTML file includes a basic structure with buttons and input fields that trigger JavaScript functions. The JavaScript code fetches cat data from TheCatAPI and dynamically updates the <pre id="output"> element with the results.

HTML Structure
Buttons to trigger various data display and filtering functions.
Input fields for specifying health issues and child-friendly thresholds.
Radio buttons for selecting weight units (imperial/metric).
A <pre> tag with id="output" where all results are displayed.
JavaScript Functions
cats = []: An array to store the fetched cat data.
Workspace("https://api.thecatapi.com/v1/breeds"): Fetches cat breed data from TheCatAPI.
showAllNames(): Maps through the cats array and displays all cat names.
filterByHealthIssue(): Filters cats based on the health_issues property and displays matching names.
showWeights(): Iterates through cats and displays their weight based on the selected unit (imperial or metric).
showIntelligence(): Displays the intelligence and child_friendly ratings for each cat.
showAverageIntelligence(): Calculates the average of the intelligence property for all cats.
averageChildFriendlyIntelligence(): Filters cats based on a child_friendly threshold and then calculates the average intelligence of the filtered cats.
Sources
Cat Data API: TheCatAPI - https://api.thecatapi.com/v1/breeds
Programming Language: JavaScript
Markup Language: HTML
Styling: Inline CSS for basic layout.
