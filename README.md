# BovineID

Identificação facial de bovinos via deep learning.

O projeto reconhece animais individualmente a partir de imagens da face e do focinho extraídos de vídeos, oferecendo uma alternativa não invasiva aos métodos tradicionais de identificação, como brincos e marcação a ferro.

# Cattle ReID API

Pacote Python independente para identificar bovinos em video usando YOLO + ReID.

## Uso rapido

```python
from cattle_reid_api import identify_bovine_from_video, add_bovine_from_video

result = identify_bovine_from_video("video.mp4")
print(result["cow_id"], result["score"], result["status"])

add_bovine_from_video("NE_1234", "novo_bovino.mp4")
```

## Artefatos incluidos

- `models/yolo/best.pt`: detector YOLO.
- `models/reid/best.pt`: checkpoint ReID `head+face+muzzle`.
- `gallery/head_face_muzzle_gallery.npz`: galeria atualizavel de bovinos conhecidos.

A funcao `add_bovine_from_video` extrai embeddings validas do video, cria um prototipo medio normalizado e adiciona/substitui esse bovino na galeria.

## Observação

Para um correto funcionamento, é necessário que o projeto disponha das bibliotecas definidas em `requirements.txt`. Com isso, caso ainda não os tenha, instale no ambiente de uso.


## Download
Os downloads são sob requisição.

Versão 1: https://drive.google.com/file/d/1LJc9eCp_yTo3MWcr_DR8Qt7XEs9jn0YZ/view?usp=drive_link
