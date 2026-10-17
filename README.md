# fabriciolima.cloud

Landing page (perfil profissional de Fabricio Lima) servida como site estático via nginx.

## Deploy (EasyPanel + Docker)

O `Dockerfile` usa `nginx:alpine` e copia o `index.html`. No EasyPanel:

1. Crie uma **App** apontando para este repositório (Source = GitHub).
2. Build = **Dockerfile** (`./Dockerfile`).
3. Porta interna: **80**.
4. Em **Domains**, adicione `fabriciolima.cloud` e ative o HTTPS (Let's Encrypt).

O DNS do domínio deve apontar (registro A) para o IP da VPS.
