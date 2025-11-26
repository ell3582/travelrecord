Okinawa Trip 2026 Itinerary Planning App

This is a single-page interactive web application (SPA) developed using pure HTML, JavaScript, and Tailwind CSS, designed for collaborative trip itinerary planning.
Core Features

Real-time Collaboration: Itinerary data is stored in the Firestore database, allowing all users (within the same Canvas environment) to see updates instantly.

Responsive Design: The interface is optimized for mobile devices, making it convenient for viewing and updating during the trip.

Day Categorization: Users can easily switch between and view itineraries for different days.

Quick Navigation: Every itinerary item includes a direct Google Maps link for instant navigation.

Built-in Authentication: Authentication uses a custom token provided by the Canvas environment, ensuring data security.

How to Run
Because this App relies on specific Canvas environment variables (__app_id, __firebase_config, __initial_auth_token) for Firestore initialization and authentication, it cannot be run locally without modification.

If you want to preview the interface locally, you must replace the Firebase global variables in index.html with mocked data or run it on a platform that supports Firebase environment variable injection.

GitHub Pages Deployment Troubleshooting
If you deploy this file to GitHub Pages but the link only displays the raw source code (unrendered HTML), please follow these troubleshooting steps:

Check Deployment Source Settings (Settings > Pages):
In the Branch dropdown menu, ensure the Folder is set to / (root) (the repository's root directory).
File Location: Ensure your index.html file is directly located in the repository's root directory and not within any subfolders.

Confirm the Correct Access URL:
Incorrect Action: Do not click on the index.html file in the GitHub file list and then select View Raw; this will only show the code.

Correct Action: You must visit the green link displayed on the Settings > Pages page (i.e., the URL after "Your site is published at...").

Wait for Deployment Completion:
GitHub Pages typically requires 1 to 5 minutes to build and deploy after you save the settings or push new code. Visiting the link before the status updates to "Your site is live at..." may result in failure or display of old content.

Clear Browser Cache:
Try clearing your browser cache or using Incognito/Private Browsing mode to revisit the Pages link.

Project Files
index.html: Contains all the HTML, CSS, and JavaScript (including Firebase logic) in a single file.
