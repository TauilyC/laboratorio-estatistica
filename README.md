# Laboratório Interativo de Estatística

Site estático (um único `index.html`) servido por nginx na porta 80.

## Deploy na Guara Cloud
- Novo serviço → repositório `TauilyC/atlas-3d-encefalo`, branch `main`
- **Root directory:** `/laboratorio-estatistica`
- Build: Dockerfile (`Dockerfile`), porta `80`, auto deploy ligado

## Testar localmente
```bash
docker build -t lab-estatistica laboratorio-estatistica
docker run --rm -p 8080:80 lab-estatistica
```
