# Eternal Love - Wedding Album

## Overview
The "Eternal Love - Wedding Album" website is a beautifully designed webpage showcasing the wedding of Nobita and Shizuka. It includes various sections such as a hero banner, love story timeline, wedding gallery, slideshow, countdown timer, video highlights, and a guest book for comments.

---

## Features

### 1. Hero Section
- **Description**: Displays a full-screen banner with the couple's names and a background image.
- **Key Elements**:
  - Background image with a gradient overlay.
  - Animated text (`fadeIn` animation).

### 2. Love Story Timeline
- **Description**: Highlights key moments in the couple's journey.
- **Key Elements**:
  - Timeline items with animations triggered when scrolled into view.
  - Events include:
    - First Meeting (June 2018)
    - First Date (September 2018)
    - Proposal (December 2022)

### 3. Wedding Gallery
- **Description**: Displays a grid of wedding photos.
- **Key Elements**:
  - Images are displayed in a responsive grid layout.
  - Hover effects include scaling and an overlay.

### 4. Slideshow
- **Description**: A slideshow of wedding images that automatically transitions every 5 seconds.
- **Key Elements**:
  - Images from the gallery are reused in the slideshow.
  - Active slide is highlighted using the `active` class.
  - JavaScript handles the automatic transitions.

### 5. Countdown Timer
- **Description**: Displays a countdown to the couple's first anniversary.
- **Key Elements**:
  - Dynamically updates every second.
  - Shows days, hours, minutes, and seconds remaining.

### 6. Video Highlights
- **Description**: Embeds a YouTube video of the wedding highlights.
- **Key Elements**:
  - Uses an `<iframe>` to embed the video.
  - Supports fullscreen playback.

### 7. Floating Hearts Animation
- **Description**: Adds a romantic touch with floating heart animations.
- **Key Elements**:
  - Hearts are dynamically created and float upwards.
  - JavaScript handles the creation and removal of hearts.

### 8. Guest Book (Comments Section)
- **Description**: Allows visitors to leave comments and wishes for the couple.
- **Key Elements**:
  - Form for entering name and comment.
  - Comments are displayed in a styled list.
  - Comments are saved to `localStorage` and persist across page reloads.

---

## Code Structure

### HTML
- **Sections**:
  - `<section class="hero">`: Hero banner.
  - `<section class="love-story">`: Love story timeline.
  - `<section class="gallery">`: Wedding gallery.
  - `<section class="slideshow">`: Slideshow of images.
  - `<section class="countdown">`: Countdown timer.
  - `<section class="video-section">`: Embedded YouTube video.
  - `<section class="comments-section">`: Guest book for comments.

### CSS
- **Key Styles**:
  - **Hero Section**: Full-screen layout with gradient overlay and text animation.
  - **Gallery**: Responsive grid with hover effects.
  - **Slideshow**: Images are styled to fit the container with smooth transitions.
  - **Comments Section**: Modern card-style layout with shadows and rounded corners.

### JavaScript
- **Features**:
  - **Lightbox**: Enlarges gallery images when clicked.
  - **Scroll Animations**: Animates timeline items when they come into view.
  - **Floating Hearts**: Dynamically creates and animates hearts.
  - **Countdown Timer**: Calculates and updates the time remaining until the anniversary.
  - **Slideshow**: Automatically transitions between slides.
  - **Comments System**:
    - Saves comments to `localStorage`.
    - Loads comments on page load.

---

## How to Use

### 1. View the Website
- Open the `marriage.html` file in a browser to view the website.

### 2. Add Comments
- Scroll to the "Guest Book" section.
- Enter your name and comment, then click "Post Comment."
- Your comment will appear instantly and persist across page reloads.

### 3. Interact with Features
- Hover over gallery images to see effects.
- Watch the slideshow transition automatically.
- Click on gallery images to view them in a lightbox.
- Watch the embedded YouTube video in the "Wedding Highlights" section.

---

## Customization

### 1. Change Images
- Replace the `src` attributes of `<img>` tags in the gallery and slideshow sections with your own image URLs.

### 2. Update Countdown Date
- Modify the `anniversary` variable in the JavaScript section to set a new target date:
  ```javascript
  const anniversary = new Date('YYYY-MM-DD').getTime();