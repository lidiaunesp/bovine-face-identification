# BovineID

Identificação facial de bovinos via deep learning.

O projeto reconhece animais individualmente a partir de imagens da face e do focinho extraídos de vídeos, oferecendo uma alternativa não invasiva aos métodos tradicionais de identificação, como brincos e marcação a ferro.

## Sobre o projeto

Este repositório contém o material base do projeto, com o pipeline de treino
que combina as três regiões. Cada combinação gera um modelo `best.pt`, salvo em
`outputs/checkpoints`.

## Dados

O material de vídeos não é versionado neste repositório devido ao seu tamanho.
Para executar o treinamento, os vídeos devem ser inseridos em `data/`, divididos
em duas pastas:

- `duplicated_videos/`: animais com mais de um vídeo
- `unique_videos/`: animais com um único vídeo

## Configuração

O pipeline é configurado pelo arquivo `config/config.yaml`, que define, entre
outros parâmetros, as camadas do backbone a serem treinadas e a seed usada na
seleção aleatória dos vídeos.

## Execução

As instruções completas de execução estão descritas no readme dentro do proejto


## Download
Os downloads são sob requisição.

Versão 1: https://drive.google.com/file/d/1LJc9eCp_yTo3MWcr_DR8Qt7XEs9jn0YZ/view?usp=drive_link
