
# AeroRoute Vision: Using Satellite Imagery and Deep Learning for disaster relief 

AeroRoute Vision is an AI-powered solution for emergency response and disaster management, designed to identify road networks and potential helicopter landing zones in satellite imagery.

In the chaotic aftermath of natural disasters or conflict zones, making split-second decisions can mean the difference between life and death. In these critical moments, having accurate road maps is paramount for emergency medical services (EMS) to navigate swiftly and effectively. However, in rural or remote areas, traditional mapping infrastructure often falls short, especially when calamities disrupt regular routes.

To tackle this challenge head-on, this research harnesses the power of satellite imagery and cutting-edge deep learning techniques. By employing sophisticated architectures like U-Net and YOLOv8, we've created a groundbreaking solution that revolutionizes emergency response efforts.

Imagine a scenario where every minute counts, and conventional maps are outdated or nonexistent. Our approach, fueled by a meticulously curated dataset sourced from the Bhoonidhi portal, prioritizes diversity and key features like helicopter landing sites and flood-affected regions. Through the magic of U-Net, we achieve pinpoint precision in mapping roads, while YOLOv8 swiftly identifies optimal landing zones for helicopters.

The beauty of our system lies in its seamless integration of these powerful models, working in tandem to automate crucial tasks and provide real-time insights for emergency responders.

With this innovative model at their fingertips, emergency teams can navigate through chaos with clarity, potentially saving countless lives in the process.

## Setup Environment

1. **Install Dependencies:** Ensure you have the necessary dependencies installed. This includes Python 3.x, along with the following libraries:
   ```bash
   pip install numpy opencv-python torch torchvision
   pip install git+https://github.com/ultralytics/yolov5.git
   ```

2. **Clone Repository:** Clone the SkyPath Finder repository to your local machine:
   ```bash
   git clone https://github.com/tejal-1303/GH_submission.git
   cd skypath-finder
   ```

## Dataset : Related Sources and Content

- **DeepGlobe Land Cover Classification Dataset**
  - [Dataset Link](https://www.kaggle.com/datasets/balraj98/deepglobe-land-cover-classification-dataset)
    ```
    @InProceedings{DeepGlobe18,
     author = {Demir, Ilke and Koperski, Krzysztof and Lindenbaum, David and Pang, Guan and Huang, Jing and Basu,
     Saikat and Hughes, Forest and Tuia, Devis and Raskar, Ramesh},
     title = {DeepGlobe 2018: A Challenge to Parse the Earth Through Satellite Images},
     booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
     month = {June},
     year = {2018}
    }
    ```


- **Helicopter Landing Dataset**
  - [Dataset Link](https://universe.roboflow.com/govind-a-qfk4g/helicopter-landing)
    ```
     @misc{ helicopter-landing_dataset,
      title = { Helicopter Landing Dataset },
      type = { Open Source Dataset },
      author = { Govind A },
      howpublished = { \url{ https://universe.roboflow.com/govind-a-qfk4g/helicopter-landing } },
      url = { https://universe.roboflow.com/govind-a-qfk4g/helicopter-landing },
      journal = { Roboflow Universe },
      publisher = { Roboflow },
      year = { 2023 },
      month = { dec },
      note = { visited on 2024-01-23 },
    }
  ```

  - **Massachusetts Roads Dataset**
  - [Dataset Link](https://www.cs.toronto.edu/~vmnih/data/)
    ```
    @phdthesis{MnihThesis,
     author = {Volodymyr Mnih},
     title = {Machine Learning for Aerial Image Labeling},
     school = {University of Toronto},
     year = {2013}
    }
    ```
- **Training:** Train the models on a powerful machine or consider using cloud-based GPU instances for faster training.
- **Deployment:** Consider deploying the trained models to cloud platforms or edge devices for real-time emergency response applications.
