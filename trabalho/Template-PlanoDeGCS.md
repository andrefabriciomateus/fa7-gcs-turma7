<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão 1.0
------------------



Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|04/12/2013|1.0|Versão inicial|André Castro Alves
|05/12/2013|2.0|Alteração Seção 2|André Castro Alves
|06/12/2013|2.1|Finalizada Seção 2 |André Castro Alves


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
_[Esta subseção apresenta uma lista completa de todos os documentos mencionados no Plano de Gerenciamento de Configuração. Identifique os documentos por título, número de relatório (se aplicável), data e organização responsável pela publicação. Especifique as fontes a partir das quais as referências podem ser obtidas. Essas informações podem ser fornecidas por um anexo ou outro documento.]_

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
_[Descreva como os artefatos do projeto ou produto devem ser nomeados, marcados e numerados. O esquema de identificação deve abranger o hardware, o software do sistema, os produtos de terceiros (COTS) e todos os artefatos de desenvolvimento de aplicativos listados na estrutura de diretórios do produto; por exemplo, planos, modelos, componentes, software de teste, resultados e dados, executáveis e assim por diante.]_

### 3.1.2 Itens de Configuração
_[Relacionar os artefatos ou grupos de artefatos, separando por tipo, modulo ou subsistema, responsável ou momento em que deverão ser incluídos em baselines._
* _“Inclusão em Baseline” em branco significa que o grupo de artefatos não participará de baseline. Pode ser expresso como uma data ou identificador de uma baseline, fase ou ponto de controle_
* _“Responsável”: indicar nominalmente, sempre que possível]_

| Item (ou Tipo de Item)                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|_&lt;grupo de itens de configuração&gt;_|_&lt;nome do responsável&gt;_|_&lt;momento a partir do qual o conjunto de artefatos será incluído em baseline&gt;_|


### 3.1.3 Baselines do Projeto



### 3.1.4 Estrutura do Repositório de Versões
_[Descreva a organização de diretórios do seu repositório e que itens/arquivos devem ser armazenados em cada diretório.]_

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança
_[Descreva o processo pelo qual os problemas e as mudanças são submetidos, revisados e dispostos. Inclua como funciona a transição de estados de uma solicitação de mudança]_

### 3.2.2 Comitê de Controle de Mudança (CCB)
_[Descreva a participação e os procedimentos para processar solicitações e aprovações de mudança a serem seguidos pelo CCB. Informe quem são os membros do CCB e suas responsabilidades.]_



4. Padrões e Procedimentos
==========================
_[Descreva os padrões e procedimentos que devem ser seguidos no projeto. Crie subseções se achar necessário, para organizá-los melhor.]_



5. Treinamento e Recursos
=========================
_[Descreva as ferramentas de software, o pessoal e o treinamento necessários para implementar as atividades de CM especificadas.]_



6. Auditorias de Configuração
=============================
_[Descreva o cronograma das auditorias de configuração e o que será verificado. Informe também como serão reportados os problemas encontrados e onde sera feito o acompanhamento dos itens corretivos.]_
