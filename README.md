# 3D-Wireframe-Generation-Survey

三维线框生成的研究发展与综述



### 常用的点云特征提取backbone

|                   预览                    | 论文名称                                                     | 发表期刊/会议 |                        相关链接                        |
| :---------------------------------------: | :----------------------------------------------------------- | :-----------: | :----------------------------------------------------: |
| <img src="img/pointnet.png" width="300">  | [Pointnet: Deep learning on point sets for 3d classification and segmentation](http://openaccess.thecvf.com/content_cvpr_2017/html/Qi_PointNet_Deep_Learning_CVPR_2017_paper.html) |   CVPR 2017   |     [Code](https://github.com/charlesq34/pointnet)     |
| <img src="img/pointnet2.jpg" width="300"> | [Pointnet++: Deep hierarchical feature learning on point sets in a metric space](https://proceedings.neurips.cc/paper/2017/hash/d8bf84be3800d12f74d8b05e9b89836f-Abstract.html) |   NIPS 2017   |    [Code](https://github.com/charlesq34/pointnet2)     |
|   <img src="img/DGCNN.png" width="300">   | [Dynamic graph cnn for learning on point clouds](https://dl.acm.org/doi/abs/10.1145/3326362) |   TOG 2019    | [Code](https://github.com/WangYueFt/dgcnn/tree/master) |
| <img src="img/pointcept.png" width="300"> | Pointcept                                                    |   Codebase    |     [Code](https://github.com/Pointcept/Pointcept)     |

### 常用数据集

|                    预览                    | 论文名称                                                     | 发表期刊/会议 |                        相关链接                         |
| :----------------------------------------: | :----------------------------------------------------------- | :-----------: | :-----------------------------------------------------: |
|    <img src="img/ABC.png" width="300">     | [Abc: A big cad model dataset for geometric deep learning](http://openaccess.thecvf.com/content_CVPR_2019/html/Koch_ABC_A_Big_CAD_Model_Dataset_for_Geometric_Deep_Learning_CVPR_2019_paper.html) |   CVPR 2019   | [Project](https://deep-geometry.github.io/abc-dataset/) |
| <img src="img/Building3D.png" width="300"> | [Building3d: A urban-scale dataset and benchmarks for learning roof structures from point clouds](http://openaccess.thecvf.com/content/ICCV2023/html/Wang_Building3D_A_Urban-Scale_Dataset_and_Benchmarks_for_Learning_Roof_Structures_ICCV_2023_paper.html) |   ICCV 2023   |       [Project](https://building3d.ucalgary.ca/)        |
| <img src="img/Semantic3d.png" width="300"> | [Semantic3d. net: A new large-scale point cloud classification benchmark](https://arxiv.org/abs/1704.03847) |  arXiv 2017   |                [Project](semantic3d.net)                |
|    <img src="img/DTU.png" width="300">     | [Large-scale data for multiple-view stereopsis](https://link.springer.com/article/10.1007/s11263-016-0902-9) |   IJCV 2016   |    [Project](https://roboimagedata.compute.dtu.dk/)     |
| <img src="img/blendedmvs.png" width="300"> | [Blendedmvs: A large-scale dataset for generalized multi-view stereo networks](http://openaccess.thecvf.com/content_CVPR_2020/html/Yao_BlendedMVS_A_Large-Scale_Dataset_for_Generalized_Multi-View_Stereo_Networks_CVPR_2020_paper.html) |   CVPR 2020   |    [Project](https://github.com/YoYo000/BlendedMVS)     |
|  <img src="img/ABC-NEF.png" width="300">   | [Nef: Neural edge fields for 3d parametric curve reconstruction from multi-view images](http://openaccess.thecvf.com/content/CVPR2023/html/Ye_NEF_Neural_Edge_Fields_for_3D_Parametric_Curve_Reconstruction_From_CVPR_2023_paper.html) |   CVPR 2023   |      [Project](https://yunfan1202.github.io/NEF/)       |

### 一、基于网格的三维线框生成方法

#### 1.1 基于曲率估计的谷脊线检测

1. [Solid shape](https://mitpress.mit.edu/9780262111393/)
2. [Ridge curves and shape analysis](https://www.bmva-archive.org.uk/bmvc/1996/kent_1.pdf)
3. [Extraction of feature lines on triangulated surfaces using morphological operators](https://aaai.org/papers/0012-SS00-04-012-extraction-of-feature-lines-on-triangulated-surfaces-using-morphological-operators/)
4. [Detection of salient curvature features on polygonal surfaces](https://onlinelibrary.wiley.com/doi/full/10.1111/1467-8659.00531)
5. [Normal vector voting: crease detection and curvature estimation on large, noisy meshes](https://www.sciencedirect.com/science/article/pii/S1524070302905746)
6. [The implicit structure of ridges of a smooth parametric surface](https://www.sciencedirect.com/science/article/pii/S0167839606000410)
7. [Ridge-valley lines on meshes via implicit surface fitting](https://dl.acm.org/doi/10.1145/1015706.1015768)
8. [Fast and Robust Detection of Crest Lines on Meshes](https://www2.riken.jp/brict/Yoshizawa/Papers/spm05ybs.pdf)
9. [Smooth Feature Lines on Surface Meshes](https://diglib.eg.org/items/860abe10-40fd-4436-bae1-7db8f05df494)
10. [Estimating Curvatures and Their Derivatives on Triangle Meshes](https://gfx.cs.princeton.edu/pubs/Rusinkiewicz_2004_ECA/curvpaper.pdf)
11. [Functional Optimization for Fair Surface Design](https://people.eecs.berkeley.edu/~sequin/CS284/TEXT/p167-moreton.pdf)
12. [Large Deformable Splines, Crest Lines and Matching](https://ieeexplore.ieee.org/abstract/document/378150)
13. [Finding Ridges and Valleys in a Discrete Surface Using a Modified MLS Approximation](https://www.sciencedirect.com/science/article/abs/pii/S0010448505001806)
14. [Fast, Robust, and Faithful Methods for Detecting Crest Lines on Meshes](https://www.sciencedirect.com/science/article/pii/S0167839608000435)
15. [Separatrix Persistence: Extraction of Salient Edges on Surfaces Using Topological Methods](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1467-8659.2009.01528.x)
16. [Feature Detection of Triangular Meshes Based on Tensor Voting Theory](https://www.sciencedirect.com/science/article/abs/pii/S0010448508002297)
17. [Demarcating Curves for Shape Illustration](https://dl.acm.org/doi/abs/10.1145/1457515.1409110)
18. [Thin nets and crest lines: Application to satellite data and medical images](https://www.sciencedirect.com/science/article/pii/S107731429690507X)
19. [The 3D marching lines algorithm](https://www.sciencedirect.com/science/article/pii/S1077316996900428)
20. [Extracting line representations of sulcal and gyral patterns in MR images of the human brain](https://ieeexplore.ieee.org/abstract/document/746714/)
21. [Using a statistical shape model to extract sulcal curves on the outer cortex of the human brain](https://ieeexplore.ieee.org/abstract/document/1009387/)
22. [Crest lines for surface segmentation and flattening](https://dl.acm.org/doi/abs/10.1109/TVCG.2004.24)
23. [Learning line features in 3D geometry](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1467-8659.2011.01858.x)
24. [Feature curve co-completion in noisy data](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.13337)

#### 1.2 基于网格分割的特征曲线检测

1. [A general and efficient method for finding cycles in 3D curve networks](https://dl.acm.org/doi/10.1145/2508363.2508423)
2. [Flow aligned surfacing of curve networks](https://dl.acm.org/doi/10.1145/2766990)
3. [FlowRep: Descriptive curve networks for free-form design shapes](https://dl.acm.org/doi/10.1145/3072959.3073639)
4. [Cassie: Curve and surface sketching in immersive environments](https://dl.acm.org/doi/10.1145/3411764.3445158)
5. [Strokes2Surface: Recovering curve networks from 4D architectural design sketches](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.15054)
6. [Fibermesh: Designing freeform surfaces with 3D curves](https://dl.acm.org/doi/10.1145/1276377.1276429)
7. [Segmentation through variable-order surface fitting](https://www.cs.hunter.cuny.edu/~ioannis/3DP_F03/PAPERS/SEGMENTATION/besl_jain.pdf)
8. [High-level CAD model acquisition from range images](https://www.sciencedirect.com/science/article/pii/S0010448596000590)
9. [Variational shape approximation](https://dl.acm.org/doi/abs/10.1145/1186562.1015817)
10. [Structure Recovery via Hybrid Variational Surface Approximation](https://www.graphics.rwth-aachen.de/publication/87/hybrid1.pdf)
11. [Quadric surface extraction by variational shape approximation](https://link.springer.com/chapter/10.1007/11802914_6)
12. [Variational mesh segmentation via quadric surface fitting](https://www.sciencedirect.com/science/article/pii/S0010448512000887)
13. [Interactive segmentation of scanned mechanical models based on quadratic surfaces fitting](https://www.jcad.cn/en/article/doi/10.3724/SP.J.1089.2019.17508)
14. [Extraction and remeshing of ellipsoidal representations from mesh data](https://www.cs.toronto.edu/~psimari/publications/2005_gi_simari_singh.pdf)
15. [D-Charts: Quasi-Developable Mesh Segmentation](https://openurl.ebsco.com/EPDB%3Agcd%3A11%3A23907611/detailv2?sid=ebsco%3Aplink%3Ascholar-a&id=ebsco%3Agcd%3A18272051&crl=c&jrnl=01677055&id_token_hint=eyJraWQiOiIxNjg2MTQ5MjEzNjMxIiwiYWxnIjoiUlMyNTYifQ.eyJzdWIiOiJzMzg5NDEzMC5tYWluIiwiZGV2aWNlX2lkIjoiNTUxNjQ3OTItY2FlZC00OGIwLTg2MTMtZjJlYjI5ZGJkY2VlIiwiYW1yIjpbImlwIl0sImlzcyI6Imh0dHBzOlwvXC9hdXRoLmVic2NvLnpvbmVcL2FwaVwvZGlzcGF0Y2hlciIsImNsaWVudF9pZCI6ImF3Z3ljSXg1N01yd25EUTVoNFVlNnlDVkVQMHI1TXQ5IiwiYXVkIjpbImh0dHBzOlwvXC9hdXRoLmVic2NvLnpvbmVcL2FwaVwvZGlzcGF0Y2hlciIsImh0dHA6XC9cL2F1dGgtY3h0LW1nci5laG9zdC1saXZlLmVrcy5laG9zdC1saXZlLmVpc2x6LmNvbSIsImh0dHBzOlwvXC9hY2Nlc3MtYXBpLmVic2NvLmNvbSIsImF3Z3ljSXg1N01yd25EUTVoNFVlNnlDVkVQMHI1TXQ5Il0sImF6cCI6ImF3Z3ljSXg1N01yd25EUTVoNFVlNnlDVkVQMHI1TXQ5IiwiaWR0IjoiaW5zdGl0dXRpb25hbCIsImV4cCI6MTc2MDYyODUwMSwiaWF0IjoxNzYwNjI0OTAxLCJjbGllbnRfbmFtZSI6IldlYmF1dGggLSBOZXcgRURTIGlkX3Rva2VuIiwianRpIjoiYjMwOTY2N2UtOWZhYS00ODRiLWI3ZDQtYjg1ZjA4Mzc4ZWQ0IiwidXNlcm5hbWUiOiJJbnN0aXR1dGlvbmFsVXNlciJ9.SU685yBYb62AweEc8810G9HOvFBnBnPZirmIY-D1zDi3HwX29Jo0qR1BhQORU-hSEpf5c98er4cm6bW0wFmLBUYA2GQvzWBu4yHGzbbOc56-QAu8KodMuwfh-yPqCoF3s7nVe4h2ANROchYL6OLf9_5K6H8BLb90yw_k01BfCpSyLmN11_YLkigZbx3jSILy-hsaXqJhnt_B3s58Nf-LU_L87x3nYwvPdgN0ItTQfJZfW66xCunxVVi4fYkPhPTjBhsHkzDMjXRwOAMzQ-zsxdT3gjNE9LLjrF4Y2PkiRDoYYHonuSoZvlgpOBUD8fhPFcBJytL3jeEWR8bD6DSj1g&link_origin=scholar.google.com.hk)
16. [Blending surface segmentation and editing for 3D models](https://ieeexplore.ieee.org/abstract/document/9296787)
17. [Hierarchical mesh segmentation based on fitting primitives](https://link.springer.com/article/10.1007/s00371-006-0375-x)
18. [Hierarchical mesh decomposition using fuzzy clustering and cuts](https://dl.acm.org/doi/abs/10.1145/882262.882369)
19. [A new CAD mesh segmentation method, based on curvature tensor analysis](https://www.sciencedirect.com/science/article/pii/S0010448504002003)
20. [Abstraction of man-made shapes](https://dl.acm.org/doi/abs/10.1145/1661412.1618483)
21. [Adapting feature curve networks to a prescribed scale](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.12834)
22. [iWIRES: An analyze-and-edit approach to shape manipulation](https://dl.acm.org/doi/abs/10.1145/1576246.1531339)
23. [Exoskeleton: Curve network abstraction for 3D shapes](https://www.sciencedirect.com/science/article/pii/S0097849310001810)
24. [Recognition of feature curves on 3D shapes using an algebraic approach to Hough transforms](https://www.sciencedirect.com/science/article/pii/S0031320317303096)
25. [Patch layout generation by detecting feature networks](https://www.sciencedirect.com/science/article/pii/S0097849314001101)
26. [Extracting cycle-aware feature curve networks from 3D models](https://www.sciencedirect.com/science/article/pii/S0010448520301421)
27. [Feature-aligned segmentation using correlation clustering](https://ieeexplore.ieee.org/abstract/document/10897514)
28. [Seg-mat: 3D shape segmentation using medial axis transform](https://ieeexplore.ieee.org/abstract/document/9234096)
29. [3D Shape Segmentation with Potential Consistency Mining and Enhancement](https://ieeexplore.ieee.org/abstract/document/10814983)
30. [Patch layout from feature graphs](https://www.sciencedirect.com/science/article/pii/S0010448509002851)
31. [Extract feature curves on noisy triangular meshes](https://www.sciencedirect.com/science/article/pii/S1524070317300498)

### 二、基于点云的三维线框生成方法

#### 2.1 基于几何分析的尖锐特征检测

1. [Feature Extraction From Point Clouds](https://www.researchgate.net/profile/Stefan-Gumhold/publication/2554207_Feature_Extraction_from_Point_Clouds/links/0deec522ee1463f801000000/Feature-Extraction-from-Point-Clouds.pdf)
2. [Multi‐scale feature extraction on point‐sampled surfaces](https://onlinelibrary.wiley.com/doi/abs/10.1111/1467-8659.00675)
3. [Spline-based feature curves from point-sampled geometry](https://link.springer.com/article/10.1007/s00371-008-0223-2)
4. [Feature preserving mesh generation from 3D point clouds](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1467-8659.2010.01771.x)
5. [Sharp feature preserving MLS surface reconstruction based on local feature line approximations](https://www.sciencedirect.com/science/article/pii/S152407031200032X)
6. [Sharp feature detection in point clouds](https://ieeexplore.ieee.org/abstract/document/5521460/)
7. [Fast and robust edge extraction in unorganized point clouds](https://ieeexplore.ieee.org/abstract/document/7371262/)
8. [Feature‐preserving reconstruction of singular surfaces](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1467-8659.2012.03183.x)
9. [Robust moving least-squares fitting with sharp features](https://dl.acm.org/doi/abs/10.1145/1073204.1073227)
10. [Data-dependent MLS for faithful surface approximation](https://dl.acm.org/doi/abs/10.5555/1281991.1281999)
11. [Voronoi-based feature curves extraction for sampled singular surfaces](https://www.sciencedirect.com/science/article/pii/S0097849313000885)
12. [Patch-graph reconstruction for piecewise smooth surfaces](https://www.google.com/books?hl=zh-CN&lr=&id=WCVFWYlAeCMC&oi=fnd&pg=PA3&dq=Patch-graph+reconstruction+for+piecewise+smooth+surfaces&ots=QDKiVh40M-&sig=J6VqqWfIGI9zdC067UGE6uCBfrs)
13. [Feature preserving point set surfaces based on non‐linear kernel regression](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1467-8659.2009.01388.x)
14. [Multi-scale tensor voting for feature extraction from unstructured point clouds](https://www.sciencedirect.com/science/article/pii/S1524070312000288)
15. [A feature-preserving framework for point cloud denoising](https://www.sciencedirect.com/science/article/pii/S0010448520300506)
16. [Voronoi-based curvature and feature estimation from point clouds](https://ieeexplore.ieee.org/abstract/document/5669298/)
17. [SGLBP: Subgraph‐based local binary patterns for feature extraction on point clouds](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.14500)
18. [Extracting feature lines from point clouds based on smooth shrink and iterative thinning](https://www.sciencedirect.com/science/article/pii/S1524070316300054)
19. [Neighbor reweighted local centroid for geometric feature identification](https://ieeexplore.ieee.org/abstract/document/9600876/)
20. [An adaptive normal estimation method for scanned point clouds with sharp features](https://www.sciencedirect.com/science/article/pii/S0010448513001000)
21. [A statistical approach for extraction of feature lines from point clouds](https://www.sciencedirect.com/science/article/pii/S0097849316300097)
22. [Edge and corner detection for unorganized 3d point clouds with application to robotic welding](https://ieeexplore.ieee.org/abstract/document/8593910/)
23. [Multiscale feature line extraction from raw point clouds based on local surface variation and anisotropic contraction](https://ieeexplore.ieee.org/abstract/document/9351738/)
24. [Rfeps: Reconstructing feature-line equipped polygonal surface](https://dl.acm.org/doi/abs/10.1145/3550454.3555443)

#### 2.2 基于深度学习的CAD模型三维线框生成

1. [Contour detection in unstructured 3D point clouds](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Hackel_Contour_Detection_in_CVPR_2016_paper.html)
2. [Edge-aware point set resampling](https://dl.acm.org/doi/abs/10.1145/2421636.2421645)
3. [Ec-net: an edge-aware point set consolidation network](http://openaccess.thecvf.com/content_ECCV_2018/html/Lequan_Yu_EC-Net_an_Edge-aware_ECCV_2018_paper.html)
4. [Learning part boundaries from 3D point clouds](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.14078)
5. [Def: Deep estimation of sharp geometric features in 3d shapes](https://par.nsf.gov/biblio/10357187)
6. [MSL-Net: Sharp feature detection network for 3D point clouds](https://ieeexplore.ieee.org/abstract/document/10373950/)
7. [Complexgen: Cad reconstruction by b-rep chain complex generation](https://dl.acm.org/doi/abs/10.1145/3528223.3530078)
8. [Surface and edge detection for primitive fitting of point clouds](https://dl.acm.org/doi/abs/10.1145/3588432.3591522)
9. [Brepgen: A b-rep generative diffusion model with structured latent geometry](https://dl.acm.org/doi/abs/10.1145/3658129)
10. [Split-and-fit: Learning b-reps via structure-aware voronoi partitioning](https://dl.acm.org/doi/abs/10.1145/3658155)
11. [Hola: B-rep generation using a holistic latent representation](https://dl.acm.org/doi/abs/10.1145/3730842)
12. [Sharp feature consolidation from raw 3D point clouds via displacement learning](https://www.sciencedirect.com/science/article/pii/S0167839623000365)
13. [Sepicnet: Sharp edges recovery by parametric inference of curves in 3d shapes](https://openaccess.thecvf.com/content/CVPR2023W/StruCo3D/html/Cherenkova_SepicNet_Sharp_Edges_Recovery_by_Parametric_Inference_of_Curves_in_CVPRW_2023_paper.html)
14. [Thin-walled aircraft panel edge extraction from 3-D measurement surfaces via feature-aware displacement learning](https://ieeexplore.ieee.org/abstract/document/10458949/)
15. [STAR-Edge: Structure-aware Local Spherical Curve Representation for Thin-walled Edge Extraction from Unstructured Point Clouds](https://openaccess.thecvf.com/content/CVPR2025/html/Li_STAR-Edge_Structure-aware_Local_Spherical_Curve_Representation_for_Thin-walled_Edge_Extraction_CVPR_2025_paper.html)
16. [Sketch2cad: Sequential cad modeling by sketching in context](https://dl.acm.org/doi/abs/10.1145/3414685.3417807)
17. [Free2cad: Parsing freehand drawings into cad commands](https://dl.acm.org/doi/abs/10.1145/3528223.3530133)
18. [Pie-net: Parametric inference of point cloud edges](https://proceedings.neurips.cc/paper/2020/hash/e94550c93cd70fe748e6982b3439ad3b-Abstract.html)
19. [Pc2wf: 3d wireframe reconstruction from raw point clouds](https://arxiv.org/abs/2103.02766)
20. [Coarse-to-fine pipeline for 3D wireframe reconstruction from point cloud](https://www.sciencedirect.com/science/article/pii/S0097849322001194)
21. [WireframeNet: A novel method for wireframe generation from point cloud](https://www.sciencedirect.com/science/article/pii/S0097849323001449)
22. [EDWG: Efficient Edge Detection and Wireframe Generation from Point Clouds](https://ieeexplore.ieee.org/abstract/document/11005571/)
23. [Nerve: Neural volumetric edges for parametric curve extraction from point cloud](http://openaccess.thecvf.com/content/CVPR2023/html/Zhu_NerVE_Neural_Volumetric_Edges_for_Parametric_Curve_Extraction_From_Point_CVPR_2023_paper.html)
24. [Deep Point Cloud Edge Reconstruction Via Surface Patch Segmentation](https://ieeexplore.ieee.org/abstract/document/10909144/)
25. [Generating 3D House Wireframes with Semantics](https://link.springer.com/chapter/10.1007/978-3-031-72670-5_13)
26. [Clr-wire: Towards continuous latent representations for 3d curve wireframe generation](https://dl.acm.org/doi/abs/10.1145/3721238.3730638)

