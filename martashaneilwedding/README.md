# Wedding site – setup

1. Copy this whole `martashaneilwedding` folder into the root of your GitHub Pages repo, commit and push.
   It goes live at shaneiln.com/martashaneilwedding/
2. **Change the password** (starter password is `ChangeMe2027`):
   - Open any page in your browser, press F12, open the Console, and run:
     `crypto.subtle.digest("SHA-256",new TextEncoder().encode("YOURPASSWORD")).then(b=>console.log([...new Uint8Array(b)].map(x=>x.toString(16).padStart(2,"0")).join("")))`
   - Paste the result over the long hash after `const HASH=` in `details/index.html`.
3. **RSVP form:** create a free form at formspree.io, then replace `YOUR_FORM_ID` in `rsvp/index.html` with your form ID.
4. Replace every highlighted TBC (class `todo`) in `details/index.html` and `rsvp/index.html`.
5. **Names font:** add `ADayWithoutSun.ttf` (or `.woff2`) to the `fonts` folder - see `fonts/README.txt`.
6. Colours live at the top of `style.css` (background #FFF6EF, text #74323E). Artwork is `images/artwork.webp`.

Note: the details password is a soft gate. The content is still in the page source, so keep anything sensitive off it.
To remove the site later: delete this folder, commit, push.
