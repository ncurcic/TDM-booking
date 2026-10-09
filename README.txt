TDM Booking — Firebase-connected prototype

1. In Firebase Console > Firestore Database > Rules, paste firestore.rules and Publish.
2. Ensure the three Authentication user UIDs have matching authorizedUsers documents with active=true.
3. To publish, use Firebase Hosting via Firebase CLI on a computer, or another static HTTPS hosting provider. The app is not hosted by this ZIP.
4. Open the HTTPS site on iPhone in Safari and choose Share > Add to Home Screen.

IMPORTANT: This prototype checks overlapping bookings against currently loaded records, but concurrent edits from multiple phones can still cause double bookings. It is not yet production safe. Implement atomic occupancy locks and stricter server-side validation before relying on it for real guests. Test all three accounts and database rules first. Do not upload personal guest data until these protections are complete.
