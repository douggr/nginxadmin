# nginxadmin
Bash script to create, enable or disable a site in nginx.

## Requeriments
  - nginx. yes.
  - pre configured nginx with [h5bp/server-configs-nginx](https://github.com/h5bp/server-configs-nginx) files

## Usage
```shell
$ nginxadmin
Usage: nginxadmin <command> <filename> [document root]

Available commands:
  help                         : Show this message and exit.
  -c, create  <filename> <root>: Create (and enable) a new site.
  -e, enable  <filename>       : Enable an earlier created site.
  -d, disable <filename>       : Disable a site.

$ nginxadmin create test.io absolute/path/to/test.io/web-files
Testing nginx configuration… Ok
Site test.io has been enabled. 
Run "/usr/sbin/nginx -s reload" to apply the changes.
$ 
```
