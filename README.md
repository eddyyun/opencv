# opencv
python opencv hand recognition

Pre-Processing

- Captured and set up the template images
- Set up functions for use to process images (Frame differencing, Motion Energy, Skin RGB Detection)
Recognition

- Capture live feed from camera
- Set a rectanglular area where we will detect hand gestures
- Changed image to use white pixels for skin colored pixels of captured feed
- Used CV2.TM_CCOEFF_NORMED for template matching function with Thresholds of 0.6 for Static Gestures and 0.4 for Dynamic Gestsure
- Frame Differencing + Motion Energy/History to compare to template of dynamic gesture(Waving)
Post-Processing

- Tested 20 trials each for Paper, Rock, Waving, Other, and Not Recognized
- Created Confusion Matrix for Paper, Rock, and Waving and calculated Precision, Recall, and F-1 Scores for respective Gestures
