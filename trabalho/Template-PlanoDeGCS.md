<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão &lt;1.0&gt;
------------------

_[Observação: O template a seguir é fornecido para uso com o Rational Unified Process (RUP).  O texto exibido entre colchetes e em itálico foi incluído para orientar o autor e deve ser excluído antes da publicação do documento._

_Este documento utiliza a formatação da linguagem [Markdown] (http://daringfireball.net/projects/markdown/). Você pode encontrar um guia de referência rápido [aqui] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).]_

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|_&lt;dd/mm/aaaa&gt;_|_&lt;1.0&gt;_|_&lt;Versão inicial&gt;_|_&lt;autor&gt;_|
|_&lt;dd/mm/aaaa&gt;_|_&lt;1.1&gt;_|_&lt;Outra versão&gt;_  |_&lt;autor&gt;_|



1. Introdução
==============

_[A introdução do Plano de Gerenciamento de Configuração  oferece uma visão geral de todo o documento. 
Ela inclui a finalidade, o escopo, as definições, os acrônimos, as abreviações, as referências e uma visão geral deste
Plano de Gerenciamento de Configuração.]_

1.1 Finalidade
---------------
_[Especifique a finalidade deste Plano de Gerenciamento de Configuração.]_

1.2 Escopo
----------
_[Uma breve descrição do escopo deste Plano de Gerenciamento de Configuração; o modelo ao qual ele está associado e tudo o que é afetado ou influenciado por este documento.]_

1.3 Definições, Acrônimos e Abreviações
---------------------------------------
_[Esta subseção apresenta as definições de todos os termos, acrônimos e abreviações necessários para a correta interpretação do Plano de Gerenciamento de Configuração.  Essas informações podem ser fornecidas mediante referência ao Glossário do projeto.]_

1.4 Referências
---------------
_[Esta subseção apresenta uma lista completa de todos os documentos mencionados no Plano de Gerenciamento de Configuração. Identifique os documentos por título, número de relatório (se aplicável), data e organização responsável pela publicação. Especifique as fontes a partir das quais as referências podem ser obtidas. Essas informações podem ser fornecidas por um anexo ou outro documento.]_

1.5 Visão Geral
---------------
_[Esta subseção descreve o conteúdo restante do Plano de Gerenciamento de Configuração e explica como o documento está organizado.]_



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
_[Descreva os padrões e procedimentos que devem ser seguidos no projeto. Crie subseções se achar necessário, para organizá-los melhor.]_



5. Treinamento e Recursos
=========================
_[Descreva as ferramentas de software, o pessoal e o treinamento necessários para implementar as atividades de CM especificadas.]_



6. Auditorias de Configuração
=============================
_[Descreva o cronograma das auditorias de configuração e o que será verificado. Informe também como serão reportados os problemas encontrados e onde sera feito o acompanhamento dos itens corretivos.]_
