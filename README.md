# webman [![Travis-CI](https://api.travis-ci.org/ostera/webman.svg)](https://travis-ci.org/ostera/webman)
> :globe_with_meridians::man: An Erlang tool to scaffold and inspect webmachine applications.

Use it to start up a project, or inspect existing ones, without altering your typical build toolchain.

## Tutorial

```bash
$ webman init --name myapp
webman v0.1.0

Scaffolfing base app:
  > Setting up rebar.config
  > Pulling dependencies

$ webman resource users
webman v0.1.0

Creating users endpoint:
  > Module:         src/myapp_users.erl
  > Fixtures:       test/myapp_users_fixtures.erl
  > Unit tests:     test/myapp_users_test.erl
  > Property tests: test/myapp_users_prop_test.erl
  > Common tests:   test/myapp_users_common_test.erl

$ webman resource --list
webman v0.1.0

Resources:
  * /api/users  => src/myapp_users.erl

$ webman resource users
webman v0.1.0

> DELETE /api/users
> GET    /api/users
> HEAD   /api/users
> POST   /api/users
> PUT    /api/users

Accept: application/json
Accept-Charset: UTF-8
Accept-Encoding: identity, gzip, deflate
Accept-Language: en-us, en; q=0.5

Content-Type: text/html, application/json
```
