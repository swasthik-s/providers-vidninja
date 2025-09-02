# @p-stream/providers

READ: Most sources marked with 🔥 or 🤝 are only avaliable on https://pstream.mov

Because these scrapers are getting harder and harder to maintain, as they get patched. We need to close-source them. This is unfortunate, but it's the reality of the pirating scene. Sites that we scrape are blocking us, and we keep losing them. Fortunately, P-Stream has partnered with many people who offered their services on the site.
You are still free to self-host; several sources are still usable, with more open-source ones coming soon. If you have experience coding, this is a great oppurtunity to develop your own scrapers. 

package that holds all providers of P-Stream.
Feel free to use for your own projects.

features:
- scrape popular streaming websites
- works in both browser and server-side

Visit documentation here: https://providers.pstream.mov/

## Provider Status (Updated September 2, 2025)

Based on comprehensive testing with Fight Club (TMDB ID: 550), here's the current status of providers:

### ✅ Working Providers (5/11 tested - 45% success rate)

| Provider | Type | Quality | Notes |
|----------|------|---------|-------|
| **cloudnestra** | HLS | Multiple | Proxy depth 2, reliable streaming |
| **rgshows** | HLS | Multiple | Custom headers, stable performance |
| **lookmovie** | HLS | Multiple | 44 subtitle languages, IP-locked |
| **vidnest** | Embeds | Variable | Returns 2 embed URLs (hollymoviehd, allmovies) |
| **hdrezka** | MP4 | 4 levels | Direct file streams, 3 subtitle languages |

### ❌ Disabled Providers (6/11 tested)

| Provider | Issue | Details |
|----------|--------|---------|
| **ridomovies** | Broken embeds | Closeload embed scraper has corrupted decoding |
| **tugaflix** | Geo-blocking | Streamtape embeds blocked in India |
| **fsharetv** | Geo-blocking | Works only with VPN, provides excellent MP4 streams |
| **animetsu** | Broken logic | Returns embed URLs but no actual streams |
| **wecima** | Complex structure | Arabic site with obfuscated JavaScript player |
| **zunime** | API issues | Authentication problems with backend services |

### 🌍 Common Issues

1. **Geo-blocking**: Major issue affecting multiple providers (ridomovies, tugaflix, fsharetv)
2. **Embed Dependencies**: Many providers rely on third-party embeds that get broken/blocked
3. **Anti-Bot Protection**: Sites frequently update obfuscation methods
4. **Domain Changes**: Streaming sites change domains to avoid blocking

### 🔧 Technical Infrastructure

- **Proxy System**: Multi-level proxy support with depth configuration (0, 1, 2)
- **Fetcher Types**: Native, Browser, Browser Extension support
- **Stream Types**: HLS, MP4, File-based with quality selection
- **Subtitle Support**: Multiple languages with VTT format
- **Headers/CORS**: Automatic handling of referer, origin, and CORS restrictions

## How to run locally or test my changes

These topics are also covered in the documentation
