# FLAM-Assignment-Bounded-Box

I have used the provided dataset to create an algorithm that detects and creates bounding boxes on images. Below, you will find instructions on how to run the project.

## Usage

### 1. Download and Unzip the Dataset
Download the dataset file, named `dataset.zip`, and mount it to your notebook environment like, Google Colab or Jupyter Notebook.

### 2. Copy the Best Model Weight File
You will need the `best.pt` file, which contains the trained model's weights. You can either copy and paste the `best.pt` file saved in the `runs` folder into the `weights` folder of your project, or if needed, download and upload the `best.pt` file directly from this repository.

### 3. Run the Model
You can upload and run the model on any image by following these steps:

- In your notebook environment, execute the following command, replacing `<image_path>` with the path to your image file:

  ```bash
  !yolo task=detect \
  mode=predict \
  model=path/to/weights/best.pt \
  conf=0.9 \
  source=<image_path>
  ```

 
### 4. View Results
After running the model, you can access the results in the `predict` folders that will be generated in the `runs` directory. These folders will contain the images with bounding boxes drawn around detected children for that session.

