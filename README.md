# CSS Image Scaling Bug
This repository demonstrates a subtle bug in CSS that can lead to unexpected image scaling and clipping issues in certain browsers. The bug occurs when combining `overflow: hidden;`, `width: 100%;`, and `height: auto;` on an image within a containing div.

## Bug Description
The CSS code attempts to scale an image to fit its container while maintaining its aspect ratio. However, some browsers may misinterpret the combination of these styles, resulting in the image being clipped or scaled incorrectly.

## Solution
The solution involves using the `object-fit` CSS property to control how the image is resized to fit its container while preventing clipping. This property ensures that the image maintains its aspect ratio and is correctly positioned within the container.