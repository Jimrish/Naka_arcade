# Shielded Naka Arcade

Professional responsive game portal for Vercel. The homepage contains the eight supplied game links and uses local cover art in `assets/`.

## Deploy to Vercel
1. Extract this ZIP.
2. Create a GitHub repository and upload `index.html` plus the complete `assets` folder, or import the repository directly into Vercel.
3. In Vercel, choose **Add New → Project**, import the repository, and deploy.
4. Framework preset: **Other**. Build command: leave empty. Output directory: `.` (root). No environment variables are required.
5. Vercel will provide a deployment URL.

This is a static website; it does not require a server, database, API key, or paid hosting plan for basic use.

## Add more games later
Open `index.html`, find `const games = [ ... ]`, and add another object:
`{name:"New Naka Game",category:"arcade",description:"Short game description.",image:"assets/new-cover.jpg",url:"https://your-game.vercel.app/"}`
Upload the new cover image into `assets/`. Categories supported by the filters: `arcade`, `racing`, `action`, `collect`.
No fixed game-count limit is coded into the site.

## Video previews
The uploaded MP4 is used as a muted looping hover preview on both Shielded Car Race and Naka Hill Rush. Keep `assets/car-hill-rush-preview.mp4` in the assets folder when deploying. If the same recording does not contain both games, replace it with the correct separate recording for the relevant card.

## Homepage video banner
The uploaded MP4 is shown as a wide 16:9 video banner immediately below the site navigation at the top of the homepage. It is muted, autoplaying, looping and inline on mobile, with visible playback controls. Keep `assets/homepage-showreel.mp4` in the assets folder when deploying.

## Latest homepage video and X profile
The latest uploaded MP4 is used in the prominent homepage showreel banner directly below the navigation and above the hero introduction. It autoplays muted, loops, and has playback controls. The header and hero include links to https://x.com/satoshijex.
Keep `assets/shielded-naka-homepage.mp4` in the assets folder.
