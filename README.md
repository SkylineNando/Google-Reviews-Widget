# Google-Reviews-Widget

Este widget exibe as 5 principais avaliações do Google, incluindo o nome do autor, sua foto de perfil, a classificação em estrelas e o texto da avaliação.

## Como usar

Obtenha a chave da API do Google Places: Para usar este widget, você precisará de uma chave da API do Google Places. Você pode obter uma no <a href="https://cloud.google.com">Google Cloud Console</a>.

Encontre o Place ID: Use a Ferramenta de <a href="https://developers.google.com/maps/documentation/javascript/place-id?hl=pt-br">Place ID do Google</a> para encontrar o Place ID.

Inclua o widget no seu site: Adicione o seguinte código HTML ao seu site, substituindo ```SUA_CHAVE_DA_API``` pela sua chave da API do Google Places e ```ID_DO_LUGAR``` pelo Place ID.

```html
Copy code
<!DOCTYPE html>
<html>
<head>
  <title>Google Reviews Widget</title>
  <script src="https://maps.googleapis.com/maps/api/js?key=SUA_CHAVE_DA_API&libraries=places"></script>
  <style>
    /* Estilos do widget */
  </style>
  <script>
    /* Código JavaScript do widget */
  </script>
</head>
<body onload="initMap()">
  <div class="reviews-container" id="google-reviews"></div>
</body>
</html>
```
## Personalização

Estilos: Você pode personalizar os estilos do widget editando as regras CSS dentro da tag ```<style>``` no código fornecido.
Número de avaliações: Por padrão, o widget exibe as 5 principais avaliações. Você pode alterar esse número modificando o valor passado para o método slice() na variável reviews no código JavaScript.

## Limitações

O widget depende da API do Google Places, que possui limites de uso e pode incorrer em custos se excedidos.
As avaliações exibidas são determinadas pelo Google e podem não representar todas as avaliações disponíveis para o local.

## Suporte

Para obter ajuda com este widget ou para relatar problemas, entre em contato com o desenvolvedor ou consulte a documentação da API do Google Places.
