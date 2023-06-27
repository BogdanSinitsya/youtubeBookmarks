# youtube Bookmarks
Saving timestamps in YT videos google chrome extension
# Introduction
This project contains code for a browser extension that adds the ability to bookmark and save the current timestamp on YouTube videos.

# Installation
Clone the repository to your computer:

Open the extensions page in the Chrome web browser.

Enable the developer mode.

Click on the "Load unpacked" button and select the cloned folder from the repository.

The extension will be installed in your browser.

# Usage
Open the YouTube website and watch a video.

A bookmark button in the form of an icon will appear below the video player. Click on it to add the current timestamp as a bookmark.

Bookmarks will be displayed next to the video player. You can click on them to jump directly to the corresponding timestamp in the video.

Add new bookmarks as needed.

# Examples
Here's an example of code that adds a new bookmark:



    const addNewBookmark = (bookmarksElement, bookmark) => {
    const bookmarkTitleElement = document.createElement("div");
    const newBookmarkElement = document.createElement("div");
    bookmarkTitleElement.textContent = bookmark.desc;
    bookmarkTitleElement.className = "bookmark-title";

    newBookmarkElement.id = "bookmark-" + bookmark.time;
    newBookmarkElement.className = "bookmark";
    newBookmarkElement.setAttribute("timestamp", bookmark.time);

    newBookmarkElement.appendChild(bookmarkTitleElement);
    bookmarksElement.appendChild(newBookmarkElement);
    };


# Author
Bogdan Sinitsya- synytsiabohdan@gmail.com
