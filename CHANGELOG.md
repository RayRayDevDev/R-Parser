# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [0.2] - 2026-07-11

### Changed
- Upgraded target framework from .NET 7 (EOL) to .NET 10 (LTS).
- Bumped `Magick.NET-Q16-AnyCPU` from 13.1.0 to 14.14.0, fixing a large backlog of ImageMagick CVEs, several of high severity.
- Bumped `MetadataExtractor` from 2.7.2 to 2.9.3.
- Bumped `MediaInfo.Native` and `MediaInfo.Core.Native` from 21.9.1 to 26.1.0.

### Fixed
- Nullable-reference warnings surfaced by the framework upgrade (`Console.ReadLine()` and `Path.GetDirectoryName()` results).

### Documentation
- Added a "How to Run" section to `README.md`.
