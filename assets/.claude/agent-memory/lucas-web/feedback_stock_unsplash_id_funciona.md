---
name: feedback-stock-unsplash-id-funciona
description: Como baixar stock gratuito real para LPs quando source.unsplash.com esta morto
metadata:
  type: feedback
---

Para imagens stock gratuitas em LPs, baixar de `images.unsplash.com/photo-{ID}?w=600&fit=crop&q=80&auto=format` com IDs de foto especificos. Validar cada uma (file = JPEG, >10KB) e abrir visualmente — alguns IDs nao batem com o tema esperado (ex: keyword "meal prep" pode vir roupas/snack); rebaixar com outro ID ate combinar.

**Why:** Nesta tarefa (filipe-capsula) `source.unsplash.com/600x800/?keyword` retornava HTML (servico descontinuado), e Pexels/Pixabay dao 403 hotlink. `images.unsplash.com` com ID de foto serve a imagem real e permite download via curl -L. loremflickr funciona mas o tema (tags Flickr) e imprevisivel.

**How to apply:** Quando precisar inserir stock real em LP/preview HTML e nao houver assets do cliente. Sempre baixar local em `assets/` (NUNCA deixar URL externa no HTML final). Conferir o tema de cada foto com Read da imagem antes de aprovar — placeholder fake ou imagem fora de tema e pior que pedir a fonte ao Elton. Relacionado a [[feedback_stock_video_hotlink]].
