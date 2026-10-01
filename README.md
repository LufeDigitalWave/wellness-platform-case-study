# Plataforma de hábitos e bem-estar

Case técnico anonimizado sobre registro de hábitos, alimentação e atividades, com interfaces web e móvel.

> Publicação documental. Não inclui aplicação executável, dados de usuários, regras clínicas ou integrações ativas. Os fluxos são abstrações para discussão técnica e não fornecem orientação médica.

## Problema

Registros pessoais chegam por interfaces diferentes e precisam formar um histórico coerente. A modelagem deve distinguir o que a pessoa informou, como o dado foi interpretado e o que foi apresentado na interface, sem transformar sugestões em fatos.

## Escopo representado

Interfaces para acompanhamento de hábitos, módulos de alimentação e exercício, persistência e tratamento de consentimento. O foco é a organização do domínio e a fronteira entre experiência do usuário e informações sensíveis.

A presença de módulos de consentimento não comprova que todas as regras de privacidade estejam corretamente aplicadas; essa verificação está fora do escopo documental.

## Stack identificada

Python, FastAPI, Pydantic, SQLAlchemy, Alembic e Redis; React, TypeScript e Vite; componentes móveis com React Native e Expo. A stack foi identificada em manifests e estrutura, não validada em produção nesta publicação.

## O que discutir numa entrevista

- Como representar registros incompletos sem inventar informação.
- Como conciliar alterações feitas em interfaces diferentes.
- Onde separar validação de entrada, agregação e apresentação.
- Como tratar consentimento, acesso e exclusão de registros pessoais.

Consulte a [arquitetura e o roteiro de validação](ARCHITECTURE.md).

## Limites

Não são publicados registros pessoais, imagens, dados de saúde, recomendações, parâmetros internos, marcas ou resultados clínicos. Não há alegação de eficácia, certificação ou conformidade regulatória.
