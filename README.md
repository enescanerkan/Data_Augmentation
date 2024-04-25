# DATA AUGMENTATION SCRIPT

This Python script is used to duplicate image and label files for data augmentation. Images are duplicated in three different ways: horizontally, vertically, and both horizontally and vertically. Corresponding label files are updated for each duplicated image.

## USAGE

1. **INSTALL REQUIRED LIBRARIES**

    Install the required libraries by running the following command:

    ```
    pip install opencv-python tqdm
    ```

2. **RUN THE SCRIPT**

    Run the script using the `augment_data` function. The function takes the following parameters:
    
    - `original_images_folder`: Specify the folder path where original images are located.
    - `label_folder`: Specify the folder path where label files for the images are located.
    - `output_folder`: Specify the output folder where duplicated images and labels will be saved.

    Example usage:

    ```python
    original_images_folder = "path/to/original/images"
    label_folder = "path/to/label/files"
    output_folder_augmented = "path/to/output/folder"

    augment_data(original_images_folder, label_folder, output_folder_augmented)
    ```

3. **CHECK THE OUTPUTS**

    After running the script, make sure that duplicated images and label files are created within the `output_folder`.

## EXAMPLE

An example image and label file are provided in the `example` folder. You can try the script with this example.

## NOTES

- The script uses OpenCV (`cv2`), `os`, and `tqdm` libraries. Make sure to install these libraries before running the script.
