# Sintoma: Serviço Indisponível

## 1. Verificar status

- `systemctl status <servico>`
- `journalctl -u <servico> -n 200`

## 2. Checar dependências

- Banco disponível?
- DNS resolve?
- Porta aberta?
  - `ss -tulpn | grep <porta>`

## 3. Recursos do host

- Disco cheio?
- OOM killer?
  - `dmesg | grep -i kill`

## Mitigação

- Restart seguro
- Rollback se deploy recente
- Failover se existir

## Comunicação

- Classificar severidade (SEV)
- Atualizar stakeholders