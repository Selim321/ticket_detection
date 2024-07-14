# ticket_detection

A prototype to test the workflow and integration to the code base. The ML model will be improved later.

## Model Output

The model outputs two classes:
- **Class 1:** Probability of detecting a ticket (range: [0,1]).
- **Class 2:** Probability of detecting any other object.

## Thresholding

A threshold must be used to decide if the image should be classified as "ticket" or not. Typically, the threshold is around 0.5 (e.g., if Class 1 ≥ 0.5, we consider that a ticket was detected).

## Web Interfaces

The following web interfaces are available:
- `verification_cam.html`: Uses the camera for detection.
- `verification_pick.html`: Uses a file picker to select the image to test.
