# Projeto-Integrador-II
Repositório para a etapa 1
# Projeto EcoTerminal Escolar

> **Transformando smartphones obsoletos em centrais inteligentes de comunicação para salas de aula.**

---

## Sobre o Projeto

O **EcoTerminal Escolar** é uma solução de baixo custo e sustentável voltada para a gestão e comunicação interna em ambiente escolar. O projeto consiste no reaproveitamento de celulares antigos e baratos (desde que possuam tela touch funcional) para atuarem como terminais dedicados fixos em cada sala de aula.

Com a instalação de sistemas operacionais leves e otimizados, o dispositivo executa exclusivamente um aplicativo focado na comunicação ágil entre os professores em sala e os órgãos administrativos da escola (Diretoria, Coordenação, Secretaria e Suporte).

---

## A Justificativa e Impacto

1. **Sustentabilidade (Redução de Lixo Eletrônico):** Damos uma segunda vida a aparelhos descartados ou encostados, promovendo a economia circular na tecnologia.
2. **Baixo Custo de Implementação:** Dispensa a compra de computadores, tablets caros ou sistemas de interfonia tradicionais para as salas.
3. **Agilidade no Cotidiano:** Elimina a necessidade de enviar alunos para levar recados ou procurar professores pelo corredor, mantendo o foco no ensino.

---

## Como Funciona?
1. **Hardware:** Aparelhos antigos com tela sensível ao toque e suporte a Wi-Fi.
2. **Sistema Operacional:** Custom ROMs ou distribuições Linux leves ajustadas para o hardware específico.
3. **Modo Kiosk (Modo Dedicado):** O celular é configurado para abrir apenas o aplicativo do projeto, bloqueando acesso a redes sociais, jogos ou configurações do sistema.
4. **Alimentação:** Dispositivos mantidos conectados à tomada próxima à mesa do professor ou lousa.

---

## Principais Funcionalidades

- **Chamar Professor:** Alerta a coordenação para que o professor da próxima aula suba para a sala.
- **Chamados de Suporte:** Botões rápidos para solicitar limpeza, suporte técnico (projetor/Wi-Fi) ou atendimento médico/primeiros socorros.
- **Comunicação com a Diretoria:** Envio de alertas urgentes e recebimento de avisos gerais enviados pela administração.
- **Identificação Automática:** Cada terminal é pré-configurado com a identificação única da sala (ex: *1º Ano A*, *Laboratório de Ciências*).

---

## Tecnologias Envolvidas

- **Sistemas Operacionais Otimizados:** Android AOSP / LineageOS (versões leves) ou Linux embarcado.
- **Gerenciamento (Kiosk Mode):** Ferramentas de MDM (Mobile Device Management) ou scripts de inicialização automática.
- **Comunicação de Rede:** Protocolo HTTP/WebSockets sob rede Wi-Fi local.

---

## Próximos Passos do Desenvolvimento

- [x] Levantamento de Requisitos Funcionais e Não Funcionais
- [ ] Teste de sistemas operacionais leves em modelos específicos de celulares
- [ ] Desenvolvimento da interface gráfica do aplicativo (UI/UX)
- [ ] Criação do servidor local/painel administrativo para a diretoria
- [ ] Teste piloto em uma sala de aula
