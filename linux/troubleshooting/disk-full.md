# Sintoma: Disco Cheio

## 1. Verificar espaço

- `df -h`
- `df -i`

## 2. Localizar diretórios grandes

- `du -sh /* 2>/dev/null | sort -h | tail`

Verificar especialmente:
- /var/log
- /tmp
- backups antigos
- imagens Docker

## 3. Se Docker

- `docker system df`
- `docker image prune -a`
- `docker volume prune`

## Mitigação

- Limpeza controlada
- Rotação de logs
- Expandir volume (se possível)

## Prevenção

- Alertas > 70%
- Logrotate configurado
- Política de retenção