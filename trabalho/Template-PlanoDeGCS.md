<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão 5.0
------------------



Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|04/12/2013|1.0|Versão inicial|André Castro Alves
|05/12/2013|2.0|Alteração Seção 2|André Castro Alves
|06/12/2013|2.1|Finalizada Seção 2 |André Castro Alves
|06/12/2013|3.0|Adicionada Seção 3 |Fabrício Melo
|08/12/2013|3.1|Finalizada Seção 3 |Fabrício Melo
|08/12/2013|4.0|Adicionada e Finalizada Seção 4 |Fabrício Melo
|08/12/2013|5.0|Adicionada e Finalizada Seção 5 e 6 |Mateus Bastos


1. Introdução
==============


1.1 Finalidade
---------------

Este Plano de Gerenciamento da Configuração (PGC) tem como finalidade descrever todas as atividades do Gerenciamento de Controle de Configuração e Mudança que serão executadas durante o ciclo de vida do projeto. Neste projeto será dado enfâse nas partes relacionadas a identificação da configuração que inclui: selecionar os itens de configuração, determinar o tipo de documentação, determinar o controle e permissão de acesso, definir identificadores, documentar a configuração de release e estabelecer a configuração dos baselines

1.2 Escopo
----------
Este Plano de Gerenciamento de Configuração é destinado para todos os integrantes da Equipe do projeto CA - Controle de Auditoria e abrange todo o controle e gerenciamento da configuração do projeto.

1.3 Definições, Acrônimos e Abreviações
---------------------------------------

   Baseline é uma linha de referência composta por todos os itens de configuração
de um projeto. O objetivo de uma baseline é servir de referência para o gerenciamento de mudanças de um projeto. Ela deve ser como uma fotografia capaz de descrever um projeto em um determinado instante de sua execução.

   A criação de baselines pode ser realizada de acordo com os marcos do projeto ou de alguma outra forma definida pela gerência. A baseline é armazenada em um repositório de itens de configuração. E, a partir desse  momento, só pode ser alterado por meio de uma solicitação de alteração formal para controle de mudança.
   
   Uma release do sistema é uma versão fina distribuída ao cliente. Cada release deve incorporar novas funcionalidades ou ser planejado para uma plataforma diferente de hardware. Há, normalmente, muito mais versões de um sistema do que liberações. As versões são criadas no âmbito da organização, para  desenvolvimentos ou testes internos, e não são previstas para serem liberadas para os clientes.
   
   **Abreviações:**
   
|Sigla               |Descrição       |
|--------------------|-------------|
|PGC | Planos de Gerenciamento da Configuração|
|CCM | Comissão de controle de Mudança|
|GC | Gerente de configuração|
|ICS	| Item de Configuração de Software|
|PT	| Plano de Teste|
 
    


1.4 Referências
---------------


1.5 Visão Geral
---------------


|Seção               |Descrição       |
|--------------------|-------------|
|2 Gerenciamento de Configuração de Software | Descreve os papeis , reponsabilidades, Ferramentas ,ambientes e infraestrutura necessarias para o projeto.|
|3 O Programa de Gerenciamento de Configuração | Descreve como os artefatos do projeto devem ser nomeados , marcados e numerados, as baselines do projeto , os processos do controle de configuração e mudança.|
|4 Padrões e Procedimentos | Esta seção descreve os padrões e procedimentos que serão seguidos no processo.|
|5 Treinamento e Recursos	|  Esta seção descreve as ferramentas , e os treinamento necessarios à implementar as atividades do Controle de Mudanças.|
|6 Auditorias de Configuração	|  Esta seção descreve o cronograma das auditorias de configuração e os itens que serão verificados.|

     
2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------

|Responsavél                |Atividades       |
|--------------------|-------------|
|Gerente do Projeto | Identificar Atividades do Processo,Identificar Responsáveis ,Integrar Plano de CGS ,Identificar Itens de Configuração,Identificar Responsáveis ,Analisar Pedido de Alteração ,Verificar Item de Software Alterado,Relatar Situação,Auditoria da Configuração ,Criar Baseline ,Entregar Baseline.|
|Gerente de Configuração | Identificar Responsáveis,Identificar Responsáveis,Analisar Pedido de Alteração,Verificar Item de Software Alterado,Relatar Situação.|
| Equipe de Desenvolvimento | Solicitar Alteração,Implementar Alteração,Relatar Situação.|


