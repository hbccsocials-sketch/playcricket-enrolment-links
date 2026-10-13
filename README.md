# PlayCricket Learn Enrolment Link Generator

A static web app that extracts the UUID after `/event/` from a PlayCricket Learn admin URL and the UUID after `/module/` from a learner URL, then generates:

`https://learn.cricket.com.au/module/{moduleId}/event/{eventId}/enrol`

## Use
Open `index.html` in a browser, or deploy the folder to GitHub Pages, Netlify, or Vercel. No dependencies, accounts, API keys, or backend required.

## Deploy to Vercel
Create a GitHub repository containing `index.html` at its root, import the repository into Vercel, and deploy using the **Other** framework preset. No build command is needed.

The generator checks the expected HTTPS domains and UUID path segments. It does not check that the event exists or is open.

Supported module URLs: learner standalone, learner certification pathway, and admin /module/{id}/versions/{versionId}. The first ID after /module/ is used.
