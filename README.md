# Criação de Shapefile do RISP do estado Espírito Santo

Repositório de criação de arquivos shapefiles de acordo com as Regiões Integradas de Segurança Pública (RISP) do estado do Espírito Santo.

## Índice de Conteúdo

- [Descrição do Projeto](#descrição-do-projeto)
- [Shapefile do RISP do estado do Espírito Santo](#criação-de-shapefile-do-risp-do-estado-espírito-santo)
- [Programas e Arquivos Usados](#programas-e-arquivos-usados)
- [Instalação e Dependências](#instalação-e-dependências)
- [Guia de Uso](#guia-de-uso)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Licença](#licença)
- [Autores](#autores)
- [Referência](#referência)

## Descrição do Projeto

O crime organizado e a proliferação de diversos delitos exigem uma nova dinâmica dos órgãos de segurança e do Sistema de Persecução Criminal. Esse desafio, de potencializar tecnologia, integração, estatísticas, inteligência e cooperação, encontrou em alguns estados as condições adequadas para a construção de um novo modelo: a instituição das Regiões Integradas de Segurança Pública (RISP).

As RISP são um arranjo territorial no qual há uma divisão em microrregiões estaduais, contemplando cidades com demandas comuns. Nessas regiões, são instalados Centros Integrados de Comando e Controle (CICC), que reúnem todos os órgãos de segurança pública e permitem customizar políticas de segurança à realidade local. Esse modelo potencializa a ação das autoridades e otimiza recursos, promovendo uma atuação integrada e colegiada.

Esse projeto busca preencher uma lacuna, já que poucos estados brasileiros possuem arquivos shapefiles divididos por RISP. O repositório visa ajudar profissionais e pesquisadores interessados em arquivos geoespaciais que refletem a divisão das RISP no Espírito Santo.

## Shapefile do RISP do estado do Espírito Santo

Se você deseja somente baixar o shapefile com as regiões do RISP do ES, basta realizar o download [nesse link](/output/SHAPEFILE_RISP_ES.zip).

## Programas e arquivos usados

- Arquivo shapefile do estado do Espírito Santo (disponível no site do IBGE).
- Scripts em Python.

## Instalação e Dependências

Para rodar o projeto, ou seja, para juntar as partes das cidades e tornar um região, certifique-se de ter as seguintes dependências instaladas:

- **Python** 3.x
- Bibliotecas: `os`, `unidecode`, `pandas`, `geopandas`,  e `matplotlib.pylot`

Instale as dependências com:

```bash
!pip install unidecode -q
!pip install geopandas -q
```

## Guia de Uso

Clone o repositório:

```bash
git clone https://github.com/vert-brasil/Mapa-RISP-ES.git
```

Navegue até o diretório do projeto:

```bash
cd seurepositorio
```

Execute o script principal para gerar o shapefile. Nele, há uma passo a passo de como as cidades se relacionam com o RISP que está em `data`:

```bash
python scripts/shapefile_risp_es.ipynb
```

## Estrutura do Projeto

```bash
seurepositorio/
├── data/
├── scripts/
├── output/
└── README.md
```

## Licença

[CC0 1.0 Universal](/LICENSE)

## Autores

- [Arthur Diego Pereira](https://www.linkedin.com/in/arthurdiegopereira/)
- [Matheus Henrique Malta Valadares](https://github.com/matheus-valadares)
- [Rafhael de Oliveira Martins](https://github.com/rafhaelom)

## Referência

- [Programa Estado Presente - Eixo Proteção Policial](https://sesp.es.gov.br/Media/Sesp/Prog.%20EP/MANUAL%20B%C3%81SICO%20DO%20PROGRAMA%20ESTADO%20PRESENTE%20-%20EIXO%20PROTE%C3%87%C3%83O%20POLICIAL.pdf) - Acessado em 04/11/2024 17:14
- [Regiões Integradas (RISP): Uma nova abordagem da Segurança Pública](https://www.correiodopovo.com.br/blogs/2.221/regi%C3%B5es-integradas-risp-uma-nova-abordagem-da-seguran%C3%A7a-p%C3%BAblica-1.1084987#:~:text=As%20Risp%20s%C3%A3o%20um%20novo,%C3%A0%20realidade%20local%2C%20potencializando%20a)- Acessado em 04/11/2024 17:20