
#### Status:
In order to unpack this project in a new space:

0. Clone this repository into your project's static folder, probably `/static/`
1. install npm, gulp, bower.
2. gulp has dependencies in gulpfile.js, bower has dependencies in bower.json.
3. Put your assets in the src folder.
4. Build dist for the first time by running `$ gulp`

#### Notes:
- Carefully review the .gitignore for new projects.
- Currently ignored: dist/, bower_modules/, node_packages/
- There are options in gulpfule.js to install or update bower.


#### Special Tooling:
- Added bower dependencies to satisfy the needs of pinax-bootstrap.
- These dependencies need to be wired into gulp and subsequently into whatever base.html or site_base.html is used by the web app.

#### TODO:
Looks like there isn't any default css minifier. Add one! See sage/roots gulpfile.
Fix vendor to copy directly from src to dist.  This doesn't behave quite right, currently.
