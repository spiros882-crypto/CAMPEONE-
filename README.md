# CAMPEONE — Release Candidate 1

Έτοιμο πακέτο web/PWA για έκδοση σε hosting που υποστηρίζει Node.js 20+ και persistent disk. Η εφαρμογή ανοίγει από κινητό και μπορεί να εγκατασταθεί ως PWA.

## Περιλαμβάνει
- 12 παίκτες / 8 συμμετέχοντες ανά αγωνιστική / 4 ζευγάρια
- κοινή online βάση SQLite στον server
- live συγχρονισμό με WebSocket
- ξεχωριστό κωδικό παίκτη και admin
- φύλλα αγώνα
- ατομικά γκολ/ασίστ
- κοινά άμυνα/γκολ κατά/ομαδικοί βαθμοί
- αυτόματο Train
- MVP ανά ημερολογιακό μήνα
- πίνακα 66 ζευγαριών
- σχολές και ιστορικό αλλαγών
- παραμετροποιήσιμους κανόνες
- PWA

## Προεπιλεγμένοι κωδικοί
- Παίκτες: `CAMPEONE`
- Admin: `CAMPEONE-ADMIN-2026`

**Πριν από πραγματική χρήση άλλαξε και τους δύο κωδικούς και το JWT_SECRET μέσω environment variables.**

## Τοπική εκτέλεση
```bash
npm install
npm start
```
και άνοιξε `http://localhost:3000`.

## Deployment
Χρησιμοποίησε hosting Node.js με persistent disk. Για Docker υπάρχει έτοιμο `Dockerfile`. Το database file πρέπει να βρίσκεται στο `/data/campeone.db`.

## Σημείωση
Αυτή η έκδοση είναι Release Candidate. Το online Supabase project CAMPEONE έχει ήδη δημιουργηθεί, αλλά το συγκεκριμένο πακέτο χρησιμοποιεί τον δικό του persistent SQLite server ώστε να μπορεί να εκδοθεί άμεσα χωρίς να εξαρτάται από μη διαθέσιμο deployment connector.
