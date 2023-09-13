
### Using group-equivariant deep-learning to determine the chirality of spiral galaxies

*The angular momentum of nearby galaxies may be sensitive to the initial conditions of the universe, but determining the spin direction of all the galaxies 
in modern optical surveys requires the development of new efficient algorithms. In this project the student(s) will design and implement a deep-learning 
classifier for separating S-wise (clockwise) and Z-wise (anti-clockwise) spirals. In particular this project will investigate the impact of using convolutions 
that are equivariant to chirality in their deep-learning model and evaluate the potential biases that arise from the choice of such convolutions. This project 
will use the python PyTorch library. Students are expected to be proficient in python, but not necessarily to have any prior knowledge of deep-learning.*

---

### Work Plan

1. Cross-match the original Galaxy Zoo catalogue (S/Z labels) with the GZ3D catalogue (spiral arm masks) and the DESI catalogue (optical images);
2. Build a model to classify the images from DESI according to their S/Z labels from GZ:
       - Option 1 [clean slate approach]: Build a simple classifier from scratch using a LeNET architecture (or similar);
       - Option 2 [foundation model approach]: Finetune the zoobot classifier;
4. Investigate the performance improvement from including spiral arm masks from GZ3D as inputs;
5. Adapt the model to incorporate group equivariant convolutions, enforcing rotational or reflectional equivariance; 
6. Examine performance differences for different types of equivariance;
7. Discuss and explain results.

### Potential outputs

1. Chirality predictions for the full DESI catalogue;
2. Chriality analysis for DESI [this is quite a bit of work - could be a second semester project]

<!---
#### Potential publications

* [MNRAS (or similar) astronomy paper on uncertainty calibration in FR classification](https://www.overleaf.com/4756255635rdcxgzpvbkbq)
* NIPS (or similar) workshop paper on uncertainty calibration as a function of equivariance
--->

#### Useful Links

* [GZ3D dataset](https://www.sdss4.org/dr17/data_access/value-added-catalogs/?vac_id=galaxy-zoo-3d)
* [ZooBot Model](https://github.com/mwalmsley/zoobot)
