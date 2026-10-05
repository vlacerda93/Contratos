# API DevOps - Infraestrutura e Implantação

Este repositório contém a infraestrutura containerizada, monitorização e documentação para a API do projeto, desenvolvida como atividade prática da disciplina de Engenharia DevOps.



A arquitetura foi projetada focando nos pilares de escalabilidade, segurança, confiabilidade e reprodutibilidade, aplicando as melhores práticas de DevOps:

Containerização (Docker & Docker Compose): A aplicação foi isolada em um contêiner Docker para garantir paridade entre os ambientes de desenvolvimento e produção. O Docker Compose gerencia a orquestração local dos serviços (API e Prometheus), garantindo subida consistente com um único comando.

Monitorização e Observabilidade (Prometheus): A inclusão do Prometheus permite a recolha de métricas em tempo real (/metrics) para monitorizar a saúde, latência e consumo de recursos da aplicação, garantindo alta visibilidade e confiabilidade operacional.

Automação de Testes (Jest): Integração de suites de testes para validação contínua da qualidade do código antes e durante a implantação.

Padronização e Segurança: Separação rígida de variáveis de ambiente via .env.example para evitar exposição de credenciais e segredos no controlo de versão.

🛠️ Pré-requisitos
Para executar este projeto localmente, precisarás de ter instalado na tua máquina:

Git

Docker e Docker Compose

Node.js (opcional, apenas para execução sem Docker)