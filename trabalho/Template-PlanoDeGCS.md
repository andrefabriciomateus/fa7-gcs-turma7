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
|_&lt;dd/mm/aaaa&gt;_|_&lt;1.1&gt;_|_&lt;Outra versão&gt;_  |_&lt;autor&gt;_|



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
 
PGC Planos de Gerenciamento da Configuração

CCM Comissão de controle de Mudança

GC  Gerente de configuração

ICS	Item de Configuração de Software

PT	Plano de Teste




1.4 Referências
---------------
_[Esta subseção apresenta uma lista completa de todos os documentos mencionados no Plano de Gerenciamento de Configuração. Identifique os documentos por título, número de relatório (se aplicável), data e organização responsável pela publicação. Especifique as fontes a partir das quais as referências podem ser obtidas. Essas informações podem ser fornecidas por um anexo ou outro documento.]_

1.5 Visão Geral
---------------


      2 Gerenciamento de Configuração de Software
          
          Descreve os papeis , reponsabilidades, Ferramentas ,ambientes e infraestrutura necessarias para o projeto. 

      3 O Programa de Gerenciamento de Configuração
          
          Descreve como os artefatos do projeto devem ser nomeados , marcados e numerados, as baselines do projeto , os processos do controle de configuração e mudança.
        
      4 Padrões e Procedimentos
      
        Esta seção descreve os padrões e procedimentos que serão seguidos no processo.  
  
      5 Treinamento e Recursos
      
        Esta seção descreve as ferramentas , e os treinamento necessarios à implementar as atividades do Controle de Mudanças.
      
      6 Auditorias de Configuração
    
        Esta seção descreve o cronograma das auditorias de configuração e os itens que serão verificados.
2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------
_[Descreva quem será o responsável pela execução das diversas atividades de Gerenciamento de Configuração (CM) descritas no Processo de CM.]_

2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------
_[Descreva o ambiente de computação e as ferramentas de software a serem utilizadas para desempenhar as funções de CM em todo o ciclo de vida do projeto ou produto._
_Descreva as ferramentas e os procedimentos necessários utilizados para o controle de versão dos itens de configuração gerados no ciclo de vida do projeto ou produto._
_As questões envolvidas na configuração do ambiente de CM incluem:_
* _tamanho previsto dos dados do produto_
* _distribuição da equipe do produto_
* _localização física dos servidores e clientes]_
 


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
