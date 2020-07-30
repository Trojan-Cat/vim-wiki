# These are some linux commands I use and why

## ls

lists directory contents

## chown
chown tochange who the owner of a directory is
exp: NPM modules that don't have permission to be installed, the NPM directory
might have been made under the wrong user such as root.

Fix: First check the folder to see who has permission to it
`ls -la /DIR`
That'll show you the owner
After that you want to check who you are logged in as
`id -un`
Now use chown on the folder
`sudo chown -R $USER /DIR`
The $USER will automatially grab the logged in user to be the one being set to
owner 
