# mukeles42 - K3d + Argo CD GitOps Demo

Bu repository K3d ve Argo CD kullanarak GitOps workflow'unu göstermektedir.

## Uygulama
- **Image**: wil42/playground
- **Port**: 8888
- **Versions**: v1, v2

## Deployment
1. K3d cluster oluşturun
2. Argo CD'yi kurun
3. Bu repository'yi Argo CD'ye kaydedin
4. Otomatik sync ile uygulama deploy edilir

## Version Değiştirme
`manifests/deployment.yaml` dosyasında image tag'ini `v1`'den `v2`'ye değiştirin:
```yaml
image: wil42/playground:v2
