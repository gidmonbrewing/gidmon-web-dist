# gidmon-web-dist
Production Dist For gidmon-web

# Publishing
From your development environment run:
ember build --output-path=..\gidmon-web-dist\dist --environment=production

This assumes that you have gidmon-web-dist checked out in the same folder as gidmon-web.

Commit changes to gidmon-web-dist and push to GitHub.

On web server:
git pull to refresh
