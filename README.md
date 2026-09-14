# FramePair

FramePair is a native macOS app for preparing JPEG photos for mobile-first social platforms. It works with local JPEG files.

FramePair helps landscape photos, including common 16:9 images, work better on vertical screens. Stack two or three matching photos into a taller composition with Merge, or divide one wide photo into consecutive left and right images with Split. Direct export is available when no rearrangement is needed.

[Download FramePair 0.2 DMG](https://github.com/CedricChanning/FramePair-Downloads/releases/download/v0.2/FramePair-0.2-macOS-arm64.dmg) · [All releases](https://github.com/CedricChanning/FramePair-Downloads/releases) · [Report an issue](https://github.com/CedricChanning/FramePair-Downloads/issues)

FramePair 0.2 is a pre-release. The app is signed with Developer ID and notarized by Apple.

## Requirements

- Apple Silicon Mac
- macOS 26.0 or later

## Installation

### DMG (Recommended)

1. Download `FramePair-0.2-macOS-arm64.dmg`
2. Open the disk image
3. Drag `FramePair.app` onto the Applications shortcut
4. Eject the disk image, then open FramePair from Applications

### ZIP (Alternative)

Download `FramePair-0.2-macOS-arm64.zip`, extract it, and move `FramePair.app` into Applications.

> Do not download GitHub's automatically generated Source code archives. They contain repository contents, not a runnable FramePair app.

## Verify the download

Download the matching `.sha256` file into the same folder as the DMG or ZIP, then run:

```bash
cd ~/Downloads
shasum -a 256 -c FramePair-0.2-macOS-arm64.dmg.sha256
```

The expected result ends with `OK`.

| Package | SHA-256 |
|---|---|
| `FramePair-0.2-macOS-arm64.dmg` | `c54b7d8cb95c57ad2862e993ab1c9e7fa8cff8099ddb067a7025bb5d2c95de45` |
| `FramePair-0.2-macOS-arm64.zip` | `364e7c4da501a18527237a842b1d6f80f99e00d799611b18dbbf5a5c2e8f8334` |

## Features

- Local JPEG input from any source
- Direct export without unnecessary JPEG recompression
- Vertical Merge stacks two or three matching photos into a taller composition
- Center Split turns one wide photo into consecutive left and right images for swipe-based viewing
- Mixed Direct, Merge, and Split arrangements in one batch
- Ordered output preview and configurable sequential filenames
- Optional per-file size limit without reducing pixel dimensions

## Image safety and privacy

- Original photos remain read-only
- Existing destination files are never silently overwritten
- Valid RGB ICC color information is retained
- EXIF, GPS, IPTC, and XMP privacy metadata is removed
- Cancellation or export failure rolls back files created by that run

## Known limitations

- Apple Silicon and macOS 26.0 or later only
- JPEG input and output only
- English interface only
- Creates local output files only; no direct social publishing or cloud sync

## Repository scope

This public repository hosts official FramePair downloads, release notes, and issue reports. FramePair's source code is maintained in a separate private repository and is not distributed here.
