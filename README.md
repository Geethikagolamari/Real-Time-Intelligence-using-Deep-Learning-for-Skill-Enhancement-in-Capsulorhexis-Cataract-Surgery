# Real-Time Intelligence using Deep Learning for Skill Enhancement in Capsulorhexis Cataract Surgery
Published in International Conference on Machine Learning Technologies (ICMLT) 2025, Helsinki, Finland.

## Team
- Geethika Golamari
- Aditya Sharma
- Brinda.A
- Yeshaswini C V M
 

The research was carried as a part of our final year project and completed under the guidance of Dr. B Niranjana Krupa and Dr. Manjunath K P.

## ABSTRACT
This research focuses on creating a guidance map
 for computer-assisted cataract surgeries. The main focus is to
 improve surgery duration and assist young practitioners while
 performing cataract surgeries with the capsulorhexis method.
 The research features two phases, namely, the Incision Phase
 and the Capsulorhexis Phase among thirteen different phases
 of cataract surgery. This research provides methods for real
time phase recognition and segmentation. The study uses ResNet
18 for phase recognition to identify the Incision Phase and the
 Capsulorhexis Phase. The model was able to achieve an accuracy
 of 94.42% and F1 Score of 0.9452. UNet with Guidance Filter
 Module (GFM) is used to segment the cornea and the main
 incision knife. The UNet model produced masks with a mean IoU
 of 0.9315, mean Dice of 0.9642 with an inference time of 6.2ms for
 incision knife segmentation. For the task of cornea segmentation,
 the model produced results with an inference time of 6.5ms
 with mean IoU score of 0.9450 and mean Dice score of 0.9716.
 Using the extracted features and the recognized surgical phase,
 a guidance map is plotted for each frame of the video. These
 frames are rendered at 30 Frames Per Second (FPS) to create
 a video. The Incision Phase map provides a guide for the main
 incision and the side ports along with horizontal depth tracking
 of the main incision. The capsulorhexis guidance map provides a
 guide along the rhexis circle (circle along which capsule is torn).

<img src="https://github.com/Geethikagolamari/Real-Time-Intelligence-using-Deep-Learning-for-Skill-Enhancement-in-Capsulorhexis-Cataract-Surgery/blob/main/Images%20in%20readme/Incision_guidance_map_outline.png" alt="Incision Guidance Map Outline" style="width:50%; height:auto;">

<img src="https://github.com/Geethikagolamari/Real-Time-Intelligence-using-Deep-Learning-for-Skill-Enhancement-in-Capsulorhexis-Cataract-Surgery/blob/main/Images%20in%20readme/Incision_Phase_depth.png" alt="Incision Phase: Depth" style="width:50%; height:auto;">

## DATASET
The dataset was taken from the 1000 videos published as Cataract-1k Ghamsarian et.al. and processed for our use case. The codes used were derived from Cataract-1k with a few modifications of our own. 

## CODE
The code has been published in this github repository with the division of Phase recognition and Segmentation with respective phases having their own pre processing codes. The main code containing the guidance map generation is in a seperate folder. The individual phases of the project were kept seperate and not integrated. Only outputs were collected and processed further.
## OUTPUT

<img src="https://github.com/Geethikagolamari/Real-Time-Intelligence-using-Deep-Learning-for-Skill-Enhancement-in-Capsulorhexis-Cataract-Surgery/blob/main/Images%20in%20readme/Capsulorhexis_map.png" alt="Capsulorhexis Map" style="width:50%; height:auto;">


<img src="https://github.com/Geethikagolamari/Real-Time-Intelligence-using-Deep-Learning-for-Skill-Enhancement-in-Capsulorhexis-Cataract-Surgery/blob/main/Images%20in%20readme/Incision_guidance_map.png" alt="Incision Map" style="width:50%; height:auto;">


<img src="https://github.com/Geethikagolamari/Real-Time-Intelligence-using-Deep-Learning-for-Skill-Enhancement-in-Capsulorhexis-Cataract-Surgery/blob/main/Images%20in%20readme/Depth_map.png" alt="Incision Depth Map" style="width:50%; height:auto;">

## Copyrights
Copyright (c) 2022 Negin Ghamsarian;
Copyright (c) 2024 Negin Ghamsarian

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

