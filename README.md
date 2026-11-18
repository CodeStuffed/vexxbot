# Stacker robot build site

A static website: how to build the stacker robot, step by step. Plain HTML, no build tools.

## Put it on GitHub Pages

1. Make a new repository on GitHub and upload everything in this folder (keep the folders as they are).
2. In the repository go to **Settings > Pages**. Under **Source** pick **Deploy from a branch**, branch `main`, folder `/ (root)`, then **Save**.
3. After a minute the site is at `https://<your-user-name>.github.io/<repository-name>/`.

To look at it without GitHub, run `python -m http.server` in this folder and open http://localhost:8000. The 3D steps need a web server and the internet (they load three.js from a CDN); opening `index.html` straight from disk works for everything else.

## What's here

- `index.html`: start here: before you start, tools, how to read the steps, cut list, videos
- `build3d/`: animated 3D build steps with the real VEX part models (needs a web server such as GitHub Pages)
- `steps/`: the same steps as pictures (arrow keys or Back / Next)
- `parts.html`: every part with counts, for version A and B
- `media/`: the videos and pictures

Made from the CAD model by `cad/build/make_site.py`. Run it again after the robot changes.
