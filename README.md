BloodBridge AI
An AI-assisted emergency blood donor matching and coordination prototype.

BloodBridge AI demonstrates how a structured blood request can be matched with potentially suitable nearby donor profiles, ranked transparently, and tracked in one simple web interface.
Prototype notice: This repository contains a frontend demonstration using sample data. It is not connected to real donors, hospitals, blood banks, GPS services, SMS, email, or push notifications. Match scores are illustrative ranking signals—not medical compatibility or donor eligibility decisions. Real donations and transfusions must be assessed and coordinated by qualified, authorized blood-bank professionals.

Why BloodBridge?
During an urgent search for blood, families may have to contact people individually and forward messages across multiple groups. BloodBridge explores a more organized workflow:
1. Create a structured blood request.
2. Filter sample donor profiles by blood group and search radius.
3. Rank potential profiles using an explainable score.
4. Review donor availability and profile-verification indicators.
5. Track the request in a single dashboard.
Features in this prototype
- Dashboard with sample network metrics and recent requests.
- Emergency blood request form.
- Donor matching simulation with blood-group and distance filters.
- Explainable ranking using blood-group filter, proximity, availability, and profile verification.
- Donor registration form (session-only sample profile).
- Request tracking and illustrative impact analytics.
- Responsive layout for desktop and mobile screens.
Run locally
No installation or build step is required.
1. Download or clone this repository.
2. Open index.html in a modern browser.
For a local development server, run
Deploy with GitHub Pages
1. Create a public GitHub repository named bloodbridge-ai (or another name you prefer).
2. Upload the files in this repository, keeping index.html at the repository root.
3. Open Settings → Pages in the GitHub repository.
4. Under Build and deployment, choose Deploy from a branch.
5. Select the main branch and / (root), then save.
6. Wait for GitHub Pages to publish the site. The published URL will appear in the Pages settings.
Project structure
bloodbridge-ai/
├── index.html                  # Complete self-contained web prototype
├── README.md                   # Project overview and setup instructions
├── LICENSE                     # MIT license
├── .gitignore                  # Common local/editor exclusions
└── docs/
    ├── PROJECT_OVERVIEW.md     # Problem, users, goals, and scope
    ├── ARCHITECTURE.md         # Current prototype and future architecture
    └── DEMO_SCRIPT.md          # Short judge demonstration walkthrough
Matching logic (prototype)
The demo uses a transparent weighted score:
Score = 0.40 × Blood-group filter
      + 0.25 × Location proximity
      + 0.20 × Availability
      + 0.15 × Profile verification
This is a demonstration ranking formula only. The blood-group component is a prototype filter, not a clinical compatibility determination. The prototype uses a small hard-coded sample donor list and approximate distances; it does not calculate live routes or real locations.
Suggested next steps
- Replace sample data with a secure API and PostgreSQL database.
- Add consent-based donor accounts and secure authentication.
- Integrate verified hospital/blood-bank request review.
- Use a geospatial database such as PostGIS for real distance queries.
- Add opt-in notifications and audit logging.
- Conduct privacy, security, clinical, and regulatory review before any real-world pilot.
See the docs/ folder for the project scope, architecture, and demo script.
Team / competition use
BloodBridge AI is presented as a prototype concept for improving emergency donor discovery and coordination. Update this section with your team name, member names, institution, and competition details before submission.
License
This project is released under the MIT License. See LICENSE.
