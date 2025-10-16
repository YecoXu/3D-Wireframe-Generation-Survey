# 3D-Wireframe-Generation-Survey

三维线框生成的研究发展与综述



### 常用的点云特征提取backbone

|                   预览                    | 论文名称                                                     | 发表期刊/会议 |                        相关链接                        |
| :---------------------------------------: | :----------------------------------------------------------- | :-----------: | :----------------------------------------------------: |
| <img src="img/pointnet.png" width="300">  | [Pointnet: Deep learning on point sets for 3d classification and segmentation](http://openaccess.thecvf.com/content_cvpr_2017/html/Qi_PointNet_Deep_Learning_CVPR_2017_paper.html) |   CVPR 2017   |     [Code](https://github.com/charlesq34/pointnet)     |
| <img src="img/pointnet2.jpg" width="300"> | [Pointnet++: Deep hierarchical feature learning on point sets in a metric space](https://proceedings.neurips.cc/paper/2017/hash/d8bf84be3800d12f74d8b05e9b89836f-Abstract.html) |   NIPS 2017   |    [Code](https://github.com/charlesq34/pointnet2)     |
|   <img src="img/DGCNN.png" width="300">   | [Dynamic graph cnn for learning on point clouds](https://dl.acm.org/doi/abs/10.1145/3326362) |   TOG 2019    | [Code](https://github.com/WangYueFt/dgcnn/tree/master) |
| <img src="img/pointcept.png" width="300"> | Pointcept                                                    |   Codebase    |     [Code](https://github.com/Pointcept/Pointcept)     |

### 数据集

| 类别               |                    预览                    | 论文名称                                                     | 发表期刊/会议 |                        相关链接                         |
| ------------------ | :----------------------------------------: | :----------------------------------------------------------- | :-----------: | :-----------------------------------------------------: |
| CAD数据集          |    <img src="img/ABC.png" width="300">     | [Abc: A big cad model dataset for geometric deep learning](http://openaccess.thecvf.com/content_CVPR_2019/html/Koch_ABC_A_Big_CAD_Model_Dataset_for_Geometric_Deep_Learning_CVPR_2019_paper.html) |   CVPR 2019   | [Project](https://deep-geometry.github.io/abc-dataset/) |
| 三维测量点云数据集 | <img src="img/Building3D.png" width="300"> | [Building3d: A urban-scale dataset and benchmarks for learning roof structures from point clouds](http://openaccess.thecvf.com/content/ICCV2023/html/Wang_Building3D_A_Urban-Scale_Dataset_and_Benchmarks_for_Learning_Roof_Structures_ICCV_2023_paper.html) |   ICCV 2023   |       [Project](https://building3d.ucalgary.ca/)        |
| 三维测量点云数据集 | <img src="img/Semantic3d.png" width="300"> | [[Semantic3d. net: A new large-scale point cloud classification benchmark](https://arxiv.org/abs/1704.03847)](https://dl.acm.org/doi/abs/10.1145/3326362) |  arXiv 2017   |                [Project](semantic3d.net)                |
| 多视图数据集       |    <img src="img/DTU.png" width="300">     | [Large-scale data for multiple-view stereopsis](https://link.springer.com/article/10.1007/s11263-016-0902-9) |   IJCV 2016   |    [Project](https://roboimagedata.compute.dtu.dk/)     |
| 多视图数据集       | <img src="img/blendedmvs.png" width="300"> | [Blendedmvs: A large-scale dataset for generalized multi-view stereo networks](http://openaccess.thecvf.com/content_CVPR_2020/html/Yao_BlendedMVS_A_Large-Scale_Dataset_for_Generalized_Multi-View_Stereo_Networks_CVPR_2020_paper.html) |   CVPR 2020   |    [Project](https://github.com/YoYo000/BlendedMVS)     |
| 多视图数据集       |  <img src="img/ABC-NEF.png" width="300">   | [Nef: Neural edge fields for 3d parametric curve reconstruction from multi-view images](http://openaccess.thecvf.com/content/CVPR2023/html/Ye_NEF_Neural_Edge_Fields_for_3D_Parametric_Curve_Reconstruction_From_CVPR_2023_paper.html) |   CVPR 2023   |      [Project](https://yunfan1202.github.io/NEF/)       |