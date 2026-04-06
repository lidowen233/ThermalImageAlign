This project is used to help align the thermal images and original images, which can't align due to the thermal camera's auto-scaling feature. The basic process :
<img width="1005" height="483" alt="Screenshot 2026-04-06 at 3 36 39 PM" src="https://github.com/user-attachments/assets/2cfbdfd3-725e-45e6-9d62-af58bffd87aa" />
1. Extract human contour by YOLO v8
2. Simple human contour
3. Align contours by multi-scale search and Template matching until get the Best Normalized cross-correlation index
4. If the Best Normalized cross-correlation index is less than 0.5, align the images by multi-scale search and Template matching until get the Best  Structural Similarity Index (SSIM)
