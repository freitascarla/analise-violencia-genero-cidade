#### <center> Projeto Final - {reprograma} </center>


# <center> **Violência contra mulheres nas cidades brasileiras** </center>


- [Contexto e Objetivos](#-Objetivo)
- [Coleta de Dados](#-Coleta-de-Dados)
- [Arquitetura do Projeto](#-Arquitetura-do-Projeto)
- [Tecnologias e Dependências Utilizadas](#-Tecnologias-e-Dependências-Utilizadas)
- [Visualização](#-Visualização)
- [Interface Gráfica](#-Interface-Gráfica)
- [Conclusões e Recomendações](#-Conlusões-e-Recomendações)


## Contexto e Objetivos

A violência urbana é uma realidade compartilhada por todos os brasileiros. Mas será que homens e mulheres enfrentam os mesmos desafios ao lidar com essa violência no espaço público? O medo que assombra as mulheres ao sair de casa é semelhante ao medo experimentado pelos homens?

Este estudo tem como propósito analisar a influência do gênero na vivência da violência urbana e compreender se as experiências de homens e mulheres diante da violência nos espaços urbanos são equiparáveis.

O foco central é analisar as ocorrências de violência por gênero entre os anos de 2010 a 2020 nos espaços públicos das cidades brasileiras. Nesse contexto, buscando identificar os tipos de violência mais prevalentes, mapear os locais de maior incidência e compreender os perfis dos principais agressores.


## Coleta de Dados

Os dados foram extraídos do Sistema de Informação de Agravos de Notificação (SINAN) através do [DATASUS](https://datasus.saude.gov.br/transferencia-de-arquivos/).

Foi utilizado o banco de dados "VIOL - Violência doméstica, sexual e/ou outras violências" oriundo do [Sistema de Vigilância de Violências e Acidentes (Viva)](http://www.portalsinan.saude.gov.br/violencia-interpessoal-autoprovocada). 

Esses conjuntos de dados estão disponíveis no formato DBC e foram processados utilizando o programa TabWin para filtragem e visualização.

Para mais informações sobre as bases de dados acesse o [_notebook_](https://github.com/freitascarla/analise-violencia-genero-cidade/blob/main/analise-exploratoria/analise_exploratoria.ipynb) da análise exploratória.


## Arquitetura do Projeto

```

 📁analise-violencia-genero-cidade
   |
   |--📁 analise-exploratoria
   |  |    |- 📄 analise-exploratoria.ipynb
   |
   |--📁 dataset
   |  |    |- 📄 base_final_sinan.rar
   |  |    |- 📄 dados_violencia_local_ocorrencia_sinan_2010_2020.rar
   |  |    |- 📄 estrutura_base_dados.txt
   |  |
   |--📁 visualizacoes
   |  |    |- 📄 dashboard_tableau.pdf
   |  |    |- 📄 slide_apresentacao.pdf
   |  |
   |- 📄 readme.md
   
```


## Tecnologias e Dependências Utilizadas

| Ferramenta | Descrição |
| --- | --- |
| `python` | Linguagem de programação. |
| `pandas`    | Biblioteca criada para a linguagem Python para manipulação e análise de dados.|
| `numpy`    | Biblioteca para a linguagem Python, que suporta o processamento de grandes, multi-dimensionais arranjos e matrizes. |
| `matplotlib`   | Biblioteca de software para criação de gráficos e visualizações de dados em geral, feita para e da linguagem de programação Python.|
| `seaborn`    | Ferramenta para plotagem dos mais variados tipos de gráficos em Python.|
| `jupyter notebook`| Aplicação web criada para desenvolver software de código aberto, padrões abertos e serviços para computação interativa em dezenas de linguagens de programação.|
| `Tableau`    | Plataforma de análise, exploração e gerenciamento de dados visuais.|


## Visualização

```ps
# Clonar o repositório
$ git clone https://github.com/freitascarla/analise-violencia-genero-cidade.git

# Entrar na pasta do repositório
$ cd analise_violencia_genero_cidade

# Instalar as bibliotecas
$ import pandas as pd
$ import numpy as np
$ import matplotlib.pyplot as plt
$ import seaborn as sns

# Executar o comando na parte superior do arquivo .ipynb para que você possa rodar o projeto localmente no arquivo 'analise-exploratoria.ipynb'.
$ Run ou Run All
```

## Interface Gráfica

Este projeto está com visualizações públicas no Tableau. Você pode acessar no link [Tableau](https://public.tableau.com/views/Livro1_17019033104050/Painel1?:language=pt-BR&:display_count=n&:origin=viz_share_link).


## Conclusões e Recomendações

O resultado desta análise constata que cerca de 62% das ocorrências de violência registradas entre 2010 e 2020 têm mulheres como as principais vítimas.

Esses dados não apenas destacam a frequência com que as mulheres são afetadas, mas também evidenciam um aspecto preocupante: a violência sexual prevalece, seguida a outras formas de agressão, como violência psicológica/moral, tortura, tráfico humano e outros tipos de violência física.

O estupro e a exploração sexual se destacam como os tipos mais frequentemente registrados de violência sexual. Nos espaços públicos, a insegurança feminina vai além da simples preocupação com perdas materiais, revelando uma complexidade de medos e apreensões. Essas preocupações estão intimamente ligadas às estruturas sociais fundamentadas no patriarcado, perpetuando uma dinâmica de desigualdade na qual as mulheres frequentemente se encontram em uma posição de vulnerabilidade.

Como complemento a esta análise, sugerimos a criação de indicadores específicos para avaliar a violência de gênero nos espaços urbanos, aliada ao desenvolvimento de uma plataforma colaborativa de mapeamento. A proposta com essa ferramenta é oferecer às autoridades uma visão abrangente da infraestrutura urbana, possibilitando a identificação e solução de questões que alimentam a insegurança e a violência contra as mulheres nas cidades brasileiras.



##
Desenvolvido por [Carla Freitas](https://www.linkedin.com/in/freitas-carla/)


