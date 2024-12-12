# wisdom-reach

Wisdom Reach é um data lake concebido para rodar em um pequeno cluster k3s arm64, atuando como um ponto central de armazenamento e disponibilização de dados brutos provenientes de diversas fontes. Nesta etapa inicial, o foco está na ingestão de informações obtidas via bots do Telegram, abrangendo não apenas mensagens, mas qualquer dado acessível ao bot, independentemente de seu nível de estruturação.

A partir desse repositório, as pipelines ETL extraem conteúdo para o Data Warehouse Wisdom Core, compondo juntos uma arquitetura de Data LakeHouse. Essa combinação permite uma análise mais rica, integrada e escalável, oferecendo subsídios sólidos para a tomada de decisão.  
