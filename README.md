# masque
## Face Isolation using JSFeat

Goal: extract face from webcam video

Process:
* Detect and crop to largest face
* Convert RGB to HSV, keeping the Hue channel to key off of [skin tone](https://larryjordan.com/articles/color-correction-make-people-look-normal)
* Morphological operations on the hue key to isolate face and clean up edges.
* Use mask as alpha channel for Canvas image data.
