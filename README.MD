# Rotates images, makes the created background transparent

```python
$pip install transparent-rotate
from transparent_rotate import rotate_with_adjusting,rotate_without_adjusting
i1 = r"https://github.com/hansalemaos/screenshots/raw/main/splitted1.png"
i2 = rotate_without_adjusting(
    img="https://github.com/hansalemaos/screenshots/raw/main/papag_00000008.png",
    angle=60,
    save_path=None,
)
# The picture can easily be merged with other pictures

from cv2watermark import merge_image_percentage_width_position

merg3 = merge_image_percentage_width_position(
    back=i1,
    front=i2,
    percentx=20,
    percenty=20,
    front_percentage_width=30,
    save_path="f:\\cv2mergepics\\rotate1.png",
)

i1 = r"https://github.com/hansalemaos/screenshots/raw/main/splitted1.png"
i2 = rotate_with_adjusting(
    img="https://github.com/hansalemaos/screenshots/raw/main/papag_00000008.png",
    angle=60,
    save_path=None,
)


merg3 = merge_image_percentage_width_position(
    back=i1,
    front=i2,
    percentx=20,
    percenty=20,
    front_percentage_width=30,
    save_path="f:\\cv2mergepics\\rotate2.png",
)

```



<img src="https://github.com/hansalemaos/screenshots/raw/main/splitted1.png"/>


<img src="https://github.com/hansalemaos/screenshots/raw/main/papag_00000008.png"/>


<img src="https://github.com/hansalemaos/screenshots/raw/main/rotate1.png"/>


<img src="https://github.com/hansalemaos/screenshots/raw/main/rotate2.png"/>





