# SavageWolf Official — V11 editable showcase

Based on approved Version 10. The original embedded banner and product mockups remain as fallbacks. No payments or checkout are enabled.

## Launch
1. Create a GitHub account and a new PRIVATE repository (e.g. savagewolf-website).
2. Upload the **contents** of this folder into the repository root, including the hidden `.pages.yml` file. GitHub web upload may not show hidden files in some file pickers; verify it is present. For easiest setup use GitHub Desktop to commit and push this folder.
3. In Netlify, choose **Add new project > Import an existing project > GitHub**. Select your repository. Set publish directory to `.` and deploy (no build command).
4. Open the temporary `*.netlify.app` address to test. Tap **ENTER THE SAVAGES DEN** to start the music.
5. Visit https://pagescms.org/ and sign in with GitHub, authorize access to your repo, and select it. The dashboard uses `.pages.yml` and lets you edit **Website Settings** and **Merchandise Showcase**. Save/commit changes and Netlify automatically redeploys.
6. Purchase the domain `SavageWolfOfficial.com` if available, then in Netlify select **Domain management > Add a domain**, and follow Netlify's current DNS directions for your registrar. Enable HTTPS and test mobile.

## Editable content
- `site.json`: entrance, headings, announcements, Twitch link, soundtrack path/volume, and optional hero image.
- `products.json`: existing eight product names, categories, concept prices, visibility, and replacement image paths.
- To replace imagery, upload images into `media/` and set a field to `/media/filename.jpg`.
- To replace the soundtrack, upload the new MP3 to the repo and edit `music_file`.

**Important limitations:** This first release preserves eight product slots; adding more slots requires a layout change. A Pages CMS save creates a GitHub commit; it is not an in-page drag-and-drop editor. Keep the repository private until you understand any repository access/hosting implications. Confirm Pages CMS supports your repository's visibility under your plan.

**Licensing:** The supplied MP3 is Content ID registered; check the Pixabay license and any Content ID claims before a public launch.

**Testing:** Open from a hosted HTTPS site, not the iPhone Files/ChatGPT file preview; those previews can block audio and JSON fetches.
