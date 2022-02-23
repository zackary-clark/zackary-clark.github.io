# Zack's Portfolio

## Releasing

1. Commit code to be released.
2. Run `npm build`
3. Move static files in `./build` to `portfolio-claim` for K8s Nginx container to serve
4. `kubectl rollout restart deployment portfolio-deployment` (technically only necessary if index.html changes)