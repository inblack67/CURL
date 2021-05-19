### cURL

- Supports protocols like http, https, ftp etc

```sh
curl https://jsonplaceholder.typicode.com/posts

# -I or --head includes the header info
curl --head https://jsonplaceholder.typicode.com/posts

# includes the other info, header etc
curl -i https://jsonplaceholder.typicode.com/posts

# output res to a file
curl -o posts.json https://jsonplaceholder.typicode.com/posts

# download => image can be downloaded like this too
curl -O https://jsonplaceholder.typicode.com/posts

# limit transfer rate for download
curl -O --limit-rate 1000B https://jsonplaceholder.typicode.com/posts

# post => -d or --data
curl --data "title=hello&body=worlds" https://jsonplaceholder.typicode.com/posts

# put
curl -X PUT -d "title=hello" https://jsonplaceholder.typicode.com/posts/1

# delete
curl -X  DELETE https://jsonplaceholder.typicode.com/posts/1

# auth
curl -u $username:$password http://...

# redirection => follow up => http to https, https to www
curl -L https://google.com
```
