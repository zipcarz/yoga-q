yoga-q
======
$ curl https://api.github.com/users/guyguy22 -I
HTTP/1.1 200 OK
X-GitHub-Media-Type: github.v3

$ curl https://api.github.com/users/guyguy22 -I \
  -H "Accept: application/vnd.github.full+json"
HTTP/1.1 200 OK
X-GitHub-Media-Type: github.v3; param=full; format=json

$ curl https://api.github.com/users/guyguy22 -I \
  -H "Accept: application/vnd.github.v3.full+json"
HTTP/1.1 200 OK
X-GitHub-Media-Type: github.v3; param=full; format=json
