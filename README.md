# Linka

## Problema
Atualmente no Departamento de Computação da Unb existem diversos grupos e linhas de pesquisa, monitorias ou tutoriais que podem contribuir para formação de novos talentos na área. Contudo, como as informações estão espalhadas por canais diversos, ou ainda não recebem a devida divulgação, muitas vezes se torna difícil de realizar a ligação entre alunos interessados e professores com oportunidades disponíveis. 

## Escopo
O linka tem como público alvo alunos e professores vinculados ao Departamento de Computação da Unb e departamentos afins como a Faculdade de Tecnologia, podendo ser escalável para a comunidade acadêmica da UnB.
Através de técnicas de webscrapping em fontes confiáveis como Plataforma Lattes, Google Scholar, IEEE, SIGAA Público, entre outros, a aplicação busca otimizar a divulgação de oportunidades acadêmicas de pesquisa, também deixando disponível opções de edição manual para professores e alunos em seus respectivos perfis.

## Stakeholders
- Alunos
- Professores
- Servidores do departamento

## Requisitos
### Requisitos Funcionais
- O sistema deve permitir que alunos criem e editem seu perfil com informações acadêmicas (como titulação), habilidades e áreas de interesse
- O sistema deve permitir que professores criem e editem seu perfil com informações acadêmicas e linhas de pesquisa
- O sistema deve permitir que servidores do departamento realizem edições em informações gerais relacionados ao respectivo departamento (como vagas e oportunidades)
- O sistema deve permitir a criação e edição de perfis de grupos de pesquisa vinculados a um ou mais professores
- O sistema deve exibir as oportunidades vinculadas ao perfil do professor ou grupo de pesquisa

- O sistema deve permitir login exclusivamente via conta institucional Office 365
- O sistema deve restringir o acesso a usuários autenticados com vínculo à UnB
- O sistema deve diferenciar os papéis de aluno e professor após a autenticação, liberando as funcionalidades correspondentes a cada perfil

- O sistema deve permitir busca de oportunidades e grupos de pesquisa por tema ou área do conhecimento
- O sistema deve permitir que professores busquem alunos filtrando por habilidades e interesses
- O sistema deve exibir resultados de busca com informações resumidas do perfil ou oportunidade encontrada

- O sistema deve importar dados acadêmicos de professores e alunos automaticamente a partir de fontes como Lattes, Google Scholar, IEEE e SIGAA
- O sistema deve permitir que usuários revisem, complementem ou corrijam manualmente as informações importadas em seus perfis
- O sistema deve indicar a origem dos dados exibidos no perfil (fonte importada ou edição manual)

- O sistema deve permitir que professores (ou servidores do departamento) publiquem, editem e encerrem vagas de pesquisa ou monitoria
- O sistema deve permitir que alunos demonstrem interesse em uma vaga ou grupo de pesquisa
- O sistema deve notificar o professor quando um aluno demonstrar interesse em sua vaga
- O sistema deve notificar o aluno quando uma nova oportunidade compatível com seus interesses for publicada

### Requisitos Não Funcionais
- A interface deve ser responsiva e funcionar adequadamente em dispositivos móveis e desktops (Usabilidade)
- O processo de web scraping deve ocorrer em segundo plano, sem impactar a experiência do usuário (Desempenho)
- O acesso à plataforma deve ser restrito a usuários com conta institucional válida (Segurança)

## Épicos
1. Perfis
Criação e edição das páginas de perfil de alunos, professores e grupos de pesquisa
3. Autenticação
Integração com login via conta institucional Office 365
4. Busca e Descoberta
Mecanismos de pesquisa e filtragem para que alunos encontrem oportunidades por tema e professores encontrem alunos por habilidade ou interesse
5. Ingestão de Dados
Importação automatizada de dados acadêmicos via web scraping (Lattes, Scholar, SIGAA etc.) e edição manual para complementar ou corrigir informações nos perfis
6. Oportunidades e Interações (sistema de notificações)
Fluxo de publicação de vagas por professores, demonstração de interesse por alunos e notificações básicas entre as partes

## Equipe
- 211010350	Célio Júnio de Freitas Eduardo
- 232002539	Guilherme Delmonte Pereira de Souza Rios
- 242037322	Izadora Netz Sieczkowski
- 241039681	Luisa Ramos Barros
- 231037020 Suzana Miranda

## Histórico de Atualizações
