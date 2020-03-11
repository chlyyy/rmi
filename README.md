# rmi
docker  registry rmi script


optional arguments:
  -h, --help            show this help message and exit
  -l USER:PASSWORD, --login USER:PASSWORD
                        Login and password to access to docker registry
  -r URL, --host URL    Hostname for registry server, e.g.
                        https://example.com:5000
  -d, --delete          If specified, delete all but last 10 tags of all
                        images
  -n [N], --num [N]     Set the number of tags to keep(10 if not set)
  --dry-run             If used in combination with --delete,then images will
                        not be deleted
  -i IMAGE:[TAG] [IMAGE:[TAG] ...], --image IMAGE:[TAG] [IMAGE:[TAG] ...]
                        Specify images and tags to list/delete
  --keep-tags KEEP_TAGS [KEEP_TAGS ...]
                        List of tags that will be omitted from deletion if
                        used in combination with --delete or --delete-all
  --tags-like TAGS_LIKE [TAGS_LIKE ...]
                        List of tags (regexp check) that will be handled
  --keep-tags-like KEEP_TAGS_LIKE [KEEP_TAGS_LIKE ...]
                        List of tags (regexp check) that will be omitted from
                        deletion if used in combination with --delete or
                        --delete-all
  --no-validate-ssl     Disable ssl validation
  --delete-all          Will delete all tags. Be careful with this!
  --layers              Show layers digests for all images and all tags
