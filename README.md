# PixLoom

A wallpaper browsing app for iOS and Android, built with React Native and Expo. Browse curated wallpapers across collections, preview them full-screen, and save them straight to your device gallery.

## Features

- **Three-tab navigation** — *For You*, *Explore*, and *Account*, using file-based routing.
- **Explore** — an animated carousel header that scales and fades on scroll, sitting above a two-column wallpaper grid.
- **For You** — swipeable top-tab sections for *Library*, *Liked*, and *Suggested* collections.
- **Full-screen preview** — tapping any wallpaper opens a draggable bottom sheet with the image, title, and actions.
- **Download to gallery** — saves the selected wallpaper to the device's photo library, with runtime permission handling.
- **Light / dark / system theming** — switchable from the Account tab and applied across every screen.

## Tech Stack

- **React Native**
- **TypeScript**
- **Expo Router** — file-based navigation
- **React Navigation** — material top tabs
- **React Native Reanimated** — carousel and scroll-driven header animations
- **Gorhom Bottom Sheet** — preview sheet
- **Expo Media Library** + **Expo File System** — image download and gallery saving

## Getting Started

**Prerequisites:** Node.js, the Expo Go app (or an Android/iOS emulator).

```bash
# 1. Install dependencies
npm install

# 2. Add your environment variables (see below)

# 3. Start the dev server
npx expo start
```

Scan the QR code with Expo Go, or press `a` / `i` to launch an Android emulator or iOS simulator.

### Environment

Create a `.env` file in the project root:

```
REACT_APP_UNSPLASH_API_KEY=your_key_here
```

## Project Structure

```
app/            Screens and routing (tab layout + For You / Explore / Account)
components/     Reusable UI (ImageCard, SplitView, BottomSheet, themed views)
hooks/          Wallpaper data, carousel data, color-scheme helpers
constants/      Theme colors
services/       Data-source layer
```
