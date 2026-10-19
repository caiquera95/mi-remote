# Mi Remote — interface PWA (protótipo)

Este pacote contém apenas o PWA, **não** o receptor Android. Os botões só funcionarão após desenvolver e instalar um receptor Android TV compatível, com autenticação, pareamento e endpoints `GET /health` e `POST /api/key` (`{"key":"UP"}` etc.). Não exponha um receptor sem autenticação na rede. O receptor precisa oferecer HTTPS ou arquitetura de mesma origem/ponte adequada: uma página hospedada em HTTPS pode ser bloqueada pelo navegador ao acessar HTTP local (mixed content / private network access / CORS). O protótipo atual serve para avaliar interface e não garante comunicação a partir do GitHub Pages.

Para testar a interface localmente: `python3 -m http.server 8000` nesta pasta, e abra `http://localhost:8000` no computador. Para publicar os arquivos estáticos, use GitHub Pages; a conexão com a TV exige a etapa Android e ajustes de segurança.
