# CBM Wiki

# Status
on hold for right now, has issues with relative images, can't display excalidraw diagrams or work with any plugins
if those are solved, then might pick this back up

# Setup
One time setup: on the server to run the webserver, from project root, run `docker compose -f webserver/docker-compose.yml up`

# Usage
1. change content in /content either directly on Github, or by pushing changes to Github
2. changes should be reflected on the webserver after 30 seconds at http://localhost:8765

# Components
1. content - Primarily uses Obsidian flavored .md (markdown) files as content
2. server - Automatically generates html pages from files in /content directory
