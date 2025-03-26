<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Projeto de Software</a></h3>


<font size="+12"><center>
*&lt;Sistema Falcão Sombrio para Drones&gt;*
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

* Aluno/RA
* Aluno/RA


# Descrição do Projeto

*&lt;Introdução do projeto&gt;*

# Análise de Requisitos Funcionais e Não-Funcionais
*&lt;
Informações de requisitos e funcionalidades obtidas:
1. Central de Controle
- 1.1 Interface para gerenciamento de frotas de drones.
- 1.2 Controle remoto e autônomo dos drones.
- 1.3 Dashboard em tempo real com telemetria.

2. Sistema de Navegação Inteligente
- 2.1 Sensoriamento do ambiente via LIDAR, câmeras e GPS.
- 2.2 Detecção e evasão de ameaças em tempo real.
- 2.3 Operação autônoma baseada em redes neurais.

3. Gerenciamento de Comunicação
- 3.1 Protocolos para comunicação segura e em tempo real com os drones.
- 3.2 Mecanismos de fallback para evitar perda de conexão.

4. Banco de Dados e Auditoria
- 4.1 Logs de missões realizadas e eventos críticos.
- 4.2 Criptografia de ponta e assinaturas digitais.
- 4.3 Banco de dados NoSQL distribuído para dados em tempo real. 

5. Sistemas Embarcados e Segurança
- 5.1 Autenticação de operadores via biometria e autenticação
multifator.
- 5.2 Monitoramento de processos do SO embarcado para evitar falhas.

----------------------------------------------------------------------------------
FUNCIONAIS

RF-01 Autenticação - identificar o usuário com base em biometria e autenticação multifator

RF-02 Interface - possibilita o gerenciamento dos drones a partir de telemetria, status e permite executar comandos

RF-03 Controle de drones - permitir o controle das frotas de modo autônomo

RF-04 Redes neurais - o funcionamento autônomo dos drones é baseado em redes neurais

RF-05 Logs - Registra missões realizadas e seus dados

RF-06 Banco de dados - Garante que logs e possam ser armazenados e acessados em tempo real

RF-07 Comunicação- Troca de informações entre os drones e o sistema de controle

RF-08-Dashboard - garante a visualização em tempo real dos drones e seus acessórios

RF-09 Sensoriamento -  Permite acesso às câmeras e sensores do drones




NÃO FUNCIONAIS

RNF-01 Segurança - O sistema deve implementar criptografia AES-256 para armazenamento de dados, TLS para comunicação e IDS para detecção de ameaças.

RNF-02 Desempenho - A latência de comunicação entre drone e sistema não pode ultrapassar 50ms em condições normais.

RNF-03 Disponibilidade - O sistema deve estar disponível o tempo todo, com 99,9% de uptime, para garantir operação contínua em situações críticas.

RNF-04 Armazenamento - O banco de dados deve ser replicado geograficamente garantindo redundância e integridade dos dados.

RNF-05 Escalabilidade - A arquitetura deve permitir a adição de novos drones e servidores de maneira fácil e sem comprometer o desempenho e segurança.

RNF-06 Conformidade - O sistema deve atender padrões de segurança cibernética como ISO 27001 e NIST 800-53

RNF-07 Resiliência - O sistema deve identificar, investigar e corrigir ataques cibernéticos, recuperar a operação normal da organização, os sistemas de informação e processos em funcionamento rapidamente.

RNF-08 Tolerâncias a Falhas - A arquitetura deve suportar controladores duplos ativos com conexão heartbeat para proteção contra eventuais problemas de funcionamento.

RNF-09 Eficiência  - Os drones devem otimizar o consumo de bateria e rotas com o uso de algoritmos de IA para gestão de tempo e energia.

RNF-10 Log e Auditoria - Os logs devem ser protegidos e armazenados por no mínimo 06 anos para evitar alteração e exclusão.

   &gt;*

# Diagrama de Atividades

*&lt;Diagrama para visualizer as pessoas das áreas de negócios e de desenvolvimento de uma organização para entender o processo e comportamento.&gt;*

# Diagrama de Casos de Uso

*&lt;Diagrama para visualizar o comportamento dos atores&gt;*

# Descrição dos Casos de Uso

*&lt;Descrição do comportamento entre os atores/resquisitos&gt;*

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
