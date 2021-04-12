# Spring-Cloud-Config-Demo

- [reference doc](https://cloud.spring.io/spring-cloud-config/reference/html/)

## demo-1

demo-1 is from [here](https://cloud.spring.io/spring-cloud-config/reference/html/).

when you curl the server, you will see these:

```bash
$ curl localhost:8888/foo/development
{"name":"foo","label":"master","propertySources":[
  {"name":"https://github.com/scratches/config-repo/foo-development.properties","source":{"bar":"spam"}},
  {"name":"https://github.com/scratches/config-repo/foo.properties","source":{"foo":"bar"}}
]}
```

## demo-2

See this  [branch](https://github.com/caliburn1994/Spring-Cloud-Config-Demo/tree/demo-2), get config from Github.

```bash
$ curl localhost:8888/foo/development/main
```

### demo-3

See this  [branch](https://github.com/caliburn1994/Spring-Cloud-Config-Demo/tree/demo-3)

1.  Run `\Spring-Cloud-Config-Demo\src\main\java\kyakya\icu\cloudconfig\CloudConfigApplication.java`
2. Run `\Spring-Cloud-Config-Demo\client-test\src\main\java\kyakya\icu\clienttest\ClientTestApplication.java`
   1. After starting,  click http://localhost:8080/message .

ref: https://spring.io/guides/gs/centralized-configuration/

## TODO

- [ ] server with dir,not git rep

- [ ] client get config from git rep, not server.