# Travlr Getaways — CS 465 Module One

This project serves the supplied Travlr Getaways static HTML through Node.js and Express. The Express Generator scaffold uses Handlebars for later coursework; Module One serves the HTML files in `public`.

## Run locally

Install Node.js LTS, then open Terminal in this folder:

```sh
npm install
npm start
```

Visit http://localhost:3000 in a browser. Leave Terminal running. Press Control+C to stop the server.

## Files

- `app.js`: Express middleware, static public directory, routes, and error handling.
- `bin/www`: HTTP server, default port 3000.
- `public/*.html`: original course pages.
- `public/css/style.css`: original stylesheet.
- `public/images/`: original images.
- `routes/` and `views/`: generator scaffold for subsequent modules.

The original static assets are supplied by SNHU in travlr.zip. Their existing attribution comments are preserved. The server scaffold was created with express-generator 4.16.1.

## Verify and submit

Open the home page and click Travel, Rooms, Meals, News, About, and Contact. Confirm images and styling load. This is a static shell: forms are not connected to a backend.

Capture a screenshot on your computer with the browser address showing localhost:3000 and the styled Travlr page. Submit that screenshot and the project ZIP. Also commit and push this project to the module1 branch of your own GitHub repository. This ZIP does not include your repository history or node_modules.

In your existing cloned course repository, copy these project files into its root (preserve its .git folder). Create the branch with `git switch -c module1`, or use `git switch module1` if it already exists. Then:

```sh
git add .
git commit -m "Complete Module One Express static website"
git push -u origin module1
```

If you have not cloned your course repository yet, clone your own GitHub URL first. GitHub upload has not been performed for you.

## Validation

HTTP checks passed for the home page, all 35 supplied files, and the 404 response. Node.js 24.22.1 was used. Browser visual testing was unavailable here; verify locally and capture your screenshot. Dependencies were updated while retaining Express 4 and HBS 4. npm audit reports one moderate HBS advisory with no available fix (GHSA-7f5c-rpf4-86p8); this course scaffold is intended for local development.
