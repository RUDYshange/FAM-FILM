# Turnover

**The call sheet stops being a PDF.**

A live, personalised call sheet for commercial film production. Every person on the sheet
opens one link and sees only their own day. Production sees who has actually read it, and
can move the schedule without sending another attachment.

**Live site:** https://rudyshange.github.io/turnover/

---

## What's here

| File | What it is |
|---|---|
| `index.html` | Landing page — demo video, problem, live prototype, proposal |
| `app.html` | The full interactive prototype. Four roles, five tabs, staged publishing |
| `roles.html` | Permission model — the same shoot day rendered under four roles |
| `concept.html` | Original concept sketch: crew phone beside a production console |
| `assets/demo.mp4` | 75-second captioned walkthrough (no audio) |
| `assets/Turnover-Proposal.pdf` | Nine-page pilot proposal |

No build step, no dependencies, no framework. Plain HTML, CSS and JavaScript.
Everything runs in the browser and no data leaves the page.

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Try the prototype

1. Signed in as **Barry, 1st AD** — open **SHOTS**, add **+15 min** to the patio setup
2. The change stages as a draft. Press **Publish**
3. Switch to **Edmond, AD Trainee** — his wrap time and meals have already moved
4. Switch to **Suki, Coordinator** — the **CONTROL** tab appears; nudge the 15 who never opened it
5. Switch to **Kagiso, Agency guest** — the crew tab is gone and locations are hidden

## Status

Working prototype, seeking a pilot production. The permission checks are currently
client-side, which is fine for a demo and not for production — every request needs to be
authorised server-side against `(user, project, role)`.

## Note on data

All names, brands, crew and schedule data are fictional. Production paperwork carries
confidentiality obligations and real personal contact details, so nothing here is drawn
from a live call sheet — only the shape of the problem.

## Contact

Edmond Itumeleng Shange · Gauteng, South Africa
[itumelengshange016@gmail.com](mailto:itumelengshange016@gmail.com) · [github.com/RUDYshange](https://github.com/RUDYshange)
