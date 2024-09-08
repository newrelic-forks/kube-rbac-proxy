FROM alpine:3.19.4

RUN apk add --no-cache curl

CMD curl -v -s -k -H "Authorization: Bearer `cat /var/run/secrets/kubernetes.io/serviceaccount/token`" https://kube-rbac-proxy.default.svc:8443/metrics
