# Song Suggestion Form — Build Plan

A step-by-step plan for adding a song suggestion form to the K'YRAS website.
Each step is scoped to be reviewable and testable in 5–10 minutes.

---

## Step 1 — Add a blank "Suggest a Song" page with navigation link

- Create `suggest.html` with the existing header/footer/nav structure
- Add a "Suggest" link to the nav on all pages
- **Test:** Click through nav on every page, confirm the new link works and the page loads with correct styling.

## Step 2 — Build the form HTML (no styling yet)

- Add the form fields: name (optional), song title, artist, genre dropdown, and a message/reason textarea
- Add a submit button
- **Test:** Open the page, confirm all fields render and are interactive (can type, select, etc.).

## Step 3 — Style the form to match the neon/cyber theme

- Add CSS for form inputs, labels, the submit button, and layout — using existing CSS variables (`--neon-cyan`, `--bg-panel`, etc.)
- **Test:** Visually compare against other pages. Resize browser to check mobile responsiveness.

## Step 4 — Add client-side validation

- Make song title and artist required
- Show inline error messages if the user submits with empty required fields
- **Test:** Try submitting empty, partially filled, and fully filled forms. Confirm error messages appear/disappear correctly.

## Step 5 — Add a submission confirmation state

- On valid submit, hide the form and show a "Thanks for your suggestion!" message with a neon glow
- No actual backend — this is a visual confirmation only
- **Test:** Fill out the form, submit, confirm the thank-you message appears. Refresh to confirm the form resets.

---

## Optional Future Steps

- Hook up to a free form service (Formspree, Netlify Forms, etc.) for real submissions
- Add a "suggest another" button to the confirmation state
