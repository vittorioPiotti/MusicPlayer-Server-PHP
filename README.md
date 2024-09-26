# Music-Player-Server

Server sviluppato per la versione `v.7.3` di PHP per Client Web di Music Player

Link al Client Web di Music Player: [(link)](https://github.com/vittorioPiotti/Music-Player-Web)


#### Support Me


[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/P5P012BC8U)

## Indice :
 - [API](#api)
 - [Albero di Path](#albero-di-path)
 - [Licenze](#licenze)
   
## API

### Indice API:

- [API Home](#api-home)
- [API Music](#api-music)
- [API Artist](#api-artist)


### Lista API:


<div id="api-home"></div>

| API HOME |
|----------|
| **Name**: getSearchedArtists<br>**Endpoint**: [`type=home&method=getSearchedArtists`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getSearchedArtists&searchText=mirage&listIds=)<br>**Type**: `GET`<br>**Parametri**: `searchText=testoDaCercare`, `listIds=1,2,3`<br>**Descrizione**: Cerca artisti in base al testo specificato. |
| **Name**: getSearchedMusics<br>**Endpoint**: [`type=home&method=getSearchedMusics`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getSearchedMusics&searchText=electric&listIds=)<br>**Type**: `GET`<br>**Parametri**: `searchText=testoDaCercare`, `listIds=1,2,3`<br>**Descrizione**: Cerca canzoni in base al testo specificato. |
| **Name**: getAllHomeData<br>**Endpoint**: [`type=home&method=getAllHomeData`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getAllHomeData)<br>**Type**: `GET`<br>**Parametri**: Nessuno<br>**Descrizione**: Ottiene tutti i dati necessari per la schermata iniziale. |
| **Name**: getMusics<br>**Endpoint**: [`type=home&method=getMusics`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getMusics&listIds=)<br>**Type**: `GET`<br>**Parametri**: `listIds=1,2,3`<br>**Descrizione**: Ottiene la lista delle canzoni specificate. |
| **Name**: getArtists<br>**Endpoint**: [`type=home&method=getArtists`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getArtists&listIds)<br>**Type**: `GET`<br>**Parametri**: `listIds=1,2,3`<br>**Descrizione**: Ottiene la lista degli artisti specificati. |




<div id="api-music"></div>


| API MUSIC | 
|-----------| 
| **Name**: getMusic<br>**Endpoint**: [`type=music&method=getMusic`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=music&method=getMusic&idMusic=3)<br>**Type**: `GET`<br>**Parametri**: `idMusic=12`<br>**Descrizione**: Ottiene i dati di una specifica canzone. |
| **Name**: getMusicMin<br>**Endpoint**: [`type=music&method=getMusicMin`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=music&method=getMusicMin&idMusic=2)<br>**Type**: `GET`<br>**Parametri**: `idMusic=12`<br>**Descrizione**: Ottiene dati ridotti di una specifica canzone. |

<div id="api-artist"></div>


| API ARTIST | 
|------------| 
| **Name**: getAllArtistData<br>**Endpoint**: [`type=artist&method=getAllArtistData`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=artist&method=getAllArtistData&idArtist=12)<br>**Type**: `GET`<br>**Parametri**: `idArtist=12`<br>**Descrizione**: Ottiene tutti i dati di un artista specifico. |
| **Name**: getArtist<br>**Endpoint**: [`type=artist&method=getArtist`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=artist&method=getArtist&idArtist=1)<br>**Type**: `GET`<br>**Parametri**: `idArtist=12`<br>**Descrizione**: Ottiene i dati di un artista specifico. |
| **Name**: getAlbums<br>**Endpoint**: [`type=artist&method=getAlbums`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=artist&method=getAlbums&idArtist=12&listIds=)<br>**Type**: `GET`<br>**Parametri**: `idArtist=12`, `listIds=1,2,3`<br>**Descrizione**: Ottiene la lista degli album di un artista. |
| **Name**: getSingles<br>**Endpoint**: [`type=artist&method=getSingle`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=artist&method=getSingles&idArtist=6&listIds=)<br>**Type**: `GET`<br>**Parametri**: `idArtist=12`, `listIds=1,2,3`<br>**Descrizione**: Ottiene la lista dei singoli di un artista. |



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

> [!WARNING]
> Questo software è rilasciato sotto la licenza **GPL v3** quindi l'uso, la modifica e la distribuzione del codice sorgente ne deve rispettare i termini.
> 
> I contenuti multimediali possono essere soggetti a una **licenza non commerciale** richiedendo l'acquisto di una licenza separata.
>
> Gli audio generati da **Suno AI** [(Termini di utilizo)](https://suno.com/terms) necessitano dell'acquisto di una licenza separata per l'uso commerciale.


| Componente         | Versione  | Copyright                         | Licenza                                                       |
|--------------------|-----------|-----------------------------------|---------------------------------------------------------------|
| [DijkstraSolver](https://github.com/vittorioPiotti/MusicPlayer-Server-PHP) | [v1.0.0](https://github.com/vittorioPiotti/MusicPlayer-Server-PHP/releases/tag/v1.0.0)    | 2024 Vittorio Piotti [(GitHub page)](https://github.com/vittorioPiotti) [(Personal page)](https://vittoriopiotti.altervista.org/)            | [GPL-3.0 ](https://github.com/vittorioPiotti/MusicPlayer-Server-PHP/blob/main/LICENSE.md) |

Canzoni generate usando **Suno AI** [(Termini di utilizo)](https://suno.com/terms)

Immagini generate usando **OpenArt** [(Termini di utilizzo)](https://openart.ai/terms)

