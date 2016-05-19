# website-content
The content folder for Pelican

## Content variables
Content files can contain a number of different variables to be parsed by pelican.

While you should not have to directly edit these most times you might have to use the variables for pathing relative to server root.

The configuration file sets what the site url will be which may change based on if it is being published to production or a qa site.  For example production will all be starting at / like /images or http://thelab.ms/images but the qa site might start with /website-content/ line /website-content/images or http://thelab-ms.github.io/website-content/

So in order to make sure internal links work properly you should use the {filename} variable on content pages.

Do not simply create an internal link to content such as href="/images/abc.gif" and expect it to work!  Use the proper variable format of href="{filename}/images/abc.gif" and it will work fine.

See the website-pelican repository README.md file for more details.

