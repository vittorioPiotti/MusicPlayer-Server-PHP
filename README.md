# Music-Player-Server

Server sviluppato per la versione `v.7.3` di PHP per Client Web di Music Player

Link al Client Web di Music Player: [(link)](https://github.com/vittorioPiotti/Music-Player-Web)


## API


| API HOME |
|----------|
| **Name**: getSearchedArtists<br>**Endpoint**: [`type=home&method=getSearchedArtists&searchText=${encodeURIComponent(resultREGEXP)}&listIds=${encodeURIComponent(resultStr)}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getSearchedArtists&searchText=mirage&listIds=)<br>**Type**: `GET`<br>**Parametri**: `searchText=${encodeURIComponent(resultREGEXP)}`, `listIds=${encodeURIComponent(resultStr)}`<br>**Descrizione**: Cerca artisti in base al testo specificato. |



#### getSearchedMusics
- **Endpoint**: [`type=home&method=getSearchedMusics&searchText=${encodeURIComponent(resultREGEXP)}&listIds=${encodeURIComponent(resultStr)}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getSearchedMusics&searchText=electric&listIds=)
- **Type**: `GET`
- **Parametri**: `searchText=${encodeURIComponent(resultREGEXP)}`, `listIds=${encodeURIComponent(resultStr)}`
- **Descrizione**: Cerca canzoni in base al testo specificato.

#### getAllHomeData
- **Endpoint**: [`type=home&method=getAllHomeData`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getAllHomeData)
- **Type**: `GET`
- **Parametri**: Nessuno
- **Descrizione**: Ottiene tutti i dati necessari per la schermata iniziale.

#### getMusics
- **Endpoint**: [`type=home&method=getMusics&listIds=${encodeURIComponent(resultStr)}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getMusics&listIds=)
- **Type**: `GET`
- **Parametri**: `listIds=${encodeURIComponent(resultStr)}`
- **Descrizione**: Ottiene la lista delle canzoni specificate.

#### getArtists
- **Endpoint**: [`type=home&method=getArtists&listIds=${encodeURIComponent(resultStr)}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getArtists&listIds)
- **Type**: `GET`
- **Parametri**: `listIds=${encodeURIComponent(resultStr)}`
- **Descrizione**: Ottiene la lista degli artisti specificati.


### API ARTIST


### API MUSIC

### getMusic
- **Endpoint**: [`type=music&method=getMusic&idMusic=${elementId}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=music&method=getMusic&idMusic=3)
- **Type**: `GET`
- **Parametri**: `idMusic=${elementId}`
- **Descrizione**: Ottiene i dati di una specifica canzone.

### getMusicMin
- **Endpoint**: [`type=music&method=getMusicMin&idMusic=${elementId}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=music&method=getMusicMin&idMusic=2)
- **Type**: `GET`
- **Parametri**: `idMusic=${elementId}`
- **Descrizione**: Ottiene dati ridotti di una specifica canzone.

### getAllArtistData
- **Endpoint**: [`type=artist&method=getAllArtistData&idArtist=${elementId}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=artist&method=getAllArtistData&idArtist=12)
- **Type**: `GET`
- **Parametri**: `idArtist=${elementId}`
- **Descrizione**: Ottiene tutti i dati di un artista specifico.

### getArtist
- **Endpoint**: [`type=artist&method=getArtist&idArtist=${elementId}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=artist&method=getArtist&idArtist=1)
- **Type**: `GET`
- **Parametri**: `idArtist=${elementId}`
- **Descrizione**: Ottiene i dati di un artista specifico.

### getAlbums
- **Endpoint**: [`type=artist&method=getAlbums&idArtist=${elementId}&listIds=${resultStr}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=artist&method=getAlbums&idArtist=12&listIds=)
- **Type**: `GET`
- **Parametri**: `idArtist=${elementId}`, `listIds=${resultStr}`
- **Descrizione**: Ottiene la lista degli album di un artista.

### getSingles
- **Endpoint**: [`type=artist&method=getSingles&idArtist=${elementId}&listIds=${resultStr}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=artist&method=getSingles&idArtist=6&listIds=)
- **Type**: `GET`
- **Parametri**: `idArtist=${elementId}`, `listIds=${resultStr}`
- **Descrizione**: Ottiene la lista dei singoli di un artista.




### Albero di Path

```bash
$ tree
.
├── Server
│   ├── src
│   │   ├── controllers
│   │   │   ├── CArtist.php
│   │   │   ├── CHome.php
│   │   │   └── CMusic.php
│   │   ├── foundations
│   │   │   ├── FAPI.php
│   │   │   └── FDB.php
│   │   ├── models
│   │   │   ├── MArtist.php
│   │   │   ├── MHome.php
│   │   │   └── MMusic.php
│   │   └── autoloader.php
│   ├── index.php
└── index.php
```


## Licenze
| Componente         | Versione  | Copyright                         | Licenza                                                       |
|--------------------|-----------|-----------------------------------|---------------------------------------------------------------|
| Music Player Server | v1.0.0    | 2024 Vittorio Piotti              | [GPL-3.0 License](https://github.com/vittorioPiotti/Music-Player-Server/blob/main/LICENSE.md) |


Canzoni generate usando Suno AI [(Termini di utilizo)](https://suno.com/terms)

Immagini generate usando OpenArt [(Termini di utilizzo)](https://openart.ai/terms)

