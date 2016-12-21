# gidmon-web-dist
Production Dist For gidmon-web

# Publishing
From your development environment run:
ember build --output-path=..\gidmon-web-dist\dist --environment=production

This assumes that you have gidmon-web-dist checked out in the same folder as gidmon-web.

Commit changes to gidmon-web-dist and push to GitHub.

# Web server setup

We assume that the web site is located at /var/www/gidmon/.

If this is the initial setup of the server we run: git clone https://github.com/gidmonbrewing/gidmon-web-dist.git.

If you have already cloned the repository go into /var/www/gidmon/gid-web-dist/ and run: git pull.

We assume the site root points to: /var/www/gidmon/gid-web-dist/.

For nginx that would look like this:

server {
	listen 80;
	server_name gidmon.se www.gidmon.se;
	root /var/www/gidmon/gidmon-web-dist/dist;
	
	...
	...
}

