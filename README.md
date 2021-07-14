# Survey on Adversarial Machine Learning

Literature survey of Adversarial Machine Learning especially in the context of self-driving vehicles and physical realizability

## Page Structure
- Important Conferences
- Important People and Groups
- Important Terminology
- Important Papers
- Uses [shield.io](https://shields.io/) badges to show information at a glance (ex: ![](https://img.shields.io/badge/impact--factor-33.49-purple), ![](https://img.shields.io/badge/sensor-camera-orange.svg))

## Important Conferences

### NeurIPS  ![](https://img.shields.io/badge/impact--factor-33.49-purple)
- Neural Information Processing Systems
- Dec 6, 2021 - Dec 14, 2021 - Online
- Premier machine learning conference

### AAAI  ![](https://img.shields.io/badge/impact--factor-25.57-purple)
- AAAI Conference on Artificial Intelligence
- Feb 2, 2021 - Feb 9, 2021 - Vancouver, Canada

### ICML  ![](https://img.shields.io/badge/impact--factor-18.48-purple)
- International Conference on Machine Learning
- Jul 18, 2021 - Jul 24, 2021 - Vienna, Austria

### ICLR  ![](https://img.shields.io/badge/impact--factor-11.38-purple)
- International Conference on Learning Representations 
- May 4, 2021 - May 8, 2021 - Vienna, Austria

### IJCAI  ![](https://img.shields.io/badge/impact--factor-11.71-purple)
- International Joint Conference on Artificial Intelligence
- Aug 21, 2021 - Aug 26, 2021 - Montreal, Canada

### CVPR  ![](https://img.shields.io/badge/impact--factor-51.98-purple)
- Conference on Computer Vision and Pattern Recognition 
- Jun 21, 2021 - Jun 24, 2021 - Nashville, United States
- Premier Computer Vision Conference

## Important People and Groups:

#### Ian Goodfellow [![](https://img.shields.io/badge/h--index-71-blue.svg)](https://scholar.google.com/citations?hl=en&user=iYN86KEAAAAJ)
#### Nicolas Papernot [![](https://img.shields.io/badge/h--index-32-blue.svg)](https://scholar.google.com/citations?user=cGxq0cMAAAAJ)
#### Nicholas Carlini [![](https://img.shields.io/badge/h--index-28-blue.svg)](https://scholar.google.com/citations?user=q4qDvAoAAAAJ)
#### Christian Szegedy [![](https://img.shields.io/badge/h--index-23-blue.svg)](https://scholar.google.com/citations?hl=en&user=3QeF7mAAAAAJ)
#### Kevin Eykholt [![](https://img.shields.io/badge/h--index-6-blue.svg)](https://scholar.google.com/citations?hl=en&user=f_LN0jUAAAAJ)
#### Bo Li [![](https://img.shields.io/badge/h--index-40-blue.svg)](https://scholar.google.com/citations?user=K8vJkTcAAAAJ&hl=en&oi=sra)
#### Yevgeniy Vorobeychik [![](https://img.shields.io/badge/h--index-36-blue.svg)](https://scholar.google.com/citations?hl=en&user=ptI-HHkAAAAJ)

```
todo: add more information about authors (key contributions, etc.)
```
---

## Important Terminology

### Attack types based on DNN model knowledge
#### White-box attacks
#### Black-box attacks

### Types based on attack setting
#### Theoretical
#### Digital (usually against image classifiers)
#### Simulation
#### Physical

## Important Papers

### Seminal Papers

#### Dalvi, Nilesh, et al. "Adversarial classification." Proceedings of the tenth ACM SIGKDD international conference on Knowledge discovery and data mining. 2004. ![](https://img.shields.io/badge/type-theory-brightgreen.svg) 

#### Lowd, Daniel, and Christopher Meek. "Adversarial learning." Proceedings of the eleventh ACM SIGKDD international conference on Knowledge discovery in data mining. 2005. ![](https://img.shields.io/badge/type-theory-brightgreen.svg) 

#### Biggio, Battista, et al. "Evasion attacks against machine learning at test time." Joint European conference on machine learning and knowledge discovery in databases. Springer, Berlin, Heidelberg, 2013.

#### Szegedy, Christian, et al. "Intriguing properties of neural networks." arXiv preprint arXiv:1312.6199 (2013).

#### Goodfellow, Ian J., Jonathon Shlens, and Christian Szegedy. "Explaining and harnessing adversarial examples." arXiv preprint arXiv:1412.6572 (2014). ![](https://img.shields.io/badge/type-digital-brightgreen.svg) 
- The classic panda image with adversarial noise added to it to make a DNN misclassify the model
- Introduces the idea of gradient based PGD attack which is highly effective in white-box adversarial scenarios

#### Papernot, Nicolas, et al. "The limitations of deep learning in adversarial settings." 2016 IEEE European symposium on security and privacy (EuroS&P). IEEE, 2016. ![](https://img.shields.io/badge/type-digital-brightgreen.svg)  

#### Moosavi-Dezfooli, Seyed-Mohsen, Alhussein Fawzi, and Pascal Frossard. "Deepfool: a simple and accurate method to fool deep neural networks." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.

#### Papernot, Nicolas, et al. "Practical black-box attacks against machine learning." Proceedings of the 2017 ACM on Asia conference on computer and communications security. 2017. ![](https://img.shields.io/badge/type-digital-brightgreen.svg) 

- Precursor to Eykholt's physical attacks with stickers on traffic signs
- Introduces black-box attacks against Google's, Amazon's and MetaMind's DNN classification models
- Assumptions
  * No access to DNN structure and parameters
  * No access to large training dataset
  * Accses to only the output labels of the oracle model
- A synthetic dataset is constructed by the adversary to train a *substitute* model for the DNN classifier
- DNN is expected to misclassify inputs due to transferability with the *substitute* model

#### Carlini, Nicholas, and David Wagner. "Towards evaluating the robustness of neural networks." 2017 ieee symposium on security and privacy (sp). IEEE, 2017.

#### Carlini, Nicholas, and David Wagner. "Adversarial examples are not easily detected: Bypassing ten detection methods." Proceedings of the 10th ACM workshop on artificial intelligence and security. 2017.

#### Athalye, Anish, Nicholas Carlini, and David Wagner. "Obfuscated gradients give a false sense of security: Circumventing defenses to adversarial examples." International conference on machine learning. PMLR, 2018.

#### Ilyas, Andrew, et al. "Black-box adversarial attacks with limited queries and information." International Conference on Machine Learning. PMLR, 2018.
#### Carlini, Nicholas, et al. "On evaluating adversarial robustness." arXiv preprint arXiv:1902.06705 (2019).

---

### Physical Adversarial ML

#### Kurakin, Alexey, Ian Goodfellow, and Samy Bengio. "Adversarial examples in the physical world." (2016).

#### Sharif, Mahmood, et al. "Accessorize to a crime: Real and stealthy attacks on state-of-the-art face recognition." Proceedings of the 2016 acm sigsac conference on computer and communications security. 2016. ![](https://img.shields.io/badge/type-physical-brightgreen.svg) ![](https://img.shields.io/badge/sensor-camera-orange.svg)
- Attacks against facial recognition models that are physically realizable and inconspicuous
- They design adversarially painted eye glass frames that fool facial recognition models

#### Athalye, Anish, et al. "Synthesizing robust adversarial examples." International conference on machine learning. PMLR, 2018. ![](https://img.shields.io/badge/type-physical-brightgreen.svg) ![](https://img.shields.io/badge/sensor-camera-orange.svg) 
- Proposes *Expectation Over Transformation (EOT)* that produces robust adversarial examples that are simultaneously adversarial over an entire distribution of transformations
- This allows them to 3D print adversarial objects in which the object can be misclassified from various orientations

#### Eykholt, Kevin, et al. "Robust physical-world attacks on deep learning visual classification." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2018. ![](https://img.shields.io/badge/type-physical-brightgreen.svg) ![](https://img.shields.io/badge/sensor-camera-orange.svg)
- Proposes RP2 to generate physical perturbations in the form of stickers to fool DNN-based classifiers
- Cannonically known for misclassifying stop-signs by placing stickers on it
- Takes into consideration widely changing distances and angles of the viewing camera with respect to traffic signs
- They propose an evaluation method to study the effectiveness of physical perturbations
- 80-100% accuracy on various models attacked in stationary and drive-by testing datasets
- They do show the generalizability of the attack by attacking regular DNNs like Inception to misclassify objects like microwaves
- White-box attacks
- Focuses on *classifiers* and not *detectors*

#### Uesato, Jonathan, et al. "Adversarial risk and the dangers of evaluating against weak attacks." International Conference on Machine Learning. PMLR, 2018.

#### Zhao, Yue, et al. "Seeing isn't believing: Towards more robust adversarial attack against real world object detectors." Proceedings of the 2019 ACM SIGSAC Conference on Computer and Communications Security. 2019.

#### Boloor, Adith, et al. "Attacking vision-based perception in end-to-end autonomous driving models." Journal of Systems Architecture 110 (2020): 101766. ![simulated](https://img.shields.io/badge/type-simulated-brightgreen.svg "CARLA") ![](https://img.shields.io/badge/sensor-camera-orange.svg) 

#### Cao, Yulong, et al. "Adversarial sensor attack on lidar-based perception in autonomous driving." Proceedings of the 2019 ACM SIGSAC conference on computer and communications security. 2019. ![](https://img.shields.io/badge/type-simulated-brightgreen.svg) ![](https://img.shields.io/badge/sensor-LiDAR-orange.svg)

#### Cao, Yulong, et al. "Adversarial objects against lidar-based autonomous driving systems." arXiv preprint arXiv:1907.05418 (2019). ![](https://img.shields.io/badge/type-physical-brightgreen.svg) ![](https://img.shields.io/badge/sensor-LiDAR-orange.svg)

#### Yang, Kaichen, et al. "Robust Roadside Physical Adversarial Attack Against Deep Learning in Lidar Perception Modules." Proceedings of the 2021 ACM Asia Conference on Computer and Communications Security. 2021. ![](https://img.shields.io/badge/sensor-LiDAR-orange.svg)
- Builds upon Yulong Cao's works, with a focus on real-world realizability and defense discussion
- Attacks against [PointRCNN](https://openaccess.thecvf.com/content_CVPR_2019/html/Shi_PointRCNN_3D_Object_Proposal_Generation_and_Detection_From_Point_Cloud_CVPR_2019_paper.html) for white-box attacks and [PV-RCNN](https://openaccess.thecvf.com/content_CVPR_2020/html/Shi_PV-RCNN_Point-Voxel_Feature_Set_Abstraction_for_3D_Object_Detection_CVPR_2020_paper.html) for black box attacks

---

### Defense
#### Madry, Aleksander, et al. "Towards deep learning models resistant to adversarial attacks." arXiv preprint arXiv:1706.06083 (2017).
#### Wong, Eric, and Zico Kolter. "Provable defenses against adversarial examples via the convex outer adversarial polytope." International Conference on Machine Learning. PMLR, 2018.
#### Cohen, Jeremy, Elan Rosenfeld, and Zico Kolter. "Certified adversarial robustness via randomized smoothing." International Conference on Machine Learning. PMLR, 2019.
#### Wu, Tong, Liang Tong, and Yevgeniy Vorobeychik. "Defending against physically realizable attacks on image classification." arXiv preprint arXiv:1909.09552 (2019).

---

## Useful Resources

- [Adversarial Machine Learning Reading List by Nicholas Carlini](https://nicholas.carlini.com/writing/2018/adversarial-machine-learning-reading-list.html)
- [A Complete List of All (arXiv) Adversarial Example Papers by Nicholas Carlini](https://nicholas.carlini.com/writing/2019/all-adversarial-example-papers.html)

