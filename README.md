# Expense Tracker

A mobile-responsive expense tracker built with plain HTML/CSS/JS, Firebase Authentication (Google Sign-In), and Firebase Firestore.

## Important

This project requires your own Firebase project configuration. Open `js/firebase.js` and replace the placeholder values in `firebaseConfig` with the configuration from your Firebase Web app.

### Features
- Google Sign-In
- Private per-user Firestore data
- Income and expense tracking
- Dashboard totals and charts
- Transaction search, filtering, sorting, editing and deletion
- Profile and settings pages
- Responsive mobile-friendly UI

### Run locally
Use a static server (ES modules do not work correctly from `file://`):

```bash
python3 -m http.server 5000
```

Then open `http://localhost:5000`.

### Firebase setup
1. Create a Firebase project.
2. Enable Google Authentication.
3. Create a Firestore database.
4. Register a Web app and copy its config into `js/firebase.js`.
5. Deploy the Firestore rules from `firestore.rules`.

The Firebase web configuration is not a secret; Firestore Security Rules are the security boundary.
