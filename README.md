# Zack's Portfolio

## Releasing

1. Commit code to be released.
2. Tag commit with next version.
3. Push code and tag with `git push --tags && git push`
4. Docker build `docker build ./ -t zackaryclark/portfolio:latest -t zackaryclark/portfolio:<commit-tag-just-used>`
5. Docker push `docker push zackaryclark/portfolio:latest && docker push zackaryclark/portfolio:<commit-tag-just-used>`
6. Kubectl context switch `kubectl config use-context prod`
7. Rollout new container `kubectl rollout restart deployment portfolio-deployment`