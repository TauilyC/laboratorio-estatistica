# Estatística Aplicada à Psicologia: Laboratórios Interativos

Site estático servido por nginx (porta 3000).

| Rota | Conteúdo |
|---|---|
| `/` | Página inicial com os dois laboratórios |
| `/estatistica/` | Laboratório Interativo de Estatística |
| `/psicometria/` | Laboratório Interativo de Psicometria |

Cada laboratório é um único `index.html` autocontido, em sua pasta. Para atualizar um deles, substitua o arquivo e envie para a `main`; a Guara Cloud republica sozinha (auto deploy).

## Deploy na Guara Cloud
Repositório `TauilyC/laboratorio-estatistica`, branch `main`, root `/`, build Dockerfile, porta `3000`.

## Testar localmente
```bash
docker build -t labs .
docker run --rm -p 8080:3000 labs
```
