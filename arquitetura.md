# Relatório de Arquitetura e Modelagem - EcoTerminal Escolar

## 1. Visão Geral da Arquitetura
O **EcoTerminal Escolar** utiliza celulares antigos nas salas de aula rodando em Modo Kiosk (aplicativo dedicado). Eles se conectam via Wi-Fi ao servidor da escola, que envia as notificações para a diretoria e coordenação.

```mermaid
graph TD
    N1["Terminal da Sala"] -->|Envia Alerta| N2["Servidor Central"]
    N2 -->|Notifica| N3["Painel da Diretoria"]
    N2 -->|Salva| N4["Banco de Dados"]
```
---
##2 2. Diagrama de Fluxo do Usuário
```mermaid
flowchart TD
    N1["Inicio"] --> N2["Abrir App no Terminal"]
    N2 --> N3["Exibir Tela Principal"]
    N3 --> N4{"Escolha da Ação"}
    
    N4 -->|Chamar Professor| N5["Pedir Troca de Aula"]
    N4 -->|Suporte| N6["Pedir Limpeza ou TI"]
    N4 -->|Emergência| N7["Pedir Primeiros Socorros"]
    
    N5 --> N8["Enviar para o Servidor"]
    N6 --> N8
    N7 --> N8
    
    N8 --> N9["Notificar Diretoria"]
    N9 --> N3
```
---
## 3. Estrutura de Dados
```json
[
  {
    "id": 101,
    "sala": "1º Ano A",
    "tipo": "Suporte TI",
    "descricao": "Projetor desligado",
    "status": "Pendente"
  }
]
