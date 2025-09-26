# TRUDI: TRansportation Unit Detection and Identification Dataset
[![PWC](https://img.shields.io/badge/%F0%9F%93%8E%20arXiv-Paper-red)](https://arxiv.org/pdf/2508.02372)

The TRUDI dataset is the first publicly available dataset captured from both ground and aerial perspectives, designed for the detection and identification of transportation units (intermodal loading units) such as containers and trailers. This dataset was created as part of the [InteGreatDrones](integreatdrones.de) project, to advance the development and evaluation of object detection, text detection, and text recognition methods within the logistics sector.

The download link: https://cloud.uni-hamburg.de/s/82omXqGMLWF8T2c

![trudi](https://github.com/user-attachments/assets/e36c526c-f1a5-46a6-b8a5-16b2dd547a91)

TRUDI is a densly annotated dataset consisting 733 images (35034 annotated instances) collected from inland ports, using various types of cameras, including UAVs, smartphones, action cameras and DSLRs. The images were taken in span of two years to ensure the various weather and lighting conditions. Additionally, the images feature a range of zoom levels, offering both focused and overview images of transportation units and the ports.

Number of Instances
- Containers: 11109
- Tank containers: 808
- Trailers: 2780
- Logos: 14009
- Text fields: 6328

As a baseline, we created a three-stage transportation unit identification pipeline (TITUS): (1) segmenting TU instances (containers, tank containers, and trailers), (2) detecting their ID text area, (3) extracting the ID code from detected text areas and associating the extracted ID with the corresponding TU instance. We used OpenMMLab frameworks such as [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMOCR](https://github.com/open-mmlab/mmocr/) to build this pipeline. The configurations and model weights for each stage are available in this link: https://cloud.uni-hamburg.de/s/MafTw9kEZ6AKtrz

![system_overview](https://github.com/user-attachments/assets/a149d53d-42e4-4468-870a-68b138e3e396)


If you use the TRUDI dataset and/or the TITUS pipeline please cite the following paper:
```
Gülsoylu, E., Kelm, A., Bengtson, L., Hirsch, M., Wilms, C., Rolff, T., Edinger, J. and Frintrop, S., 2025. TRUDI and TITUS: A Multi-Perspective Dataset and A Three-Stage Recognition System for Transportation Unit Identification. arXiv preprint arXiv:2508.02372.
```
```
@article{gulsoylu2025trudi,
  title={TRUDI and TITUS: A Multi-Perspective Dataset and A Three-Stage Recognition System for Transportation Unit Identification},
  author={G{\"u}lsoylu, Emre and Kelm, Andr{\'e} and Bengtson, Lennart and Hirsch, Matthias and Wilms, Christian and Rolff, Tim and Edinger, Janick and Frintrop, Simone},
  journal={arXiv preprint arXiv:2508.02372},
  year={2025}
}
```
