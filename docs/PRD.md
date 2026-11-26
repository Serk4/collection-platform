# Curio

Version: 0.1
Status: Draft
Owner: David
Repository: collection-platform

---

# 1. Vision

Curio is a mobile-first collection management platform that allows users to organize, browse, search, and showcase collections of virtually any item type.

The initial focus is vinyl record collections, but the platform is designed from day one to support books, comics, recipes, video games, movies, action figures, LEGO, trading cards, dolls, and any other collectible category.

Curio should feel like a modern, visually engaging collection browser rather than a traditional spreadsheet or inventory system.

---

# 2. Problem Statement

Collectors often manage collections using:

- Spreadsheets
- Notes apps
- Generic inventory software
- Collection-specific websites

These solutions are often:

- Difficult to browse on mobile
- Not visually appealing
- Limited to a single collection type
- Difficult to extend
- Poor for personal organization

Users want a unified platform for organizing and viewing collections in an intuitive and image-focused way.

---

# 3. Goals

## Primary Goals

- Mobile-first experience
- Fast collection browsing
- Image-centric interface
- Support multiple collection types
- Extensible architecture
- Easy deployment and maintenance

## Secondary Goals

- Public collection sharing
- Collection analytics
- Item valuation
- Import/export functionality
- Collection discovery

---

# 4. Non-Goals (MVP)

The following are explicitly out of scope for the first release:

- Marketplace functionality
- Buying and selling items
- Social feeds
- Real-time collaboration
- AI recognition
- Barcode scanning
- Native iOS or Android applications

These may be considered future enhancements.

---

# 5. Target Users

## Primary User

Collectors who maintain personal collections and want a visual, mobile-friendly way to manage them.

Examples:

- Vinyl collectors
- Comic collectors
- Book collectors
- Recipe curators
- Movie enthusiasts
- Gaming collectors

## Secondary User

Users who want to publicly share curated collections with others.

---

# 6. Success Metrics

## MVP Success Criteria

A user can:

1. Create an account
2. Create a collection
3. Add items to a collection
4. Upload images
5. Browse items using a carousel interface
6. Search items within collections
7. Edit and delete items

If these workflows function reliably, MVP is considered successful.

---

# 7. Core Concepts

## Collection

A user-created container for related items.

Examples:

- My Vinyl Collection
- Marvel Comics
- Favorite Recipes
- Retro Games

---

## Collection Item

An individual object within a collection.

Examples:

- Dark Side of the Moon
- Amazing Spider-Man #252
- Chicken Alfredo Recipe
- Super Mario World

---

## Attributes

Metadata attached to a collection item.

Examples:

Vinyl:

- Artist
- Label
- Genre
- Year

Books:

- Author
- Publisher
- ISBN

Recipes:

- Prep Time
- Cuisine
- Servings

Attributes allow flexible collection types without database redesign.

---

# 8. User Stories

## Collections

As a user,
I want to create collections,
So that I can organize related items.

As a user,
I want to edit collection details,
So that collection information stays accurate.

As a user,
I want to delete collections,
So that I can remove unwanted data.

---

## Items

As a user,
I want to add items to collections,
So that I can track my possessions.

As a user,
I want to edit item information,
So that metadata remains accurate.

As a user,
I want to upload images,
So that collections are visually appealing.

---

## Search

As a user,
I want to search my collections,
So that I can quickly find items.

---

## Browsing

As a user,
I want to swipe through items,
So that browsing feels natural on mobile devices.

---

# 9. MVP Features

## Authentication

- Sign Up
- Sign In
- Sign Out
- Protected Routes

---

## Dashboard

Display:

- Total Collections
- Total Items
- Recent Activity

---

## Collection Management

- Create Collection
- Edit Collection
- Delete Collection
- View Collection

---

## Item Management

- Create Item
- Edit Item
- Delete Item
- Favorite Item
- Upload Image

---

## Carousel Viewer

Primary browsing experience.

Requirements:

- Mobile optimized
- Swipe gestures
- Smooth transitions
- Full-screen images
- Item details view

---

## Search

Search across:

- Collection names
- Item names
- Descriptions
- Attributes

---

# 10. Technical Requirements

Frontend:

- Next.js
- TypeScript
- Tailwind CSS
- shadcn/ui

Backend:

- Next.js Server Actions
- Prisma ORM

Database:

- Neon PostgreSQL

Hosting:

- Vercel

Authentication:

- Auth.js

---

# 11. Data Model

Primary entities:

- User
- Collection
- CollectionItem
- ItemAttribute
- ItemMedia

The platform must support introducing new collection categories without significant schema changes.

---

# 12. Roadmap

## Phase 1 — MVP

- Authentication
- Collections
- Collection Items
- Image Uploads
- Carousel Browsing
- Search

---

## Phase 2 — Enhanced Organization

- Tags
- Filters
- Sorting
- Favorites
- Wishlists

---

## Phase 3 — Public Sharing

- Public Collections
- Shared Links
- Collection Profiles

---

## Phase 4 — Device Features

- Mobile Camera Upload
- Barcode Scanning
- OCR Support

---

## Phase 5 — AI Features

- Item Recognition
- Metadata Suggestions
- Collection Insights
- Smart Tagging

---

# 13. Future Vision

Curio becomes a universal collection platform where users can manage, browse, share, and discover collections of any type through a consistent, mobile-first experience.

The platform should remain flexible enough that supporting a new collectible category requires configuration and metadata, not database redesign.