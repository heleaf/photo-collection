# photo-collection
Photo collection sharing app 

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
Social photo sharing app (share photos and collections of photos, create collections of photos from other people's photos)

### App Evaluation
- **Category:** Entertainment
- **Mobile:** Easier to share photos and add photos to collections on mobile due to being able to use the camera / photo album directly 
- **Story:** Allows users to find photos, collections of photos, and curate their own photos/collections
- **Market:** Anyone who interacts with photos, can be particularly useful to creatives who want to create mood/photo boards 
- **Habit:** People take photos every day, so having a place where they can record photos/collections will be habit forming
- **Scope:** Can start out very narrow focused (just sharing single photos), can expand to sharing/modifying collections of photos, as well as interacting with other users' photos (comments, reccomended photos/collections), and other media (videos, gifs, audio) 

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**
* User can login
* User can view a feed of photos/collections
* User can add/remove photos/collections of photos to their library
* User can create posts with single photos or collections of photos 
* User can upload photos using camera or photo album 
* User can comment on other people's posts 
* User can search for photos/collections by keywords or tags 
* User can view their library of photos and collections 
* User can modify their existing collections using other people's photos 
* User can filter search results by keywords or tags 

**Optional Nice-to-have Stories**
* User can follow other people to have their posts show up on their feed
* User can view other people's libraries of photos/collections 
* User can scroll infinitely on their feed 
* User can receive photo, collection, or other user reccomendations based on the photos/collections they have saved 
* User can upload other media such as videos, gifs, and audio (which can also be added to collections) 
* User can share media to other social media platforms 
* User can share timed stories/short videos of multiple videos 
* Users can filter search results based on color scheme / other metrics
* Offline database integration (SQL) for some caching

### 2. Screen Archetypes

* Login screen 
   * User can login
* Home feed screen
   * User can view a feed of photos/collections
   * User can add/remove photos/collections of photos to their library
   * User can comment on other people's posts 
   * User can modify their existing collections using other people's photos
   * User can follow other people to have their posts show up on their feed
   * User can scroll infinitely on their feed 
   * User can receive photo, collection, or other user reccomendations based on the photos/collections they have saved
   * User can share media to other social media platforms
* Search screen
   * User can search for photos/collections by keywords or tags 
   * User can filter search results by keywords or tags 
   * User can follow other people to have their posts show up on their feed
   * User can share media to other social media platforms
   * Users can filter search results based on color scheme / other metrics
* Create post screen
   * User can create posts with single photos or collections of photos
   * User can upload photos using camera or photo album
   * User can upload other media such as videos, gifs, and audio (which can also be added to collections) 
   * User can share timed stories/short videos of multiple videos
* Library screen 
   * User can view their library of photos and collections 
   * User can modify their existing collections using other people's photos
   * User can share media to other social media platforms
* Other user library screen
   * User can view other people's libraries of photos/collections 
   * User can share media to other social media platforms

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Home Feed
* Create
* Library 

**Flow Navigation** (Screen to Screen)

* Login Screen
    * => Home Feed
* Registration Screen
    * => Home Feed
* **Home Feed Screen**
    * => Search Screen 
    * => Collection Screen
    * => Photo Screen 
    * => Add Photo to Collection Screen 
* **Create Screen**
    * => Create Photo Post Screen
    * => Create Collection Post Screen 
    * => Home Feed Screen 
* **Library Screen**
    * => Collection Screen
    * => Photo Screen
    * => Collection List Screen 
    * => Photo List Screen 
* Search Screen
    * => Collection Screen
    * => Photo Screen
    * => Collection List Screen 
    * => Photo List Screen
* Create Photo Post Screen
    * => Home Feed Screen
    * => Camera/Photo Album Intent 
* Create Collection Post Screen
    * => Add Photo to Collection Screen 
    * => Home Feed Screen
    * => Camera/Photo Album Intent
* Add Photo to Collection Screen
* Collection Screen
    * => Photo Screen
    * => Comment Screen
* Photo Screen
    * => Add Photo to Collection Screen
    * => Comment Screen
* Collection List Screen
    * => Collection Screen
* Photo List Screen 
    * => Photo Screen 
* Comment Screen

## Wireframes
![Note Jun 14, 2022](https://user-images.githubusercontent.com/59301744/173736359-b543c6a9-846d-4df0-b1dd-a3b9b98db6f9.jpg)


## TODO: Schema 
[This section will be completed in Unit 9]
### TODO: Models
[Add table of models]
### TODO: Networking
- [Add list of network requests by screen ]
- [Create basic snippets for each Parse network request]
- [OPTIONAL: List endpoints if using existing API such as Yelp]
