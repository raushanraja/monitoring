# monitoring


- Sending log using loki api:

```bash
curl -i -XPOST -H "Content-Type: application/json" http://localhost:3100/loki/api/v1/push \
     --data '{"streams":[{"stream":{"type":"test"},"values":[['$(date +"%s%N")', "hello qryn"]]}]}'
```


- View:
    - qryn: http://localhost:3100/
    - grafana: http://localhost:3000/
        - user: admin
        - pass: admin
- qryn example:
![qryn dashbaord example](./2024-07-29-221231_951x419_scrot.png) 
