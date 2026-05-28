# Épico 4 - Ingestão de Dados

## Descrição

Importação automatizada de dados acadêmicos via web scraping (Lattes, Scholar, SIGAA etc.) e edição manual para complementar ou corrigir informações nos perfis.

## Requisitos vinculados

- **RF12**: O sistema deve importar dados acadêmicos de professores e alunos automaticamente a partir de fontes como Lattes, Google Scholar, IEEE e SIGAA.
- **RF13**: O sistema deve permitir que usuários revisem, complementem ou corrijam manualmente as informações importadas em seus perfis.
- **RF14**: O sistema deve indicar a origem dos dados exibidos no perfil (fonte importada ou edição manual).
- **RNF02**: O processo de web scraping deve ocorrer em segundo plano, sem impactar a experiência do usuário (Desempenho).

## Histórias de usuário

- **HU-04.01**: Sincronização automatizada de fontes externas (Scraping)
- **HU-04.02**: Conciliação e edição manual de dados importados
- **HU-04.03**: Rastreabilidade e sinalização de proveniência dos dados