2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------

2.2.1	Ferramentas a serem utilizadas para a gerência de configuração


|Ferramenta               |Descrição       |
|--------------------|-------------|
|GIT | Controle de versão - Repositorio : https://github.com/andrefabriciomateus/fa7-gcs-turma7 |
|Whats up | Ferramenta de comunicação -  Grupo FA7|


2.2.2	Configuração do software – Ferramentas do ambiente de desenvolvimento
 
 
|Ferramenta               |Tipo       |Versão               |  
|--------------------|-------------|------------------------|
|Sistema Operacional |Windows 7 Professional|SP1|
|Controle de Versão |GIT|Alterada Seção 2|
|Editor de Texto|MS Word |2010|
|Banco de Dados|Oracle|10G|
|Plataforma de Desenvolvimento|Ferramenta: Eclipse IDE for Java and DSL Developers|Juno|
|Relatórios|JasperReports|5.0.0|


2.2.3	Estrutura do Ambiente

|Ambiente              |Descrição       |Fluxo               |  
|--------------------|-------------|------------------------|
|Desenvolvimento |É o ambiente que servirá para o desenvolvimento do Sistema.|O componente atingirá a maturidade quando os requisitos forem supridos e testados pelos desenvolvedores através dos testes unitários.|
|Teste |É o ambiente que servirá para os testes de integração.|Alterada Quando a comunicação entre os módulos atinge o um estágio satisfatório de funcionamento, ou seja, não deverão existir erros de integração entre os subsistemas.|
|Banco de Dados|É o ambiente onde conterá o Banco de dados. |Ambiente que conterá o Banco de dados do sistema.|

2.2.4	Configuração das maquinas dos ambientes

|Ambiente              |Configuração Hardware       |Configuração Software              |  
|--------------------|-------------|------------------------|
|Desenvolvedor |Processador: 2.3 GHz Memória RAM: 2GB Hard Disk: 360 GB|Windows 7 Professional , Eclipse IDE / Java , MS Word.|
|Teste |Processador: 2.3 GHz Memória RAM: 2GB Hard Disk: 360 GB|Windows 7 Professional , Eclipse IDE / Java , MS Word.|
|Banco de Dados|Processador: 2.3 GHz Memória RAM: 6GB Hard Disk: 500 GB |Oracle 10G , Linux Redhat 5|



3. O Programa de Gerenciamento de Configuração
==============================================

3.1 Identificação da Configuração
---------------------------------
### 3.1.1 Métodos de Identificação
----------------------------------


Todos os itens de configuração, com exceção do código fonte, devem ser identificados baseados na nomeclatura descrita a seguir:

(PROJETO)(ID_ARTEFATO)(DATA)(VERSAO)

onde: 


| Nomenclatura | Descrição	     
|----------------------------------------------|-----------------------------|----------------------|
|Projeto|Nome do Projeto|
|ID_ARTEFATO |Código ou identificação do item de configuração|
|Data|É a data de criação do item de configuração, ou seja, é a data da primeira versão do item de configuração. O formato da data deve obedecer a regra: DDMMAAAA.

Deve ser adotado o padrão de que todas as letras tem que serem escritas em CAIXA ALTA.


As versões do sistema devem ser geradas com o seguinte padrão:

| Versões do sistema | Exemplo	     
|----------------------------------------------|-----------------------------|----------------------|
|Versão|x|
|Release |xx|
|Build|xxx|
|Exemplo |x.xx.xxx|




Os itens de configuração são descritos com suas respectivas siglas abaixo:

| Item de Configuração | Sigla	     
|----------------------------------------------|-----------------------------|----------------------|
|Diagrama de Caso de Uso|DCU|
|Documento de Arquitetura|ARQ|
|Diagrama de Classes |DC|
|Plano de Teste|PT|
|Cronograma |CT|


### 3.1.2 Itens de Configuração


