# Requisitos Não Funcionais
- **RNF01**: A interface deve ser responsiva e funcionar adequadamente em dispositivos móveis e desktops (Usabilidade)
- **RNF02**: O processo de web scraping deve ocorrer em segundo plano, sem impactar a experiência do usuário (Desempenho)
- **RNF03**: O acesso à plataforma deve ser restrito a usuários com conta institucional válida (Segurança)
- **RNF04**: Os dados importados devem ter sua origem identificada e o usuário pode revisar ou corrigir qualquer informação importada (Integridade dos dados)
- **RNF05**: O sistema deve mitigar conflitos de concorrência entre a edição manual (feita por professores ou administradores) e a rotina de web scraping em background utilizando controle de concorrência otimista (Optimistic Locking), descartando a sobrescrita automática de dados brutos caso o estado do perfil tenha sido alterado manualmente durante o processamento.
- **RNF06**: O sistema deve obrigatoriamente restringir a busca e a ingestão de dados de fontes externas (Lattes, Google Scholar, IEEE, SIGAA) através de identificadores únicos estritos pré-cadastrados (como ID Lattes ou ID SIGAA), proibindo consultas baseadas puramente na string de nome do docente para mitigar o risco de homônimos.
