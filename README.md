AR Bites 🍲

An AR-powered restaurant menu concept. Browse dishes as usual, then tap View to drop into an interactive 3D model of the meal — rotate it, zoom in, or use View in AR to place it right on your table using your phone's camera.

Built as a lightweight, dependency-free front end: plain HTML, Tailwind CSS (CDN), and Google's <model-viewer> web component for the 3D/AR rendering.

Features

Responsive hero and menu layout, built with Tailwind's utility classes
Category tabs for browsing menu sections (Soup, Salads, Main Course, Drinks, Sandwiches)
Click-to-open modal with a live, rotatable 3D preview of each dish
One-tap AR placement on supported devices (WebXR / Android Scene Viewer / iOS Quick Look)
Fully data-driven cards — add a new dish by adding a card with data-model, data-poster, data-name, and data-price attributes, no extra JS required
Demo

Open ar-bites.html in a browser. For the full AR experience, open the hosted page on a real phone:

iPhone — Safari
Android — Chrome, with Google Play Services for AR (ARCore) installed

AR placement requires a secure context (https://) — it won't activate from a local file:// path.

3D models

Each dish needs a .glb (and ideally .usdz for iOS) 3D model. The current build ships with a placeholder model for testing. Real dish models can be captured with:

Polycam — scan a dish with your phone camera, export directly to .glb/.usdz. Recommended for speed.

Tech stack
HTML5
Tailwind CSS (browser build via CDN)
<model-viewer> by Google
Baloo 2 (Google Fonts)
polycam for image to 3d
