SEMS eLibrary
Overview
SEMS eLibrary is a web-based platform designed for the National Association of Earth and Mineral Sciences Students (NAEMSS) to provide seamless access to academic resources in fields such as Metrology, Climate Science, and Applied Geology. Built by Gabriel for NAEMMSITES, this project aims to empower students, researchers, and faculty with a user-friendly, secure, and responsive digital library. The platform features a consistent UI theme, secure authentication, and a responsive design optimized for all devices.
Live Demo: NAEMSS Eibrary (https://naemsselibrary.github.io/NaemssELibrary/)
Date: July 29, 2025
Features

Responsive Design: Fully responsive across mobile, tablet, and desktop devices, with a max-w-7xl container for consistent layout.
Consistent UI Theme:
Colors: Gold (#FFD700), Dark Gold (#B8860B), Soft Blue (#60A5FA), Light Blue (#93C5FD), Pale Green (#A7F3D0), Deep Slate (#1E293B).
Typography: Poppins font (weights 300, 400, 600, 700).
Card Styling: Department card aesthetic with gold/dark gold top borders, hover scale (1.05), and shadow effects.


Pages:
Home (/index.html): Introduces SEMS eLibrary with a hero slideshow and links to departments.
Metrology & Climate Science (/mcs.html): Showcases resources for Metrology and Climate Science.
Applied Geology (/agy.html): Highlights resources for Applied Geology.
Signup (/signup.html): Allows new users to register with email, password, name, and matric number (AGY, AGP, MST, MCS, RSG validation).
Login (/login.html): Provides secure login with email or matric number and password.
Dashboard (/dashboard.html): User hub with profile details (name, matric number, email), navigation tabs, recent resources, and logout functionality.
About (/about.html): Details the mission, history, team, and features of SEMS eLibrary.
Contact (/contact.html): Includes a contact form with validation and contact information (email, phone, address, office hours).


Authentication: Firebase Authentication for secure signup, login, and dynamic navbar links (Dashboard for logged-in users, Signup/Login for others).
Slideshows: Auto-rotating hero slideshows on Home, Dashboard, About, and Contact pages, pausing on hover.
Forms:
Signup/Login: Client-side validation for email, password, and matric number.
Contact: Validates name, email, and message fields.
Newsletter: Email subscription with regex validation (placeholder).


Footer: Consistent across all pages with newsletter subscription, quick links, contact info, social media, and credit line: © 2025 SEMS eLibrary. Proudly built by Gabriel for NAEMMSITES.

Project Structure
sems-elibrary/
├── index.html                 # Home page
├── mcs.html                   # Metrology & Climate Science page
├── agy.html                   # Applied Geology page
├── signup.html                # Signup page
├── login.html                 # Login page
├── dashboard.html             # User dashboard
├── about.html                 # About page
├── contact.html               # Contact page
├── README.md                  # Project documentation
└── assets/                    # Static assets (images, etc.)
    ├── images/                # Placeholder images for slideshows
    └── css/                   # Optional custom CSS (if not using Tailwind CDN)

Technologies

Frontend:
HTML5, CSS3, JavaScript (ES6+)
Tailwind CSS (CDN) for responsive styling
Poppins font (Google Fonts) for typography
Font Awesome (CDN) for icons (navbar hamburger, footer social media)


Key Features by Page
Home (index.html)

Hero slideshow (Library Resources, Academic Excellence, Research Innovation).
Links to Metrology & Climate Science and Applied Geology.
Navbar with conditional Dashboard/Signup/Login links.
Footer with newsletter, quick links, contact, and social media.

Metrology & Climate Science (mcs.html)

Department-specific resources in card layout (gold/dark gold borders, hover scale).
Hero slideshow and consistent navbar/footer.

Applied Geology (agy.html)

Geology resources in card layout, matching MCS page styling.
Hero slideshow and consistent navbar/footer.

Signup (signup.html)

Form with email, password, first name, last name, and matric number (AGY, AGP, MST, MCS, RSG validation).
Firebase Authentication for user creation.
Responsive card with gold/dark gold border.

Login (login.html)

Form for email/matric number and password login.
Firebase Authentication with error handling.
Responsive card with gold/dark gold border.

Dashboard (dashboard.html)

User profile (name, matric number, email; matric number requires Firestore).
Navigation tabs to all pages (Home active by default).
Recent resources grid (placeholder; needs Firestore).
Logout button with Firebase signOut.
Hero slideshow and consistent navbar/footer.

About (about.html)

Sections for mission, history, team (3 members), and features (4 cards).
Hero slideshow (Library Resources, Academic Excellence, Research Innovation).
Conditional navbar links via Firebase Authentication.

Contact (contact.html)

Contact form with client-side validation (name, email, message).
Contact info grid (email, phone, address, office hours).
Hero slideshow (Get In Touch, Support Team, Connect With Us).
Conditional navbar links via Firebase Authentication.

Recent Resources: Placeholder on Dashboard; implement Firestore collection (e.g., users/{uid}/recentResources) for dynamic data.
Slideshows: Use placeholder images (1200x400); replace with relevant visuals in production.
Authentication: Uses Firebase Compat SDK (v10.14.1). Upgrade to modular SDK (v10+) for better performance in production.
Accessibility: Ensure ARIA labels for icons and form fields in future updates.
SEO: Add meta tags (description, keywords) to all pages for better search visibility.

Future Enhancements

Backend Integration: Use Firebase Functions for contact form submissions and newsletter subscriptions.
Firestore Integration: Store matric numbers, user profiles, and recent resources.
Search Functionality: Add a search bar for resources across departments.
User Profile Editing: Implement profile update form on Dashboard.
Analytics: Integrate Firebase Analytics for user behavior tracking.
Custom Images: Replace placeholder slideshow images with NAEMSS-specific visuals.
Dark Mode Toggle: Add a manual dark mode switch (currently class-based).


License
© 2025 SEMS eLibrary. Proudly built by Gabriel for NAEMMSITES. All rights reserved.
Contact
For questions or feedback, reach out to:

Email: naemsselibrary@gamil.com
Phone: +2349132091205
Address: NAEMSS Secretariat, Federal University of Technology, Akure, Nigeria
