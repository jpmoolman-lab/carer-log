# Carer Visit Log App

A simple mobile-friendly web app for carers to sign out of visits.

## How it works
1. Open `index.html` (or the hosted landing page).
2. A QR code is displayed that links to the form.
3. Carers scan the QR code with their phone camera.
4. They fill in:
   - Carer's Name
   - Date (auto-filled to today)
   - Time Arrived
   - Planned Leave Time
   - Actual Sign-out Time (auto-filled to current time, editable)
5. On submit, the details are emailed to:
   - jpmoorman@gmail.com
   - jpm@fsace.com.au (CC)

## Hosting (required for QR + emails to work properly)
Upload these files to any static host:
- **Netlify Drop**: Drag the folder to https://app.netlify.com/drop
- **GitHub Pages**, Vercel, Cloudflare Pages, etc.
- Or any web server.

Once hosted, the QR code will automatically point to the correct `form.html` URL.

## Email setup
Uses [FormSubmit](https://formsubmit.co) (free, no account required).
- First time you submit a real form, FormSubmit will send a confirmation email to `jpmoorman@gmail.com`. Click the link to activate.
- After that, every submission emails both addresses automatically.
- Spam protection included via honeypot.

## Files
- `index.html` — Landing page with QR code
- `form.html` — The sign-out form
- `thanks.html` — Success page

## Customisation
- Change colours or text directly in the HTML files.
- To use a different email service later, update the form `action` and hidden fields in `form.html`.

Built for easy use by carers on their phones.
