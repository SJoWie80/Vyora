# VyoraXR 0.1.0-alpha9

## Highlights

- Added Stripchat as a separate live-cam source alongside Chaturbate.
- Added Stripchat Featured, Women, Men, Couples and Trans categories.
- Added Stripchat model thumbnails, viewer counts, search and pagination.
- Added direct Stripchat HLS playback for regular live streams.
- Removed the experimental Stripchat VR category because the public API does not expose a reliable separate SBS stream.
- Kept the regular Stripchat source available while avoiding incorrect VR playback claims.
- Improved live-source separation and active-source highlighting in the navigation.

## Notes

- Stripchat uses its public models endpoint with the configured affiliate user ID.
- The public endpoint reports VR capability but does not provide a separate SBS stream; VR is therefore not shown as a supported Stripchat mode in this release.
- Existing Stash, PLAYA VR, Chaturbate, Eporner, RedTube, ImageFap and local playback features remain available.
