# Roof Mockup Studio

Web apps for the California JATC (Central Valley) Plan and Design class. Apprentices design single-ply and steep-slope roof mockups board by board, check them, and build from the cut list.

| Page | What it is |
| --- | --- |
| `index.html` | Start page with links to both apps |
| `studio.html` | Roof Mockup Studio: one tablet per team, saved on the iPad |
| `team.html` | Roof Mockup Studio Team: one tablet per team, or live team sync across several iPads |

Both apps are single, self-contained HTML files: all libraries are built in, so they keep working after they load even without internet. Team sync needs internet.

## Team sync

Team sync uses a Firebase Realtime Database (project `roof-mockup`). Tablets sign in anonymously in the background; students never log in. Database rules allow reads and writes only under `classes/` and only for signed-in tablets.

## Updating

Replace `studio.html` or `team.html` with a new version and commit. GitHub Pages republishes in a minute or two. Designs saved on the iPads are kept.
