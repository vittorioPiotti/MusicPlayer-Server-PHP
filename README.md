# Music-Player-Server

Server sviluppato per la versione `v.7.3` di PHP per Client Web di Music Player

Link al Client Web di Music Player: [(link)](https://github.com/vittorioPiotti/Music-Player-Web)


## API


|API HOME|
|--------|
|
- **Name**: getSearchedArtists
- **Endpoint**: [`type=home&method=getSearchedArtists&searchText=${encodeURIComponent(resultREGEXP)}&listIds=${encodeURIComponent(resultStr)}`](https://vittoriopiotti.altervista.org/MusicPlayer/Server/index.php?type=home&method=getSearchedArtists&searchText=mirage&listIds=)
- **Type**: `GET`
- **Parametri**: `searchText=${encodeURIComponent(resultREGEXP)}`, `listIds=${encodeURIComponent(resultStr)}`
- **Descrizione**: Cerca artisti in base al testo specificato.
|




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

