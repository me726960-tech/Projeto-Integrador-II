# Relatório de Arquitetura e Modelagem - EcoTerminal Escolar

## 1. Visão Geral da Arquitetura
O **EcoTerminal Escolar** utiliza celulares antigos nas salas de aula rodando em Modo Kiosk (aplicativo dedicado). Eles se conectam via Wi-Fi ao servidor da escola, que envia as notificações para a diretoria e coordenação.

```mermaid
graph TD
    N1["Terminal da Sala"] -->|Envia Alerta| N2["Servidor Central"]
    N2 -->|Notifica| N3["Painel da Diretoria"]
    N2 -->|Salva| N4["Banco de Dados"]
