<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Projeto de Software</a></h3>


<font size="+12"><center>
Sistema Falcão Sombrio para Drones
</center></font>

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do Projeto](#introdução-do-projeto)
- [Análise de Requisitos Funcionais e Não-Fucionais](#descrição-dos-requisitos)
- [Diagrama de Atividades](#diagrama-de-atividades) 
- [Diagrama de Casos de Uso](#diagrama-de-comportamento-atores)
- [Descrição dos Casos de Uso](#descrição-das-funcões)
- [Diagrama de Senquencia](#diagrama-de-ordem-interações)
- [Diagrama de Classes](#diagrama-orientado-objetos)
- [Diagrama de Estados](#diagrama-estrutura-componente)
- [Diagrama de Implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Vitor Neudl Gandolfi / 10408845
* Hailo Rodrigues da Silva Neto / 10416839


# Descrição do Projeto

*&lt;Introdução do projeto&gt;*

# Análise de Requisitos Funcionais e Não-Funcionais

FUNCIONAIS

| Identificação |      Nome     | Descrição   |
| ------------- | ------------- | -------------
| RF-01         | Autenticação       |Identificar o usuário com base em biometria e autenticação multifator.                            |
| RF-02         | Interface          |Possibilita o gerenciamento dos drones a partir de telemetria, status e permite executar comandos.|
| RF-03         | Controle de drones |Permitir o controle das frotas de modo autônomo.                                                  |
| RF-04         | Redes neurais      |O funcionamento autônomo dos drones é baseado em redes neurais.                                   |
| RF-05         | Logs               |Registra missões realizadas e seus dados.                                                         |
| RF-06         | Banco de dados     |Garante que logs e possam ser armazenados e acessados em tempo real.                              |
| RF-07         | Comunicação        |Troca de informações entre os drones e o sistema de controle.                                     |
| RF-08         | Dashboard          |Garante a visualização em tempo real dos drones e seus acessórios.                                |
| RF-09         | Sensoriamento      |Permite acesso às câmeras e sensores do drones.                                                   |


--------------------------------------------------------------------------------------------------------------------------------------------

NÃO FUNCIONAIS

| Identificação |      Nome     | Descrição   |
| ------------- | ------------- | -------------
| RNF-01         | Segurança        |O sistema deve implementar criptografia AES-256 para armazenamento de dados, TLS para comunicação e IDS para detecção de ameaças|
| RNF-02         | Desempenho       |A latência de comunicação entre drone e sistema não pode ultrapassar 50ms em condições normais.|
| RNF-03         | Disponibilidade  | O sistema deve estar disponível o tempo todo, com 99,9% de uptime, para garantir operação contínua em situações críticas.|
| RNF-04         | Armazenamento    |O banco de dados deve ser replicado geograficamente garantindo redundância e integridade dos dados.|
| RNF-05         |Escalabilidade    |A arquitetura deve permitir a adição de novos drones e servidores de maneira fácil e sem comprometer o desempenho e segurança.|
| RNF-06         | Conformidade     |O sistema deve atender padrões de segurança cibernética como ISO 27001 e NIST 800-53|
| RNF-07         | Resiliência      |O sistema deve identificar, investigar e corrigir ataques cibernéticos, recuperar a operação normal da organização, os sistemas de informação e processos em funcionamento rapidamente.|
| RNF-08         | Tolerâncias a Falhas |A arquitetura deve suportar controladores duplos ativos com conexão heartbeat para proteção contra eventuais problemas de funcionamento.|
| RNF-09         | Eficiência            |Os drones devem otimizar o consumo de bateria e rotas com o uso de algoritmos de IA para gestão de tempo e energia.|
| RNF-10         | Log e Auditoria      |Os logs devem ser protegidos e armazenados por no mínimo 06 anos para evitar alteração e exclusão.|


# Diagrama de Atividades

*&lt;Diagrama para visualizer as pessoas das áreas de negócios e de desenvolvimento de uma organização para entender o processo e comportamento.&gt;*

# Diagrama de Casos de Uso

*&lt;Diagrama para visualizar o comportamento dos atores&gt;*

# Descrição dos Casos de Uso
|||
| ------------- | ------------- | 
|Nome do caso de uso| Controle manual de drones       |
|Ator principal     | Operador militar|
|Atores secundários| Central de controle       |
|Resumo| Este caso de uso descreve o protocolo de controle de um drone manualmente por um operador militar       |
|Pré-condições| O operador deve estar autenticado no sistema       |
|Pós-condições| A missão é realizada e um log é gerado       |
|Restrições e validações| 1.Devem existir drones disponíveis para operação 2.Necessita uma comunicação segura       |
| ------------- | ------------- | 
|Nome do caso de uso| Login      |
|Ator principal     | Operador militar|
|Atores secundários| Central de controle       |
|Resumo| Este caso de uso descreve o procedimento de login e verificação do usuário       |
|Pré-condições| O operador deve possuir um registro no banco de dados      |
|Pós-condições| O operador ganha acesso ao sistema      |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso| Gerenciar Frotas de Drones      |
|Ator principal     | Operador militar |
|Atores secundários| Central de controle      |
|Resumo| Permite cadastrar, editar, visualizar e remover drones da frota disponível no sistema. Também inclui informações como modelo, status, localização e capacidade.     |
|Pré-condições| Usuário autenticado com permissão de gestão      |
|Pós-condições| Frota atualizada no sistema.   |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso| Configurar Missão Autônoma  |
|Ator principal     | Operador militar |
|Atores secundários| Central de controle      |
|Resumo| Define rotas, pontos de interesse e objetivos para que o drone execute de forma automática sem intervenção humana durante o voo.     |
|Pré-condições| Drone disponível, plano de voo válido      |
|Pós-condições| Missão salva e pronta para execução.   |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso| Exibir Dashboard em Tempo Real     |
|Ator principal     | Operador militar |
|Atores secundários| -----------------------      |
|Resumo| Apresenta uma interface com dados atualizados em tempo real sobre drones em operação, incluindo telemetria, localização, status de bateria, vídeo ao vivo e alertas.     |
|Pré-condições| Drones ativos e conectados      |
|Pós-condições| Dashboard atualizado continuamente.   |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso|  Finalizar Sessão     |
|Ator principal     | Usuário/Operador militar |
|Atores secundários| -----------------------      |
|Resumo| Encerra a sessão atual do usuário e revoga o acesso ao sistema.     |
|Pré-condições| Sessão iniciada      |
|Pós-condições|  Sessão encerrada com segurança.   |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso| Registrar Log das Missões    |
|Ator principal     | Sistema |
|Atores secundários| -----------------------      |
|Resumo| Armazena automaticamente todas as informações da missão realizada, incluindo horário, rota, eventos ocorridos, operadores envolvidos e status final.     |
|Pré-condições| Ddos disponíveis da missão concluída ou cancelada      |
|Pós-condições| Log salvo no banco de dados.   |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso|  Transmitir Dados em Tempo Real    |
|Ator principal     | ----------------------- |
|Atores secundários| -----------------------      |
|Resumo| Envia informações de telemetria, vídeo e status do drone durante o voo para o sistema central.     |
|Pré-condições| Drone em missão com conexão estável      |
|Pós-condições| Dados disponíveis para o dashboard e registros.   |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso|  Criptografar Dados     |
|Ator principal     | Sistema |
|Atores secundários| -----------------------      |
|Resumo| Garante a segurança da comunicação e dos dados armazenados utilizando algoritmos de criptografia.     |
|Pré-condições| Dados em trânsito ou sendo armazenados      |
|Pós-condições| Dados protegidos contra acessos não autorizados.   |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso| Gerenciar Usuários     |
|Ator principal     | Administrador/central de controle |
|Atores secundários| -----------------------      |
|Resumo|  Permite o cadastro, edição, exclusão e atribuição de permissões a usuários do sistema.     |
|Pré-condições|  Sessão de administrador ativa      |
|Pós-condições| Lista de usuários atualizada.   |
|Restrições e validações| -----------------------      |
| ------------- | ------------- | 
|Nome do caso de uso| Histórico de Voos      |
|Ator principal     | ----------------------- |
|Atores secundários| -----------------------      |
|Resumo| Exibe ao usuário uma lista de todas as missões realizadas, com detalhes como data, duração, trajeto, operador e status.     |
|Pré-condições| Missões registradas      |
|Pós-condições| Histórico acessível para análise.   |
|Restrições e validações| -----------------------      |

# Diagrama de Sequência

*&lt;Diagrama de ordem e interação dos objetos&gt;*

# Diagrama de Classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Estados

*&lt;Diagrama para permite modelar o comportamento interno de um determinado objeto, subsistema ou sistema global&gt;*

# Diagrama de Implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