| Item (ou Tipo de Item)                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|Diagrama de Caso de Uso|Analista de Requisitos|Após a aprovação do cliente|
|Documento de Arquitetura|Arquiteto de Software|Arquitetura seja definida e aceita por todos envolvidos diretamente|
|Plano de Teste| Analista de Teste|Documento deve ser revisado e cobrir 60% dos requisitos do projeto|
|Diagrama de Classe| Analista de Sistemas|Toda a estrutura das classes deve ser aprovada por todos os analistas e pelo arquiteto de software|
|Código Fonte|Líder Técnico e Programadores|Após todos os testes terem sidos realizados e o código for aprovado nestes testes|
|Cronograma|Gerente De Projetos|Projeto tenha atingido o objetivo final. Ou seja, ser entregue ao cliente e o mesmo esteja satisfeito com o que foi entregue|


### 3.1.3 Baselines do Projeto

À cada nova baseline, a identificação da mesma deverá seguir o seguinte padrão:


| Baseline| Sigla	     
|----------------------------------------------|-----------------------------|----------------------|
|Baseline de Documento/Planos|DOC_V (versão)|
|Baseline de Código Fonte|FONTE_V (versão)|
|Baseline de Releases|RELEASE_V (versão)|


As baselines devem ser criadas de acordo com a tabela a seguir:


| Baseline| Responsável na equipe	     | Itens |
|----------------------------------------|-----------------------------|----------------------|
|Requisitos| Analista de Requisitos|Diagrama de Casos de Uso|
|Planejamento|Gerente de Projetos, Analista de Sistema |Diagrama de Classe, Documento de Arquitetura|
|Desenvolvimento| Analista de Sistemas, Desenvolvedores|Código Fonte|
|Testes| Analista de Testes|Plano de Teste|
|Término do Projeto| Gerente de Projeto|Versão final (release) a ser entregue ao cliente|

O padrão de tags/label deve seguir o padrão:

[release_x]

Onde 'x' é um identificador para a mesma, um numeral.



### 3.1.4 Estrutura do Repositório de Versões

| Diretório| Arquivos	     
|----------------------------------------------|-----------------------------|----------------------|
|/Projeto/Documentação/branches|Diagrama de Caso de Uso, Documento de Arquitetura, Plano de Teste, Diagrama de Classe|
|/Projeto/Codigo_Fonte/branches|Código Fonte|
|/Projeto/tags|Entregas de Release|


3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança

