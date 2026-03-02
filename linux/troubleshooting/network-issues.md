# Sintoma: Problemas de Rede

## 1. Verificar conectividade básica

- `ip a`
- `ip r`
- `ping -c 3 8.8.8.8`
- `ping -c 3 google.com`

Se IP responde mas DNS não → problema DNS.

## 2. Verificar portas

- `ss -tulpn`
- Firewall:
  - `ufw status`
  - `iptables -L -n`

## 3. Verificar latência

- `mtr <host>`
- `traceroute <host>`

## 4. VPN

- `wg show`
- `systemctl status openvpn`

## Mitigação

- Reiniciar serviço de rede
- Reiniciar túnel VPN
- Verificar rotas incorretas