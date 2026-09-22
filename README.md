# Análise de Incidente de Rede e Hardening de Segurança

## Sobre o Projeto
Este projeto documenta a análise de um incidente de segurança cibernética (ataque de Negação de Serviço - DoS) e o planeamento de resposta utilizando o framework **NIST CSF** (Identify, Protect, Detect, Respond, Recover). Adicionalmente, inclui uma avaliação de risco recomendando práticas de *Network Hardening* para mitigar vulnerabilidades estruturais.

O cenário baseia-se numa empresa de multimédia cujas operações foram paralisadas devido a um *ping flood* (pacotes ICMP) que explorou a ausência de regras rigorosas de firewall.

## Objetivos
- Analisar um incidente de rede e estruturar a resposta com base no **NIST Cybersecurity Framework**.
- Identificar falhas de configuração em ativos de rede (firewalls, gestão de credenciais).
- Propor controlos de segurança e métodos de deteção proativos (IDS/IPS, MFA, Monitorização de Logs).

## Documentação Técnica
- [Relatório de Análise de Incidente (NIST CSF)](https://github.com/shiedahacker/analise-incidente-redes/blob/main/An%C3%A1lise%20de%20relat%C3%B3rio%20de%20incidente.pdf)
- [Avaliação de Risco e Hardening de Rede](Relatório-de-avaliação-de-risco-de-segurança.pdf)

## Competências Demonstradas
- **Resposta a Incidentes:** Contenção, erradicação e planeamento de recuperação.
- **Segurança de Redes:** Regras de firewall, prevenção de *spoofing*, mitigação de DoS.
- **Ferramentas de Defesa:** Conceitos de IDS/IPS, SIEM e gestão de acessos.
- **Frameworks:** Aplicação prática das 5 funções do NIST CSF.

## Metodologia Aplicada (NIST CSF)
1. **Identify:** Mapeamento do impacto do ataque DoS nos serviços críticos da empresa.
2. **Protect:** Implementação de taxas limite (*rate limiting*) e bloqueio de IPs maliciosos.
3. **Detect:** Planeamento de monitorização de tráfego e alertas de anomalias (IDS).
4. **Respond:** Isolamento de sistemas não críticos e neutralização do tráfego ICMP externo.
5. **Recover:** Restabelecimento faseado dos serviços com as novas configurações ativas.
