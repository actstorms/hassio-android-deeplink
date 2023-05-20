# hassio-android-deeplink
Deeplink for Android tv in Home assistant. 

## Deep links
| App Name                   | URL                                       |
|---------------------------|-------------------------------------------|
|TV2 Play (Norwegin)| tv2play:// |
|Discovery Plus | discoveryplus:// |
|Viaplay (Norwegian) | [https://viaplay.no/movies](https://viaplay.no/movies) |
| 10Play                    | tenplay://                                 |
| 7Plus                     | seven://                                   |
| ABC iview                 | [https://iview.abc.net.au](https://iview.abc.net.au)                   |
| Apple TV                  | [https://tv.apple.com](https://tv.apple.com)                       |
| ARD                       | [https://www.ardmediathek.de](https://www.ardmediathek.de)               |
| Arte                      | arte://display                             |
| Auvio                     | auvio://                                   |
| Bally Sports              | ballysports://                             |
| CloudStream               | cloudstreamapp://                          |
| Crunchyroll               | crunchyroll://                             |
| Disney+                   | [https://www.disneyplus.com](https://www.disneyplus.com)                 |
| Dropout.tv 4              | vhxdropout://                              |
| Emby                      | embyatv://tv.emby.embyatv/startapp         |
| Fox Sports                | foxsports://live [series,movie,watch,category,movies,special,live,channel,ppv-purchase,search] |
| HBO Max                   | [https://play.hbomax.com](https://play.hbomax.com) or hbomax://deeplink |
| MLB TV                    | mlbatbat://                                |
| NBA: Live Games & Scores  | gametime://                                |
| Netflix                   | [https://www.netflix.com/title](https://www.netflix.com/title) or netflix:// |
| Plex                      | plex://                                    |
| Prime Video               | [https://app.primevideo.com](https://app.primevideo.com)                  |
| Private Internet Access   | piavpn://                                  |
| SkyShowtime               | [https://www.skyshowtime.com/deeplink](https://www.skyshowtime.com/deeplink)       |
| SmartTubeNext             | [https://www.youtube.com](https://www.youtube.com)                     |
| SurfShark                 | [https://surfshark.com/locations-ul](https://surfshark.com/locations-ul)         |
| Spotify                   | spotify://                                 |
| TBS                       | watchtbs://                                |
| Twitch                    | twitch://home [home,stream,game,video,clip,search,browse,channel,user] |
| VRT Max                   | vrtnu://vrtnu                              |
| VTM GO                    | vtmgo://                                   |
| YouTube                   | [https://www.youtube.com](https://www.youtube.com) or vnd.youtube:// or vnd.youtube.launch:// |
| Youtube TV                | [https://tv.youtube.com](https://tv.youtube.com)                      |
| Zattoo                    | zattoo://zattoo.com                        |
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