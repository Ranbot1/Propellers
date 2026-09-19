# Propellers · Interactive 3D Tutorial

一个面向无人机螺旋桨初学者的三维交互式科普网页。目标不是先讲公式，而是先让术语和真实实体建立一一对应关系。

## 在线查看

GitHub Pages（部署成功后）：

**https://ranbot1.github.io/Propellers/**

如果 Pages 尚未在仓库设置中启用，可先直接打开 `index.html` 查看源码；站点本身是纯静态单文件，不需要构建、npm 或本地依赖。

## 第一部分：螺旋桨基础概念

当前版本包含：

- Blade / 桨叶
- Hub / 桨毂
- Root / 桨根
- Tip / 桨尖
- Leading edge / 前缘
- Trailing edge / 后缘
- Chord / 弦与弦长
- Airfoil section / 翼型截面
- Twist / 扭转
- Pitch / 桨距
- Sweep / 后掠
- Dihedral / Anhedral / 上反与下反
- Rotation plane / 旋转平面
- Pressure / suction surface / 压力面与吸力面
- Duct / shroud / 涵道

### 交互

- 点击左侧术语：高亮三维模型中的对应实体
- 直接点击模型：反向选择概念
- 鼠标拖动旋转、滚轮缩放、右键平移
- 俯视 / 侧视快捷视角
- 教学爆炸图：分开桨毂和两片桨叶，并显示多个翼型截面
- 自动旋转
- 后掠、上反/下反、桨距、涵道都有独立辅助几何

## 几何说明

网页中的桨叶是用多个 NACA 风格厚度截面程序化放样得到的教学模型，并加入：

- 径向弦长变化 `c(r)`
- 径向扭转 `θ(r)`
- 外段后掠
- 外段轻微上反
- 四分之一弦附近的积叠逻辑

它**不是任何一款 DJI 产品的精确逆向模型**，用于建立空间概念。

## 参考资料

- NASA OpenVSP — Propellers: https://www.nasa.gov/reference/openvsp-propellers/
- NASA Glenn — Propeller Thrust: https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/propeller-thrust/
- Virginia Tech — Ducted Fans: https://archive.aoe.vt.edu/mason/Mason_f/DuctedFans.pdf

## 后续建议

第二部分可继续加入“气流与噪声”：

1. 用粒子/流线显示相对来流与下洗
2. 可视化 pressure / suction side 压力差
3. 动画显示 tip vortex
4. 对比普通桨尖、后掠桨尖、上反/下反桨尖
5. 加入 BPF、loading noise、thickness noise、trailing-edge noise 的声源位置
6. 导入你后续重建的大疆专利桨几何做对照
