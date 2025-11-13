🎵 Exercícios SQL — Nível Mediano (Banco Chinook)

Bem-vindo(a) ao desafio SQL — Nível Mediano, utilizando o banco de dados Chinook, um dos mais populares para práticas de consultas SQL.
Aqui, você colocará em prática seus conhecimentos sobre filtros, JOINs, aliases e consultas relacionais.

🧠 Objetivo do exercício

Praticar consultas intermediárias em SQL, explorando relacionamentos entre tabelas e aplicando filtros condicionais, com base em cenários reais de um banco de dados musical.

📂 Banco de dados utilizado

O Chinook Database simula uma loja de música digital.
Ele contém tabelas como:

Customer (clientes)

Album (álbuns)

Artist (artistas)

Track (faixas)

Genre (gêneros musicais)

🧾 Exercícios
🧍‍♂️ 1. Clientes do Canadá

Mostre o nome completo e o e-mail de todos os clientes que moram no Canadá.

Dicas:

Tabela: Customer

Filtro: WHERE Country = 'Canada'

Colunas: FirstName, LastName, Email

💿 2. Álbuns e Artistas

Exiba o nome do álbum e o nome do artista correspondente.

Dicas:

Tabelas: Album, Artist

Relação: Album.ArtistId = Artist.ArtistId

Utilize JOIN para unir as tabelas

🎸 3. Faixas do gênero Rock

Liste todas as músicas do gênero “Rock”, mostrando também o nome do álbum e o nome do artista.

Dicas:

Tabelas: Track, Genre, Album, Artist

Relações:

Track -> Genre (GenreId)

Track -> Album (AlbumId)

Album -> Artist (ArtistId)

Filtro: WHERE Genre.Name = 'Rock'

Utilize aliases para deixar a consulta mais legível

⏱️ 4. Faixas longas

Mostre todas as faixas com duração maior que 300000 milissegundos.

Dicas:

Tabelas: Track, Album

Relação: Track.AlbumId = Album.AlbumId

Filtro: WHERE Milliseconds > 300000

Colunas para exibir: Track.Name, Composer, Album.Title

💡 Dicas gerais

Use JOINs para combinar informações de múltiplas tabelas.

Utilize aliases para deixar o código mais limpo.

Teste as consultas passo a passo: primeiro o filtro, depois os JOINs.

Organize os resultados com ORDER BY para facilitar a visualização.

🚀 Objetivo final

Ao concluir todos os exercícios, você terá praticado:

Combinação de tabelas com INNER JOIN

Aplicação de filtros condicionais

Consulta de múltiplas tabelas relacionadas

Melhoria na legibilidade e estrutura das queries SQL

Bons estudos e boas consultas! 💻🎶
