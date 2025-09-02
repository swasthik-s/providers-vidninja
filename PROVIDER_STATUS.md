# Provider Status Report

Last Updated: September 2, 2025

## Testing Details
- **Test Movie**: Fight Club (TMDB ID: 550)
- **Fetcher**: Native
- **Environment**: Windows PowerShell

## Current Testing Progress
- **Total Tested**: 11/~50 providers
- **Success Rate**: 45% (5/11 working)
- **Working**: 5 providers 
- **Failed**: 6 providers

## Source Providers Status

### ✅ Working Providers
| Provider | Status | Notes | Last Tested |
|----------|--------|-------|-------------|
| cloudnestra | ✅ Working | Returns HLS stream with proxy depth 2 | 2025-09-02 |
| rgshows | ✅ Working | Returns HLS stream with custom headers | 2025-09-02 |
| lookmovie | ✅ Working | Returns HLS index.m3u8 + 44 subtitle languages, ip-locked flag | 2025-09-02 |
| vidnest | ✅ Working | Returns 2 embed URLs (hollymoviehd, allmovies) | 2025-09-02 |
| hdrezka | ✅ Working | File-based MP4 streams, 4 qualities + 3 subtitle languages | 2025-09-02 |

### ❌ Failing Providers
| Provider | Status | Error | Last Tested |
|----------|--------|-------|-------------|
| ridomovies | ❌ Disabled | Depends on closeload embed, which has broken decoding logic | 2025-09-02 |
| zunime | ❌ Disabled | API authentication issues with backend services | 2025-09-02 |
| tugaflix | ❌ Disabled | Mixed embeds (mixdrop/streamtape), streamtape blocked in India | 2025-09-02 |
| animetsu | ❌ Disabled | Returns embed URLs but no actual streams, anime-only | 2025-09-02 |
| wecima | ❌ Disabled | Arabic site, complex embed structure not extracting streams | 2025-09-02 |
| fsharetv | ❌ Disabled | Geo-blocked, works only with VPN (provides MP4 streams) | 2025-09-02 |

### ⏳ Pending Tests
| Provider | Rank | Media Types | Notes |
|----------|------|-------------|-------|
| vidsrcvip | 200 | Movies/Shows | - |
| vidify | 180 | Movies/Shows | - |
| animeflv | 170 | Movies/Shows | - |
| animeflv | 170 | Movies/Shows | - |
| catflix | 160 | Movies/Shows | - |
| coitus | 150 | Movies/Shows | - |
| cuevana3 | 140 | Movies/Shows | - |
| embedsu | 130 | Movies/Shows | - |
| fsharetv | 120 | Movies/Shows | - |
| iosmirror | 110 | Movies/Shows | - |
| iosmirrorpv | 105 | Movies/Shows | - |
| madplay | 100 | Movies/Shows | - |
| mp4hydra | 95 | Movies/Shows | - |
| nepu | 90 | Movies/Shows | - |
| nunflix | 85 | Movies/Shows | - |
| pirxcy | 80 | Movies/Shows | - |
| slidemovies | 70 | Movies/Shows | - |
| streambox | 65 | Movies/Shows | - |
| streambox | 65 | Movies/Shows | - |
| vidapiclick | 60 | Movies/Shows | - |
| wecima | 55 | Movies/Shows | - |
| zoechip | 50 | Movies/Shows | - |
| autoembed | 35 | Movies/Shows | - |
| cinemaos | 30 | Movies/Shows | - |

## Embed Providers Status

### ⏳ Pending Tests
| Provider | Rank | Notes |
|----------|------|-------|
| upcloud | 201 | - |
| vidcloud | 201 | Disabled, uses upcloud |
| streamwish | 125 | - |
| mp4hydra | 120 | - |
| mixdrop | 115 | - |
| streamtape | 110 | - |
| dood | 105 | - |
| streamvid | 100 | - |
| vidsrcsu | 95 | - |
| ridoo | 90 | - |
| turbovid | 85 | - |
| closeload | 80 | - |
| viper | 75 | - |
| madplay | 70 | - |
| animetsu | 65 | - |
| autoembed | 60 | - |
| cinemaos | 55 | - |
| zunime | 50 | - |

## Common Issues Encountered
1. **Connection Timeouts**: Sites may be down or blocking requests
2. **Domain Changes**: Streaming sites frequently change domains
3. **Anti-Bot Protection**: Sites may have enhanced protection
4. **Geo-blocking**: Some sites may be region-restricted

## Next Steps
- Continue testing providers in rank order
- Update status as testing progresses
- Identify patterns in failures
- Document working provider configurations