![daigrama](http://www.freeimagehosting.net/newuploads/xra99.png "")

* Em análise: Solicitações de mudanças chegam e ficam aguradando serem analisadas.
* Analisado: Ao serem avaliadas as mudanças podem seguir dois caminhos: 
      - Recusada: Neste caso a mesma será arquivada e o fluxo se encerra.
      - Aprovada: Caso seja aprovada, a mudança será desenvolvida e ficará no estado: Em Desenvolvimento.
* Desenvolvido: Após serem realizadas as mudanças, tudo que foi modificado será testado.
* Realização de Testes: As mudanças realizadas passarão por uma série de testes, para que a integridade dos requisitos não seja afetada negativamente, haverão dois cenários:
     - Teste sem erro: Caso tudo ocorra como o esperado e as mudanças não afetem negativamente os requisitos, o cenário é encerrado com sucesso e a mudança é implantada.
     - Teste com erro: Neste caso, houveram erros causados pelas novas mudanças e então a mesma será novamente analisada. Caso seja visto que não é mais viável continuar com a modificação, a mesma passa a ser arquivada. Caso contrário a modificação parte mais uma vez para o desenvolvimento.



### 3.2.2 Comitê de Controle de Mudança (CCB)

| Membro| Responsabilidade	     
|----------------------------------------------|-----------------------------|----------------------|
|Gerente de Projetos|O gerente será o mediador da reunião, realiza anotações e viabiliza as decisões.O gerente repassa a todos os outros integrantes que não fazem parte do comitê o que fora decidido.|
|Analista de Testes|Irá avaliar se a mudança poderá ser incluída no plano de testes, de modo a não interferir de forma negativo os testes já planejados e realizados.|
|Analista de Sitemas|Será a pessoa que irá analisar a complexidade de codificação da mudança. |
|Analista de Requisitos|Irá avaliar cada mudança e decidirá se a mesma afetará de forma positiva ou negativa nos requisitos.|



4. Padrões e Procedimentos
==========================

### 4.1 Padrão de nomenclatura de código


Padrões de nomenclatura de código a serem utilizados ser os mesmos padrões de nomenclatura java.

|Tipo| Regra abordada	     |
|----------------------------------------|-----------------------------|----------------------|
|Classe e interfaces|Nomes de classes e interfaces devem ter a primeira letra maiúscula, quando o nome é formado por varias palavras, a primeira letra de cada palavra deve ser maiúscula, este formato é conhecido como camelCase. Para classes, os nomes devem normalmente ser substantivos e para Interfaces normalmente são utilizados adjetivos.|
|Métodos|Nos métodos, a primeira letra do nome deve ser minúscula e se for composta por outras palavras a forma camelCase deve ser utilizada também. Os nomes são formados geralmente por verbos e podem ser seguidos de substantivos.|
|Variáveis|Como nos métodos, a primeira letra deve ser minúscula e se for composta por mais de uma palavra, o formato camelCase deve ser utilizado. É recomendado que as variáveis tenham nomes curtos e significativos e que não seja utilizado nome com apenas um carácter exceto para variáveis temporárias.|


### 4.2 Padrão para criação de braches

Será necessária a criação de um branch para cada módulo do sistema. O mesmo deve seguir a seguinte nomenclatura:

[NOME_DO_MODULO], ou seja, cada branch receberá o nome do módulo a qual o branch será responsável.

Cada líder de projeto juntamente com o gerente devem realizar a criação do mesmo. E a cada integração de módulos será realizado o merge.

### 4.2 Procedimento de backup


Todos os repositórios e bancos de dados devem ser replicados. Onde ao termino de cada baseline ou ao término de cada semana, é realizado um backup de todas as informações para um servidor a parte. Desta forma os dados poderão ficar armazenados de forma segura.




5. Treinamento e Recursos
=========================

    Descrição dos treinamentos efetuados para os integrantes da TeamUp.

    Treinamento: Repositório
    Objetivo: Repositório	Treinamento ensina como acessar o repositório através de uma máquina cliente, como dar os comandos principais do repositório,  como incluir novos itens dentro do repositório e também como remover do mesmo.	Gerente
    Público Alvo: - Analista de Sistemas;
                  - DBA;
                  - Desenvolvedor.

    Treinamento: Ferramentas	
    Objetivo: Treinamento será mostrado os padrões da empresa e como é utilizada as seguintes ferramentas :Visual Basic.NET, desenvolvimento em camadas, Sql Server, criação de relatórios através do Crystal Reports 10.	Analista de Sistemas
    Público Alvo: - DBA;
                  - Desenvolvedor.

    Treinamento: Processo de GC
	Objetivo: Treinamento consiste em seguir os padrões de nomeclatura dos artefatos, as regras de inserção/alteração de baselines.. Processo para geração de releases e builds. Apresentação dos processos de Gerência de Mudança.	Gerente de Projeto
     Público Alvo: - Gerente de Configuração;
                   - Analista de Sistemas;
                   - Desenvolvedor.


6. Auditorias de Configuração
=============================
	
	As auditorias de configuração devem ser realizadas a cada entrega a fim de garantir que o processo de configuração estão sendo aplicados corretamente.
	Auditorias de acompanhamento de projeto devem ser realizadas quando as seguintes atividades forem finalizadas:
	
	- Compreender o programa;
    - Projetar as mudanças da feature 1;
    - Implementação da feature 1;
    - Testes de debug da feature 1;
    - Projetar as mudanças da feature 2;
    - Implementação da feature 2;
    - Testes de debug da feature 2;
    - Projetar as mudanças da refatoração;
    - Implementação da refatoração;
    - Testes de debug da refatoração.

    Além disso, sempre que for necessário verificar como anda a taxa de defeitos detectados no teste a auditoria deve ser realizada.
