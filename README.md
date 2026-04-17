# Linux Server Setup

A simulated web server environment built as part of my Linux sysadmin learning path.

## What this project covers
- Linux filesystem structure
- User and group management
- File permissions with chmod and chown

## Structure
~/linux-server-setup/var/html/index.html -> web files, readable by everyone, writable by webteam
~/linux-server-setup/var/logs/access.log -> server logs, accessible by webteam only
~/linux-server-setup/var/logs/error.logs -> server logs, accessible by webteam only
~/linux-server-setup/var/config/db.conf  -> sensitive config files, owner access only

## Users & Groups
- Group: webteam
- Users: dev01, webuser (both members of webteam)

## Permissions
- html/index.html :  764
- logs/access.log :  760
- logs/error.logs :  760
- config/db.conf  :  600

## How to run
Clone the repo, create the users and group manually,
then apply permissions using chmod and chown as documented above.
