# Aryan Rahman Portfolio — Setup

## Files
index.html            Main website (HTML + Tailwind CSS + Vanilla JS)
content/site.json     All editable text, services, stats, skills and projects
admin/index.html      Decap CMS dashboard  ->  yoursite.netlify.app/admin
admin/config.yml      CMS configuration
images/               Hero photo, logo and project pictures (uploads go to images/uploads)

## Deploy (GitHub + Netlify)
1. Create a new GitHub repository and upload everything in this folder (keep the folder structure).
2. Netlify -> Add new site -> Import from Git -> choose the repo. Build command: (empty). Publish directory: (empty / root).
3. Netlify -> Project configuration -> Identity -> Enable Identity. Set Registration to "Invite only".
4. Identity -> Services -> Git Gateway -> Enable Git Gateway.
5. Identity -> Invite users -> invite your email, open the email link and set your password.
6. In admin/config.yml replace YOUR-SITE.netlify.app with your real Netlify domain.
7. Open https://YOUR-SITE.netlify.app/admin and log in.

## Admin login
The CMS logs in with EMAIL + PASSWORD through Netlify Identity (a plain username such as "ADMIN"
cannot be configured in Decap CMS). Use your email address and the password you set in step 5.
No password is stored in any file of this project, because the repository and /admin are public.

## Things to edit before going live
- Email address, stats numbers, skill percentages and project links are placeholders:
  edit them in /admin -> Homepage, or directly in content/site.json.
- Change the accent color in /admin -> Settings (for example orange: #F97316).
