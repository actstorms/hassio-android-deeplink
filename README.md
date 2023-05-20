# hassio-android-deeplink
This repository provides a deep link for Android TV devices in Home Assistant. With this deep link, you can easily navigate to various Android TV apps directly from Home Assistant.

## Categories

- [Streaming Services](#streaming-services)
- [Sports and Live TV](#sports-and-live-tv)
- [Video-on-Demand](#video-on-demand)
- [Other Apps](#other-apps)

## Streaming Services

| App Name                   | URL                                       |
|---------------------------|-------------------------------------------|
| 10Play                    | tenplay://                                 |
| 7Plus                     | seven://                                   |
| ABC iview                 | [https://iview.abc.net.au](https://iview.abc.net.au)                   |
| Apple TV                  | [https://tv.apple.com](https://tv.apple.com)                       |
| Disney+                   | [https://www.disneyplus.com](https://www.disneyplus.com)                 |
| Dropout.tv 4              | vhxdropout://                              |
| HBO Max                   | [https://play.hbomax.com](https://play.hbomax.com) or hbomax://deeplink |
| Netflix                   | [https://www.netflix.com/title](https://www.netflix.com/title) or netflix:// |
| Paramount Plus            | [https://www.paramountplus.com](https://www.paramountplus.com)         |
| Plex                      | plex://                                    |
| Prime Video               | [https://app.primevideo.com](https://app.primevideo.com)                  |
| SkyShowtime               | [https://www.skyshowtime.com/deeplink](https://www.skyshowtime.com/deeplink)       |
| Tubi                      | [https://tubitv.com](https://tubitv.com)                                |
| YouTube TV                | [https://tv.youtube.com](https://tv.youtube.com)                      |

## Sports and Live TV

| App Name                   | URL                                       |
|---------------------------|-------------------------------------------|
| Bally Sports              | ballysports://                             |
| Fox Sports                | foxsports://live [series,movie,watch,category,movies,special,live,channel,ppv-purchase,search] |
| MLB TV                    | mlbatbat://                                |
| NBA: Live Games & Scores  | gametime://                                |
| TBS                       | watchtbs://                                |
| Twitch                    | twitch://home [home,stream,game,video,clip,search,browse,channel,user] |
| Zattoo                    | zattoo://zattoo.com                        |

## Video-on-Demand

| App Name                   | URL                                       |
|---------------------------|-------------------------------------------|
| Discovery Plus            | discoveryplus://                           |
| Viaplay (Norwegian)       | [https://viaplay.no/movies](https://viaplay.no/movies) |
| YouTube                   | [https://www.youtube.com](https://www.youtube.com) or vnd.youtube:// or vnd.youtube.launch:// |

## Other Apps

| App Name                   | URL                                       |
|---------------------------|-------------------------------------------|
| ARD                       | [https://www.ardmediathek.de](https://www.ardmediathek.de)               |
| Arte                      | arte://display                             |
| Auvio                     | auvio://                                   |
| CloudStream               | cloudstreamapp://                          |
| Crunchyroll               | crunchyroll://                             |
| Emby                      | embyatv://tv.emby.embyatv/startapp         |
| Private Internet Access   | piavpn://                                  |
| SmartTubeNext             | [https://www.youtube.com](https://www.youtube.com)                     |
| Spotify                   | spotify://                                 |
| VRT Max                   | vrtnu://vrtnu                              |
| VTM GO                    | vtmgo://                                   |
| ZDF                       | [https://www.zdf.de/filme](https://www.zdf.de/filme)                   |

Source: 

[https://community.home-assistant.io/t/android-tv-remote-app-links-deep-linking-guide/567921](https://community.home-assistant.io/t/android-tv-remote-app-links-deep-linking-guide/567921)


## Example of useage

```yaml 
service: remote.turn_on
data:
  activity: discoveryplus://
target:
  entity_id: remote.shield

  ```
  
## Contributing
Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.