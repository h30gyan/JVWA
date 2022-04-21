# JVWA

java 代码审计学习靶场,边学边完善

## 目前支持

- spring actuator (web 和 jmx 方式)
  - `http://127.0.0.1:8999/actuator`
  - `http://127.0.0.1:8999/actuator/env`
  - `http://127.0.0.1:8999/actuator/heapdump`
  - `http://127.0.0.1:8999/actuator/mappings`
  - `http://127.0.0.1:8999/actuator/prometheus`
- swagger
  - `http://127.0.0.1:8999/swagger-resources`
  - `http://127.0.0.1:8999/swagger-ui.html`
  - `http://127.0.0.1:8999/v2/api-docs`
- druid
  - `http://127.0.0.1:8999/druid/login.html` admin/admin
- spel注入
  - `http://127.0.0.1:8999/spel?exec=1`
- mysql注入
  - `http://127.0.0.1:8999/user/mysql/getbyid/1`
- postgresql注入
  - `http://127.0.0.1:8999/user/postgre/getbyid/1`
- url跳转漏洞
  - `http://127.0.0.1:8999/redirect/1?url=` 无过滤
  - `http://127.0.0.1:8999/redirect/2?url=` 可以被绕过的白名单案例
  - `http://127.0.0.1:8999/redirect/3?url=` 反斜杠绕过
  - `http://127.0.0.1:8999/redirect/safe?url=` 安全案例
- log4j
