# simple docker private registry viewer
a really simple (and ugly) docker private registry viewer

## features
- list/search repository (make sure your registry support search)
- list tags for repository
- show details of repository.
- delete tags
- delete repository
- support authentication (HTTP Basic Auth), in case you implemented
- bookmarkable, you can save repository address, search as well as username but not password

## install
it's just a single HTML file, copy it to you web server and make it accessible

## configure
if you put on the same server as your docker registry, then no configuration needed
if you put on server other than your docker registry, you need to enable CORS support (not suggested), your docker registry software should have related info
to bookmark the page, you can put parameters repo, username and/or search keyword (any combination) like:

```
http://myrepo.myorg.com/index.html?repo=http://myrealrepo.myorg.com:5000&search=mylib&username=IamRoot
```

