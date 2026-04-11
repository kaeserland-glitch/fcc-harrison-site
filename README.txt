══════════════════════════════════════════════════════
  FIRST CHRISTIAN CHURCH — WEBSITE GUIDE
  fccharrison.org  |  Maintained by Kevin Kaeser
══════════════════════════════════════════════════════

YOUR SITE FOLDER CONTAINS:
  index.html        ← The entire website (one file!)
  images/           ← Put all your photos here
  README.txt        ← This guide
  css/              ← (reserved for future use)
  js/               ← (reserved for future use)


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  STEP 1 — ADDING YOUR PHOTOS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. Save your photos into the "images" folder.
   Suggested filenames:
     images/hero.jpg          ← Church exterior (main banner)
     images/sanctuary.jpg     ← Inside the sanctuary
     images/worship.jpg       ← Congregation or choir
     images/children.jpg      ← Children's Sunday School
     images/youth.jpg         ← Youth group
     images/community1.jpg    ← Congregation gathering
     images/events.jpg        ← A church event
     images/sundayschool.jpg  ← Sunday School class

2. Open index.html in a text editor (Notepad works fine,
   Notepad++ is even better — free at notepad-plus-plus.org).

3. Search for "📸" (copy/paste that emoji into the search bar)
   to jump to each photo placeholder.

4. For each placeholder, you'll see a block like this:
     <div class="photo-placeholder">
       ...
     </div>
   Replace that entire div with one line:
     <img src="images/hero.jpg" alt="First Christian Church" />

   That's it! One swap per photo.

PHOTO TIPS:
  • Horizontal photos (landscape) work best for most spots
  • The hero (top banner) looks best at 1920×1080 or wider
  • File size: try to keep each photo under 500KB
    (use squoosh.app — free — to compress them)
  • .jpg files work great for photos


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  STEP 2 — UPDATING TEXT & EVENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Open index.html in a text editor and use Ctrl+F (Find)
to search for text you want to change.

THINGS TO UPDATE:
  • Events: Search for "event-item" to find the events section
    Update the month, day, title, time, and description
    for each upcoming event.

  • Office Hours: Search for "Office Hours" — update the days/times

  • Address: Search for "Harrison, Arkansas 72601" — add your
    full street address

  • Facebook/Instagram links: Search for "facebook.com" and
    "instagram.com" — replace # with your actual page URLs

  • Google Map: Search for "maps/embed" — replace the src URL
    with your own embed from Google Maps:
      1. Go to maps.google.com
      2. Search your church address
      3. Click Share → Embed a map → Copy HTML
      4. Paste the src="..." value into index.html


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  STEP 3 — GOING LIVE ON NETLIFY (FREE)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Netlify hosts your site for FREE. You only pay for the
domain name (~$15/year wherever it's registered).

To deploy:
  1. Go to netlify.com and create a free account
  2. Click "Add new site" → "Deploy manually"
  3. Drag and drop your ENTIRE "fcc-harrison-site" folder
     onto the Netlify page
  4. Your site goes live in about 30 seconds with a
     temporary URL like "random-name.netlify.app"

To connect your domain (fccharrison.org):
  1. In Netlify → Site settings → Domain management
  2. Click "Add custom domain" → type fccharrison.org
  3. Netlify gives you DNS records to update
  4. Log in to wherever you registered fccharrison.org
     (GoDaddy, Namecheap, etc.) and update those records
  5. Takes 15 min to a few hours to go live

To UPDATE the site after changes:
  1. Make edits to your files on your computer
  2. Go back to Netlify → Deploys tab
  3. Drag and drop the folder again
  Done! Site updates in seconds.


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  SETTING UP THE PRAYER FORM (FREE)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

The prayer request form needs a free service to send
emails. Use Formspree (formspree.io — free for 50 msgs/mo):

  1. Sign up at formspree.io
  2. Create a new form → get your form ID (looks like "xrgvkpqz")
  3. In index.html, search for "handleForm"
  4. Uncomment the fetch() line and replace YOUR_ID with yours
  5. Change the <form> tag to:
       <form class="prayer-form" action="https://formspree.io/f/YOUR_ID" method="POST">
  6. Remove the onsubmit="handleForm(event)" attribute


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  COST SUMMARY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  Netlify hosting:      FREE (forever on free tier)
  Formspree forms:      FREE (up to 50 submissions/mo)
  Photo compression:    FREE (squoosh.app)
  Domain (fccharrison.org): ~$15/year (you already own it)

  TOTAL: ~$15/year  vs.  $450/year  =  $435 SAVED ✓


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  NEED HELP?
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Ask Claude at claude.ai — just paste your question and
mention "FCC website" and Claude can walk you through
any of these steps!

══════════════════════════════════════════════════════
