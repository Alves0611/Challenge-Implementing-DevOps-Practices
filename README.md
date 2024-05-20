# **Desafio: Implementação de Práticas DevOps em um Ambiente Empresarial Fictício**

## Introdução

Nesse desafio, você irá simular a implementação de práticas DevOps num ambiente empresarial fictício. Utilizará os conceitos de CALMS e as Três Maneiras do DevOps para identificar oportunidades para aprimorar os processos existentes e propor soluções que cultivem uma cultura de colaboração, automação e aprendizado contínuo.


## Descrição da empresa

A **Tech** é uma empresa fictícia especializada em desenvolvimento de software, que oferece soluções inovadoras para clientes de diversos setores. Sua missão é simplificar a vida das pessoas através da tecnologia.

### Equipe:

- Desenvolvimento: 14 desenvolvedores com experiência em Java, C# e JavaScript. Apenas um profissional tem conhecimento em Delphi, a linguagem do sistema legado.
- Operações: A equipe de operações, composta por 4 profissionais, enfrenta desafios para manter a infraestrutura de TI e os sistemas em funcionamento eficiente, frequentemente lidando com problemas de escalabilidade e desempenho.

### Projetos em andamento

1. Sistema de Gestão de Vendas (LEGADO): Um aplicativo para gerenciamento de vendas que inclui controle de estoque, emissão de notas fiscais e relatórios de vendas.
2. Plataforma de E-commerce: uma plataforma de e-commerce escalável para clientes do setor varejista.

### Descrição dos processos atuais da empresa

1. **Entrega de Código:** Após a conclusão do desenvolvimento de um novo recurso, os desenvolvedores preparam um pacote de implantação e o encaminham à equipe de operações.
2. **Deploy:** O deploy é realizado manualmente no ambiente de produção, sem seguir um procedimento padronizado ou utilizar automação.
3. **Testes:** A equipe de operações conduz testes manuais no ambiente para verificar a funcionalidade e a integridade do código após o deploy em produção.
4. **Monitoramento:** Após o deploy, a equipe de operações monitora manualmente o sistema de logs do servidor, para identificar problemas ou falhas que possam surgir.

### Dados de desempenho:

- Tempo médio entre a entrega do código e o deploy: 2 dias.
- Taxa de sucesso dos deploys manuais: 80%.
- Número de incidentes após o deploy: média de 2 por semana.
- Tempo médio de recuperação (MTTR) de incidentes: 4 horas.

## Resultados Esperados

Ao final do desafio, terá elaborado um plano abrangente para implementar práticas DevOps num ambiente empresarial fictício. Este plano incluirá sugestões de automação, métricas de avaliação e estratégias para compartilhamento de conhecimento, refletindo uma compreensão prática dos conceitos teóricos apresentados neste módulo. Este desafio te preparará para aplicar esses princípios em ambientes de trabalho reais e cultivar uma cultura de colaboração e inovação.

## Etapas do Projeto

### 1. Diagnóstico Cultural (C de CALMS)

#### Processo Identificado:
O processo de **Deploy** foi identificado como o que mais pode se beneficiar da implementação de práticas DevOps. Atualmente, este processo é realizado manualmente pela equipe de operações, sem um procedimento padronizado ou automação.

#### Descrição do Processo Atual:
1. Entrega de Código: Desenvolvedores preparam um pacote de implantação e o encaminham à equipe de operações.
2. Deploy: Realizado manualmente no ambiente de produção.
3. Testes: Conduzidos manualmente pela equipe de operações no ambiente de produção.
4. Monitoramento: Feito manualmente pela equipe de operações, monitorando os logs do servidor.

#### Pontos de Atrito e Oportunidades de Melhoria:
- Falta de automação no deploy aumenta o tempo e a chance de erros.
- Dependência excessiva na equipe de operações para testes e deploy.
- Monitoramento manual é ineficiente e propenso a falhas.

### 2. Automação (A de CALMS)

#### Solução Proposta:
Implementação de um pipeline de CI/CD (Integração Contínua/Entrega Contínua) utilizando ferramentas como Jenkins, Github Actions, GitLab CI, ou CircleCI para automatizar o processo de build, test e deploy.

#### Plano de Implementação:
1. Configuração do repositório de código para integração com a ferramenta de CI/CD.
2. Criação de scripts automatizados para build e testes.
3. Configuração de ambientes de staging e produção para deploy automatizado.
4. Treinamento da equipe de desenvolvimento e operações sobre a utilização do pipeline automatizado.

### 3. Mensuração e Compartilhamento de Conhecimento (M e S de CALMS)

#### Métricas Relevantes:
- **Lead Time:** Tempo entre a submissão do código e o deploy em produção.
- **Taxa de Sucesso do Deploy:** Porcentagem de deploys bem-sucedidos.
- **MTTR (Mean Time to Recovery):** Tempo médio para recuperação após falhas.
- **Número de Incidentes:** Quantidade de incidentes pós-deploy.

#### Plano de Disseminação de Conhecimento:
1. Documentação detalhada do novo processo de CI/CD.
2. Workshops e sessões de treinamento regulares para as equipes de desenvolvimento e operações.
3. Relatórios periódicos sobre o desempenho das novas práticas, destacando melhorias e áreas de oportunidade.

### 4. Três Maneiras

#### Primeira Maneira (Acelerar o Fluxo):
- **Simplificação do Processo:** Implementação de um pipeline CI/CD para automatizar o build, test e deploy, reduzindo o tempo de entrega e aumentando a consistência.
- **Automação de Testes:** Integração de testes automatizados no pipeline para detectar problemas mais cedo no ciclo de desenvolvimento.

#### Segunda Maneira (Ampliar o Feedback):
- **Feedback Contínuo:** Utilização de ferramentas de monitoramento contínuo como Prometheus e Grafana para coletar dados de desempenho e saúde do sistema em tempo real.
- **Feedback Rápido:** Implementação de alertas automatizados para notificar a equipe sobre falhas e problemas de desempenho imediatamente após o deploy.

#### Terceira Maneira (Experimentar e Aprender):
- **Cultura de Experimentação:** Incentivo à experimentação segura através do uso de feature toggles e canary releases, permitindo testar novas funcionalidades em produção com menor risco.
- **Aprendizado Contínuo:** Realização de post-mortems e análises de retrospectiva para aprender com falhas e incidentes, promovendo uma mentalidade de melhoria contínua.


