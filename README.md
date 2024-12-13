# Wisdom Reach

**Wisdom Reach** é um repositório dedicado a agentes responsáveis pela coleta e envio de dados ao sistema de mensageria **Kafka**, integrando-se ao projeto **Wisdom Core**, uma plataforma de Data LakeHouse.

## 🚀 Funcionalidades

- **Coleta de Dados**: Captura dados de diversas fontes, incluindo APIs, serviços web e plataformas como o Telegram.
- **Publicação no Kafka**: Garante a ingestão confiável de dados para os tópicos configurados no Kafka.
- **Escalabilidade**: Projetado para operar em ambientes distribuídos, como clusters k3s arm64.
- **Extensibilidade**: Permite adicionar novos agentes ou fontes de dados de forma modular.

## 🛠️ Tecnologias Utilizadas

- **Python**: Linguagem base para o desenvolvimento dos agentes.
- **Apache Kafka**: Sistema de mensageria para transmissão de dados.
- **Docker**: Empacotamento e deploy dos agentes em contêineres.
- **k3s**: Orquestração em clusters leves.

## 📦 Estrutura do Repositório

```
wisdom-reach/
├── agents/             # Agentes de coleta de dados
│   ├── telegram/       # Agente para captura de dados do Telegram
│   ├── api_scraper/    # Agente para consumo de APIs externas
│   └── ...             # Outros agentes
├── configs/            # Configurações dos agentes e do Kafka
├── docker/             # Arquivos Docker para deploy
├── tests/              # Testes unitários e de integração
└── README.md           # Documentação do projeto
```

## 🌐 Pré-requisitos

1. **Docker** e **Docker Compose** instalados.
2. Um cluster **Kafka** em funcionamento.
3. (Opcional) Um cluster **k3s** para deploy em ambiente distribuído.

## 🛠️ Configuração

1. Clone o repositório:
   ```bash
   git clone https://github.com/santanaMd/wisdom-reach.git
   cd wisdom-reach
   ```

2. Configure os arquivos em `configs/` conforme sua infraestrutura.

3. Construa os contêineres:
   ```bash
   docker-compose build
   ```

4. Inicie os agentes:
   ```bash
   docker-compose up
   ```

## 🧪 Testes

Execute os testes unitários para garantir o funcionamento dos agentes:

```bash
pytest tests/
```

## 📖 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do repositório.
2. Crie uma branch para sua feature ou correção de bug:
   ```bash
   git checkout -b minha-feature
   ```
3. Commit suas alterações:
   ```bash
   git commit -m "Descrição da minha feature"
   ```
4. Envie as alterações:
   ```bash
   git push origin minha-feature
   ```
5. Abra um pull request.

## 📝 Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).

---

Para mais informações sobre o **Wisdom Core**, acesse [este repositório](https://github.com/santanaMd/wisdom-core).
