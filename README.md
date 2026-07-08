# TRUDI: TRansportation Unit Detection and Identification Dataset
This repository contains the resources for the paper titled "[TRUDI and TITUS: A Multi-Perspective Dataset and A Three-Stage Recognition System for Transportation Unit Identification](https://bmva-archive.org.uk/bmvc/2025/assets/papers/Paper_1134/paper.pdf)" presented at The 36th British Machine Vision Conference (2025).

The TRUDI dataset is the first publicly available dataset captured from both ground and aerial perspectives, designed for the detection and identification of transportation units (intermodal loading units) such as containers and trailers. This dataset was created as part of the [InteGreatDrones](integreatdrones.de) project, to advance the development and evaluation of instance segmentarion, object detection, text detection, and text recognition methods within the logistics sector. 

## Download
The licence for the dataset is Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0). Under this licence, you are free to share, adapt, and use the dataset, including commercially. However, derivative works based on the dataset has to be published under the same licence. We chose this licence to foster innovation and development in serial number detection and recognition.

The download link: https://cloud.uni-hamburg.de/s/82omXqGMLWF8T2c

## Details
![trudi](https://github.com/user-attachments/assets/e36c526c-f1a5-46a6-b8a5-16b2dd547a91)

TRUDI is a densly annotated dataset consisting 733 images (35034 annotated instances) collected from inland ports, using various types of cameras, including UAVs, smartphones, action cameras and DSLRs. The images were taken in span of two years to ensure the various weather and lighting conditions. Additionally, the images feature a range of zoom levels, offering both focused and overview images of transportation units and the ports.

Number of Instances
- Containers: 11109
- Tank containers: 808
- Trailers: 2780
- Logos: 14009
- Text fields: 6328

## Baseline: Three-stage Identification of Transportation UnitS (TITUS)
As a baseline, we created a three-stage transportation unit identification pipeline (TITUS): (1) segmenting TU instances (containers, tank containers, and trailers), (2) detecting their ID text area, (3) extracting the ID code from detected text areas and associating the extracted ID with the corresponding TU instance. We used OpenMMLab frameworks such as [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMOCR](https://github.com/open-mmlab/mmocr/) to build this pipeline. The configurations and model weights for each stage are available in this link: https://cloud.uni-hamburg.de/s/MafTw9kEZ6AKtrz

![system_overview](https://github.com/user-attachments/assets/a149d53d-42e4-4468-870a-68b138e3e396)

## Citation
If you use the TRUDI dataset and/or the TITUS pipeline please cite the following paper:
```
E. Gülsoylu, A. Kelm, L. Bengtson, M. Hirsch, C. Wilms, T. Rolff, J. Edinger, S. Frintrop, TRUDI and TITUS: A Multi-Perspective Dataset and A Three-Stage Recognition System for Transportation Unit Identification, in: Proceedings of the 36th British Machine Vision Conference (BMVC), The British Machine Vision Association and Society for Pattern Recognition (BMVA), 2025, pp. 1–14.
```
```
@inproceedings{Gülsoylu_2025_BMVC,
author    = {Emre Gülsoylu and André Peter Kelm and Lennart Bengtson and Matthias Hirsch and Christian Wilms and Tim Rolff and Janick Edinger and Simone Frintrop},
title     = {TRUDI and TITUS: A Multi-Perspective Dataset and A Three-Stage Recognition System for Transportation Unit Identification},
booktitle = {36th British Machine Vision Conference 2025, {BMVC} 2025, Sheffield, UK, November 24-27, 2025},
publisher = {BMVA},
year      = {2025},
url       = {https://bmva-archive.org.uk/bmvc/2025/assets/papers/Paper_1134/paper.pdf}
}
```
## Licence
<a href="https://github.com/egulsoylu/trudi">TRansportation Unit Detection and Identification Dataset (TRUDI)</a> © 2025 by <a href="https://www.inf.uni-hamburg.de/en/inst/ab/cv/people/guelsoylu.html">Emre Gülsoylu</a> is licensed under <a href="https://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">
