AMM STEP TRAINER - how to share it as an app
=============================================

What's in this folder
  index.html             the app
  three.min.js           3D engine (three.js r128, MIT licence - see THREE-LICENSE.txt)
  manifest.webmanifest   lets phones install it with its own icon
  sw.js                  makes it work offline after the first visit
  icons/                 app icons

Put it online (free, about 5 minutes) - GitHub Pages
  1. Sign in at github.com and create a new public repository, e.g. "amm-trainer".
  2. Click "uploading an existing file" and drag in EVERYTHING from this folder
     (keep the icons folder). Commit.
  3. Go to Settings > Pages. Under "Build and deployment", choose
     "Deploy from a branch", branch "main", folder "/ (root)". Save.
  4. After a minute or two your link appears at the top of that page, like:
     https://YOUR-USERNAME.github.io/amm-trainer/
  Any other static host (Netlify, Vercel, Cloudflare Pages) works too:
  upload the whole folder as it is. It must be served over https.

Send your friends the link. Then:
  Android (Chrome)   open the link > tap "Install" in the app's header,
                     or Chrome menu > "Add to Home screen"
  iPhone (Safari)    open the link > Share button > "Add to Home Screen"
  Laptop (Chrome/Edge) open the link > install icon in the address bar
  Meta Quest         open the link in Meta Quest Browser > tap "Enter VR"

Once installed it opens full screen from its own icon and works offline.

Updating it
  Change the files, upload them again, and change CACHE = "amm-trainer-v1"
  in sw.js to "v2" so everyone's installed copy picks up the new version.

Important
  The steps and the torque value in this demo are illustrative training
  content, not taken from an approved AMM. Do not put real AMM task data on a
  public site - that data belongs to the manufacturer / operator. Keep any
  version with real tasks on an internal, access-controlled server.
