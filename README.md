# Laboratório Interativo de Estatística

Site estático (um único `index.html`) servido por nginx na porta 80.

## Deploy na Guara Cloud
- Novo serviço → repositório `TauilyC/laboratorio-estatistica`, branch `main`
- **Root directory:** `/`
- Build: Dockerfile (`Dockerfile`), porta `80`, auto deploy ligado

## Testar localmente
```bash
docker build -t lab-estatistica .
docker run --rm -p 8080:80 lab-estatistica
```
