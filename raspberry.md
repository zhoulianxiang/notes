### backup ###

- dd if=/dev/sdX | gzip > img.gz
- gzip -dc img.gz | dd of=/dev/sdX
