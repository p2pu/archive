archive
=======

Static HTML of archive.p2pu.org

## Removing users:
- Find all pages with their name / user ID
- Remove ./users/<username>.html
- Update all links to ./users/<username>.html to ./users/anonymous.html
- Delete any profile pictures and use default image
- Anonymize any info on ./user/<id>/contact.html
- Remove user names from alt description in user profile images

Something like `ack username -l | xargs sed -i "s/username/anonymous/"` can help
