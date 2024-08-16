# Music-Player-Server

Server sviluppato per la versione `v.7.3` di PHP per Client Web di Music Player

Link al Client Web di Music Player: [(link)](https://github.com/vittorioPiotti/Music-Player-Web)


## API 

| Nome API                   | URL                                                                           | Parametri                                                | Descrizione                                                                                                      |
|----------------------------|-------------------------------------------------------------------------------|----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|
| **getMusic**               | `type=music&method=getMusic&idMusic=${elementId}`           | `idMusic=${elementId}`                                    | Ottiene i dati di una specifica canzone.                                                                          |
| **getMusicMin**            | `type=music&method=getMusicMin&idMusic=${elementId}`        | `idMusic=${elementId}`                                    | Ottiene dati ridotti di una specifica canzone.                                                                    |
| **getAllArtistData**       | `type=artist&method=getAllArtistData&idArtist=${elementId}` | `idArtist=${elementId}`                                   | Ottiene tutti i dati di un artista specifico.                                                                     |
| **getArtist**              | `type=artist&method=getArtist&idArtist=${elementId}`        | `idArtist=${elementId}`                                   | Ottiene i dati di un artista specifico.                                                                           |
| **getAlbums**              | `type=artist&method=getAlbums&idArtist=${elementId}&listIds=${resultStr}` | `idArtist=${elementId}`, `listIds=${resultStr}`          | Ottiene la lista degli album di un artista.                                                                       |
| **getSingles**             | `type=artist&method=getSingles&idArtist=${elementId}&listIds=${resultStr}` | `idArtist=${elementId}`, `listIds=${resultStr}`          | Ottiene la lista dei singoli di un artista.                                                                       |
| **getMusics**              | `type=home&method=getMusics&listIds=${encodeURIComponent(resultStr)}` | `listIds=${encodeURIComponent(resultStr)}`               | Ottiene la lista delle canzoni specificate.                                                                       |
| **getArtists**             | `type=home&method=getArtists&listIds=${encodeURIComponent(resultStr)}` | `listIds=${encodeURIComponent(resultStr)}`               | Ottiene la lista degli artisti specificati.                                                                       |
| **getSearchedArtists**     | `type=home&method=getSearchedArtists&searchText=${encodeURIComponent(resultREGEXP)}&listIds=${encodeURIComponent(resultStr)}` | `searchText=${encodeURIComponent(resultREGEXP)}`, `listIds=${encodeURIComponent(resultStr)}` | Cerca artisti in base al testo specificato.                                                                        |
| **getSearchedMusics**      | `type=home&method=getSearchedMusics&searchText=${encodeURIComponent(resultREGEXP)}&listIds=${encodeURIComponent(resultStr)}` | `searchText=${encodeURIComponent(resultREGEXP)}`, `listIds=${encodeURIComponent(resultStr)}` | Cerca canzoni in base al testo specificato.                                                                        |
| **getAllHomeData**         | `type=home&method=getAllHomeData`                           | Nessun parametro                                          | Ottiene tutti i dati necessari per la schermata iniziale.                  

## Licenze
| Componente         | Versione  | Copyright                         | Licenza                                                       |
|--------------------|-----------|-----------------------------------|---------------------------------------------------------------|
| Music Player Server | v1.0.0    | 2024 Vittorio Piotti              | [GPL-3.0 License](https://github.com/vittorioPiotti/Music-Player-Server/blob/main/LICENSE.md) |
