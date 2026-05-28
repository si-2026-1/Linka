# Épico 4 - Ingestão de Dados

## Descrição

Rotinas automatizadas de gerenciamento e importação de dados acadêmicos de docentes via web scraping, com permissões de ajuste manual restritas à equipe de manutenção, servidores e aos próprios professores.

## Requisitos vinculados

- **RF12**: O sistema deve importar dados acadêmicos de professores automaticamente a partir de fontes como Lattes, Google Scholar, IEEE e SIGAA.
- **RF13**: O sistema deve permitir que professores, servidores do departamento e administradores revisem, complementem ou corrijam manualmente as informações importadas nos perfis dos docentes.
- **RF14**: O sistema deve indicar a origem dos dados exibidos no perfil (fonte importada ou edição manual).
- **RNF02**: O processo de web scraping deve ocorrer em segundo plano, sem impactar a experiência do usuário (Desempenho).
- **RNF04** O sistema deve mitigar conflitos de concorrência entre a edição manual (feita por professores ou administradores) e a rotina de web scraping em background utilizando controle de concorrência otimista (Optimistic Locking), descartando a sobrescrita automática de dados brutos caso o estado do perfil tenha sido alterado manualmente durante o processamento.
- **RNF05** O sistema deve obrigatoriamente restringir a busca e a ingestão de dados de fontes externas (Lattes, Google Scholar, IEEE, SIGAA) através de identificadores únicos estritos pré-cadastrados (como ID Lattes ou ID SIGAA), proibindo consultas baseadas puramente na string de nome do docente para mitigar o risco de homônimos.

## Histórias de usuário

- **HU-04.01**: Execução e Orquestração da Rotina de Scraping (Backend/Manutenção)
- **HU-04.02**: Interface de Conciliação e Edição Multipapel (Professor/Servidor/Admin)
- **HU-04.03**: Rastreabilidade e Sinalização de Proveniência dos Dados (Camada de Apresentação)
