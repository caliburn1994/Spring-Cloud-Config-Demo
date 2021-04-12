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

