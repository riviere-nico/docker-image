LOGIN TO GITHUB PACKAGE REGISTRY :

cat ~/Bureau/github_registry_token.txt | docker login https://docker.pkg.github.com -u riviere-nico --password-stdin


BULD IMAGE :


docker build -t docker.pkg.github.com/riviere-nico/docker-image/docker-simple-test_web:latest .


PUSH IMAGE :


docker push docker.pkg.github.com/riviere-nico/docker-image/docker-simple-test_web:latest

