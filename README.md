# Impact Ministry Linktree Page

A mobile-friendly landing page for the GPCC Singles Impact Ministry.

## Files Included

- `gpcc-singles.html` — The main landing page
- `impact-logo.png` — The Impact Ministry logo

## Setup

1. Upload both files to your web hosting service (e.g., GitHub Pages, Netlify, your church website)
2. Make sure both files are in the same folder/directory
3. The page will be accessible at your hosted URL

## Customization

### Updating Links

Find the `<!-- Link Buttons -->` section near the bottom of the HTML file. To add more buttons, copy this template:

```html
<a href="YOUR_URL_HERE" class="btn btn-outline" target="_blank">
    Button Text Here
</a>
```

Common links you might want to add:
- GroupMe invite link
- Instagram profile
- Event registration
- Church website

### Updating Service Times/Locations

Find the `<!-- Sunday Worship Services -->` section. Each location is inside an `accordion-item` div. Update the text inside:
- `.service-time` — Change the service time
- `.service-address` — Change the address (update both the display text and the Google Maps link)

### Connecting the Email Form

The form currently shows a success message but doesn't send data anywhere. To make it functional, you have a few options:

**Option 1: Google Forms**
Replace the form with an embedded Google Form iframe.

**Option 2: Formspree (free tier available)**
1. Sign up at [formspree.io](https://formspree.io)
2. Replace the form's `onsubmit` with: `action="https://formspree.io/f/YOUR_FORM_ID" method="POST"`
3. Remove the `onsubmit="handleSubmit(event)"` attribute

**Option 3: Mailchimp**
Use Mailchimp's embedded form code to replace the existing form section.

### Changing Colors

The color scheme is defined at the top of the `<style>` section in CSS variables:

```css
:root {
    --primary: #7c3aed;       /* Main purple */
    --primary-dark: #6d28d9;  /* Darker purple for hover states */
    --primary-light: #ede9fe; /* Light purple for highlights */
    --accent: #60a5fa;        /* Blue accent */
    /* ... */
}
```

## Hosting Options

Here are some free/low-cost ways to host this page:

| Service | Cost | Notes |
|---------|------|-------|
| GitHub Pages | Free | Requires GitHub account |
| Netlify | Free | Drag-and-drop upload option |
| Vercel | Free | Good for simple static sites |
| Church website | Varies | Upload to existing hosting |

## Support

For questions or changes, reach out to your web team or the person who created this page.
