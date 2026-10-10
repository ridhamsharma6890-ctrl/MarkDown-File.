# LaundryEase — AI Prompts and Tools Used

## Project overview
LaundryEase is a prototype smart hostel laundry management system. Students book laundry and track bags using a unique Bag ID and QR code. Laundry staff scan/find bags and update order status. Boys and Girls hostel administrators manage authorized student accounts and their own hostel orders.

**Repository:** https://github.com/ridhamsharma6890-ctrl/LaundryEase  
**Live website:** https://ridhamsharma6890-ctrl.github.io/LaundryEase/

## AI tools used

- **ChatGPT (OpenAI):** Assistance with brainstorming, requirements, sample HTML/CSS/JavaScript, Firebase integration guidance, debugging suggestions, interface styling, and presentation/documentation drafting.

> **Clarification:** ChatGPT was used to help *develop* the project. LaundryEase does not currently claim to contain an AI-powered model or automated AI decision-making feature.

## Development and deployment tools

| Tool | Purpose |
| --- | --- |
| Visual Studio Code | Editing HTML, CSS, and JavaScript |
| VS Code Live Server | Testing the frontend locally |
| HTML / CSS / JavaScript | Website structure, design, and interactivity |
| Firebase Authentication | Login accounts and role-based authentication |
| Cloud Firestore | Student profiles, staff/admin assignments, laundry orders, and statuses |
| Browser camera / QR scanning library | Reading bag QR codes on supported devices |
| GitHub | Version control and project repository |
| GitHub Pages | Hosting the public demo website |
| Chrome Developer Tools | Checking browser errors and troubleshooting |

## Example prompts given to ChatGPT

The following are **representative prompts from the development conversation**, with wording lightly cleaned up for readability; not a claim that this is a complete verbatim chat transcript.

1. **Problem definition:** "Help me build a hostel laundry management website that solves a real-world problem and can expand in the future."
2. **Bag identification:** "How can each student's laundry bag be identified so clothes do not get mixed up?"
3. **Hostel requirements:** "Boys and girls hostels have AC and Non-AC blocks and separate laundry collection points. How should the website manage these?"
4. **Student registration:** "Make it so only hostel admins can register students through the admin dashboard. Students should not self-register."
5. **Staff assignments:** "How many staff accounts should we create, and how can Boys staff handle Blocks A–D and Girls staff Blocks E–H?"
6. **Workflow:** "Simplify the laundry statuses to Booked, Collected, Ready for Collection and Completed."
7. **Firestore debugging:** "Staff orders are not loading and Firestore says permission-denied. Help me fix the query and security rules."
8. **QR scanning:** "How can laundry staff scan a bag's QR code and update the student's order?"
9. **Visual design:** "Make the interface look modern with a background photo of freshly folded laundry."
10. **Deployment:** "How do I upload LaundryEase to GitHub and make it live so hackathon judges can test it?"
11. **Presentation:** "Create a presentation of at most six slides covering the problem, solution, AI used and GitHub repository."

## How AI assistance was used responsibly

- Code suggestions were manually incorporated into the VS Code project and tested.
- Firebase roles and access rules were configured to separate Boys and Girls hostel data.
- Problems were debugged using visible Firebase/browser error messages.
- AI responses were treated as development suggestions, not as proof of security or production readiness.
- Demo accounts and fictional/test student information should be used for public judging.

## Project workflow

`Booked → Collected → Ready for Collection → Completed`

## Important deployment notes

- GitHub Pages hosts static frontend files; Firebase provides authentication and database services.
- Do not commit service-account private keys, real passwords or student personal data to the public repository.
- Admin-only Firestore student-profile creation can be protected with security rules, but fully preventing unauthorized Firebase Authentication sign-up requires a trusted provisioning backend.
- This project is a hackathon prototype and should undergo additional security and operational testing before a real-campus rollout.

## Credits

Concept, integration, testing and presentation: LaundryEase hackathon project team. AI assistance: ChatGPT (OpenAI).
