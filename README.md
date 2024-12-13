# FinalProject_Deep_Learning
<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>




<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->








<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
The goal of this project was to assess what impact the change in layer number of DenseNets has on binary image classification. This was coupled with a variety of saliency analysis methods as both a learning exercise and method of evaluation.


<p align="right">(<a href="#readme-top">back to top</a>)</p>



### DenseNets Used 

This project used 4 premade DenseNet architectures from the MONAI model zoo database as well as one custom DenseNet. These models were trained on the [Decathlon dataset](http://medicaldecathlon.com). Specifically, the Task01_BrainTumour dataset. Below the confusion matrices and training loss vs validation plots are shown for each model.

DenseNet121

![image](https://github.com/user-attachments/assets/1e34c444-c2c2-4c39-baa1-14e71d89e87a)

![image](https://github.com/user-attachments/assets/43d68775-2fde-46b6-9ee9-4c7d798a8a64)

DenseNet169

![image](https://github.com/user-attachments/assets/2ea331fa-85f9-4d02-8f03-6533bfef2d1a)

![image](https://github.com/user-attachments/assets/569b64e3-17cc-4de2-b93a-69a532d37ea7)

DenseNet201

![image](https://github.com/user-attachments/assets/e10202b9-9cd4-4ea6-aa26-bba123895698)


![image](https://github.com/user-attachments/assets/e71ca6dc-b7e0-4dea-a3ad-9d8058e4112c)

DenseNet264

![image](https://github.com/user-attachments/assets/655d829f-d46f-4108-b280-cf63569e83d1)

![image](https://github.com/user-attachments/assets/67a37ca2-e8da-41ed-a133-c810a6ae5bc5)

CustomDenseNet

![image](https://github.com/user-attachments/assets/70c2c81d-bb0a-4387-9b68-b45ac235b589)

![image](https://github.com/user-attachments/assets/7861b5a9-1e5a-4d2b-91b8-176be8d8ba97)



<!-- Saliency Analysis -->
## Saliency Analysis

GradCam,SmoothGrad,GuidedSmoothGrad,and GuidedVanillaGrad were the methods of saliency analysis used, the code within the notebooks can be rerun on different images from the data set for each model as it selects a random image each time. To avoid bloat of the README only the custom DenseNet has all its methods below, for other models only GradCam images have been included, the remaining analysis can be found within each models respective notebook.

CustomDenseNet

![image](https://github.com/user-attachments/assets/803b8eac-a5ce-4a25-b91f-538936aff5fd) ![image](https://github.com/user-attachments/assets/eaea6fd0-9668-43fd-bd2e-6b5a6b05cd2b) ![image](https://github.com/user-attachments/assets/0190333f-0e53-4dbc-b1d6-65f9fc235b21) ![image](https://github.com/user-attachments/assets/fcfece3f-70fb-41a1-8ac8-cc48438ab34b) ![image](https://github.com/user-attachments/assets/b8980665-2783-4800-921e-9bcfa6b3a45f)

DenseNet121

![image](https://github.com/user-attachments/assets/544e503b-45b4-408f-8151-d7c0cfc6c8a9) ![image](https://github.com/user-attachments/assets/b542dab2-534e-4ea4-b92d-167ba5ecdc53)

DenseNet169

![image](https://github.com/user-attachments/assets/8d777ee6-27ae-488c-9e95-e4e3b55a7fb8) ![image](https://github.com/user-attachments/assets/226815df-cf71-4bec-8e63-d337f9c7eb4f)

DenseNet201

![image](https://github.com/user-attachments/assets/45e90d28-55b1-4da1-bd66-ec38fd0ab7c8) ![image](https://github.com/user-attachments/assets/9b600937-4bd4-4a01-8734-3a0a95cd0898)

DenseNet264

![image](https://github.com/user-attachments/assets/69afa2eb-d19a-4a97-ac20-cfec9a783273) ![image](https://github.com/user-attachments/assets/6e6eabe3-95de-4e46-aaf3-d634e7592cd0)




<!-- Practical Takeaways -->
## Practical Takeaways

There doesn't seem to be a strong correlation with greater layer number and improved accuracy, however, testing wasn't extensive as only 5 models were used. However, the GradCam gradients clearly demonstrate that as layer number increases the model gets a much better undrstanding of the tumor location resulting in the gradient like appearance as opposed to whats seen in DenseNet121 and DenseNet169




<!-- CONTACT -->
## Contact

Ryan Townsend - rmtownse@uvm.edu

Project Link: (https://github.com/RT-Fridge/FinalProject_Deep_Learning.git)
<p align="right">(<a href="#readme-top">back to top</a>)</p>



