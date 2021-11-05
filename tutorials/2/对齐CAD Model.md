### 对齐CAD Model

* [1] 得到watertight的model
* [2] 调整模型比例至真实尺寸
* [3] 对模型做平移，使其几何中心位于世界坐标系原点
* [4] 对模型做旋转

### [1]

工具链接：https://github.com/hjwdzh/Manifold

### [2~4]

工具：MeshLab或CloudCompare

#### MeshLab

如需简化模型：Filters->Remeshing, Simplification and Reconstruction->若干Simplification方法

[2] 根据对物体的真实测量结果，在MeshLab里选定两点并测量距离（单位m），并放缩模型

[3] Filters->Normals, Curvatures and Orientation->Transform: Translate, Center, set Origin->Center or Scene BBox

[4] Filters->Normals, Curvatures and Orientation->Transform: Rotate