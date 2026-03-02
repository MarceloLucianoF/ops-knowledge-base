# Sintoma: Alta Latência

## Passo 1 — Verificar Saturação

### CPU
- `uptime`
- `top -o %CPU`
- load maior que número de cores?

### Memória
- `free -h`
- swap ativa?
- `vmstat 1 5`

### Disco
- `iostat -xz 1 3`
- %util > 80%?

### Rede
- `ss -s`
- `iftop`
- retransmissões?

---

## Passo 2 — Verificar Aplicação

- Logs recentes:
  - `journalctl -u <servico> -n 100`
- Erros 5xx?
- Conexões esgotadas?

---

## Mitigação rápida

- Scale horizontal
- Restart controlado
- Limitar tráfego
- Ativar cache temporário

---

## Pós-incidente

- Registrar métricas p95/p99
- Ajustar alertas
- Revisar capacity planning