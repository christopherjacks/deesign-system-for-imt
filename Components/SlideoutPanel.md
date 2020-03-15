# Slide-Out Panel
This spec describes the function of the slide-out panel that holds help content and other secondary content on phones and other devices.

## Breakpoints

Up to 479 (phone portrait)
* Width is 90% of viewport width, up to a max width of 360px
* Height is 100%, max 1000px
* Anchored to the upper-right corner of the viewport.
* Lightbox effect (semi-transparent background, the user must close the panel to interact with main screen)

480px to 767px (phone portrait and landscape, tablet portrait)
* Width is 360px
* Height is 100%, max 1000px
* Anchored to the upper-right corner of the viewport.
* Lightbox effect (semi-transparent background, the user must close the panel to interact with main screen)

768px and above (tablet landscape, laptop, desktop)
* Width is 360px
* Height is 100%, max 1000px
* ~~Anchored on the right side of the viewport, sitting just below the green header bar.~~
  * ~~If this is a pain, we can just anchor at the top, but I'm trying to leave the phone number and navigation items exposed when the user can interact with the rest of the page.~~
* ~~No lightbox effect (the user can interact with main screen)~~
* Note: For Convex MVP, the panel will work the same across all breakpoints. For 1.0 or 1.n, we may want to create a different component that would display help and other content on the right, but not in a slide-out panel.

## Behaviors

The panel slides out from the right on all devices. It slides to the right when it closes. Slide duration is 500ms. Note: I'm using 500ms in my prototyping tool. If the duration doesn't seem right in the actual code, I'm open to suggestions.

~~When the panel is open and the user goes to the next or previous screeen, the Help panel should close as the screen transition is occuring.~~ Not for Convex MVP; maybe for 1.0. See the above note.

When there is more content than can be displayed in the panel, a vertical scrollbar appears to let the user know they can scroll to see more content. If scrollbars are controlled by the browser fine, the main requirement is that the user should be able to scroll vertically.

## Elements

The panel has the following items:
* A heading, which should reflect the subject of the current screen (e.g., Destination Help or Travel Dates Help).
* A Close button (X) at the top of the panel.
* Main content.
* A More Help paragraph that appears after help content in the panel.
  * A “call:” link with the appropriate phone number.
  * A “chat with us” link that opens SnapEngage.
* A Close link at the bottom of the panel.

## Tracking for Analytics
We want to know when people interact with screen elements, including elements in the panel, so the following items should register events for Google Analytics:
* Clicks on FAQ headings to show or hide FAQ content. We want to know which topics are popular and which never get clicked. We want to know also which clicks are opening and which clicks are closing the content.
* Clicks on Learn More links in help content.
  * Note: Learn More links aren't in the MVP release.
* Close clicks on the Close button at the top of the Help panel.
* Close clicks on the Close link at the bottom of the Help panel.
* Clicks on the phone number in the More Help paragraph.
* Clicks on the Chat With Us link in the More Help paragraph.