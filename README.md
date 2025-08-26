## Use OpenShift to proxy Homelab Services

### TLSRoutes

#### Example

```
---
service:
  name: my-external-service
  hostname: external.example.com
  port: 80
  addresses:
    - 192.168.192.168
gateway:
  name: my-gateway
  namespace: default
secured: true
```

### HTTPRoutes

#### Example

```
---
service:
  name: my-external-service
  hostname: external.example.com
  port: 80
  addresses:
    - 192.168.192.168
gateway:
  name: my-gateway
  namespace: default
secured: false
```
