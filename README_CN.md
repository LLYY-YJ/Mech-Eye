# Python 示例

本文档提供了用于Mech-Eye工业3D相机的Mech-Eye API Python示例描述，以及如何在Windows和Ubuntu上运行这些示例的说明。

如有任何问题或想要分享的内容，欢迎在 [Mech-Mind在线社区](https://community.mech-mind.com/) 发帖。社区还设有 [专门用于Mech-Eye SDK开发的版块](https://community.mech-mind.com/c/mech-eye-sdk-development/19)。

## 示例列表

示例分为以下几类：**基础**、**高级**和**工具**。

*   **基础** 示例：连接相机并采集数据。
*   **高级** 示例：以更复杂的方式采集数据并设置型号特定的参数。
*   **工具** 示例：获取相机信息和设置通用参数。

标记为 `(OpenCV)` 的示例需要安装OpenCV。

*   **基础**
    *   [connect_to_camera](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/basic/connect_to_camera.py)
        连接到相机。
    *   [connect_and_capture_images](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/basic/connect_and_capture_images.py)
        连接到相机并获取2D图像、深度图和点云数据。
    *   [capture_2d_image](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/basic/capture_2d_image.py) `(OpenCV)`
        获取并保存2D图像。
    *   [capture_depth_map](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/basic/capture_depth_map.py) `(OpenCV)`
        获取并保存深度图。
    *   [capture_point_cloud](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/basic/capture_point_cloud.py)
        获取并保存无纹理和有纹理的点云。
    *   [capture_point_cloud_hdr](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/basic/capture_point_cloud_hdr.py)
        设置多个曝光时间，然后获取并保存无纹理和有纹理的点云。
    *   [capture_point_cloud_with_normals](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/basic/capture_point_cloud_with_normals.py)
        计算法线并保存带有法线的无纹理和有纹理点云。
*   **高级**
    *   [convert_depth_map_to_point_cloud](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/convert_depth_map_to_point_cloud.py)
        从深度图生成点云并保存点云。
    *   [multiple_cameras_capture_sequentially](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/multiple_cameras_capture_sequentially.py) `(OpenCV)`
        从多个相机顺序获取并保存2D图像、深度图和点云。
    *   [multiple_cameras_capture_simultaneously](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/multiple_cameras_capture_simultaneously.py) `(OpenCV)`
        从多个相机同时获取并保存2D图像、深度图和点云。
    *   [capture_periodically](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/capture_periodically.py) `(OpenCV)`
        在指定持续时间内，从相机周期性地获取并保存2D图像、深度图和点云。
    *   [mapping_2d_image_to_depth_map](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/mapping_2d_image_to_depth_map.py)
        从带掩膜的2D图像和深度图生成无纹理和有纹理的点云。
    *   [render_depth_map](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/render_depth_map.py) `(OpenCV)`
        获取并保存使用jet配色方案渲染的深度图。
    *   [transform_point_cloud](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/Advanced/transform_point_cloud.py)
        获取并保存自定义参考系下的点云。
    *   [set_parameters_of_laser_cameras](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/set_parameters_of_laser_cameras.py)
        设置激光相机特定的参数。
    *   [set_parameters_of_uhp_cameras](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/set_parameters_of_uhp_cameras.py)
        设置UHP系列特定的参数。
    *   [register_camera_event](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/register_camera_event.py)
        定义并注册用于监视相机事件的回调函数。
    *   [capture_stereo_2d_images](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/advanced/capture_stereo_2d_images.py) `(OpenCV)`
        获取并保存两个2D相机的2D图像。
        > 注意：此示例仅适用于以下型号：Deep、Laser L Enhanced、PRO XS、LSR L、LSR S和DEEP。
*   **工具**
    *   [get_camera_intrinsics](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/util/get_camera_intrinsics.py)
        获取并打印相机内参。
    *   [print_camera_info](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/util/print_camera_info.py)
        获取并打印相机信息，例如型号、序列号、固件版本和温度。
    *   [set_scanning_parameters](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/util/set_scanning_parameters.py)
        设置**3D参数**、**2D参数**和**ROI**类别中的参数。
    *   [set_depth_range](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/util/set_depth_range.py)
        设置**深度范围**参数。
    *   [set_point_cloud_processing_parameters](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/util/set_point_cloud_processing_parameters.py)
        设置**点云处理**参数。
    *   [manage_user_sets](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/util/manage_user_sets.py)
        管理参数组，例如获取所有参数组的名称、添加参数组、切换参数组以及将参数设置保存到参数组。
    *   [save_and_load_user_set](https://github.com/MechMindRobotics/mecheye_python_samples/tree/master/area_scan_3d_camera/util/save_and_load_user_set.py)
        从JSON文件导入并替换所有参数组，并将所有参数组保存到JSON文件。

## 运行示例

### Windows

#### 先决条件

1.  确保安装的Python是64位版本，并且版本在3.7到3.11之间。
2.  请下载并安装下面列出的必需软件。

*   [Mech-Eye SDK (最新版本)](https://downloads.mech-mind.com/?tab=tab-sdk)
*   Python Mech-Eye API (最新版本)：

    ```python
    pip install MechEyeAPI
    ```

可选软件：如果您需要构建依赖于第三方软件的示例（请参考上面的示例列表），请安装相应的软件。

*   OpenCV (最新版本)：

    ```python
    pip install opencv-python
    ```

#### 操作说明

1.  导航到示例所在的文件夹。

    ```sh
    cd xxx/area_scan_3d_camera
    ```

2.  运行示例：将 ``sample_name`` 替换为示例的名称。

    ```python
    python sample_name.py
    ```

3.  输入您要连接的相机的索引，然后按Enter键。获取的文件将保存到示例所在的文件夹。

### Ubuntu

需要Ubuntu 18或更高版本。

#### 先决条件

*   安装 [Mech-Eye SDK (最新版本)](https://downloads.mech-mind.com/?tab=tab-sdk)。

    > 注意：如果之前安装过Mech-Eye SDK，请先使用以下命令卸载：
    >
    > ```bash
    > sudo dpkg -P MechEyeApi
    > ```

    *   如果系统架构是AMD64，执行以下命令：

        ```bash
        sudo dpkg -i 'Mech-Eye_API_x.x.x_amd64.deb'
        ```

    *   如果系统架构是ARM64，执行以下命令：

        ```bash
        sudo dpkg -i 'Mech-Eye_API_x.x.x_arm64.deb'
        ```

*   升级g++，确保其版本为12或更高。

    a. 安装较新版本的g++（以g++ 13为例）：

       ```bash
       sudo add-apt-repository ppa:ubuntu-toolchain-r/test
       sudo apt-get update
       sudo apt install g++-13
       ```

    b. 使用 `ls` 命令检查已安装的g++版本：

       ```bash
       ls usr/bin/g++*
       ```

    c. 将所有已安装的g++版本添加为备选项（以g++ 9和g++ 13为例）：

       ```bash
       sudo update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-9 10
       sudo update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-13 20
       ```

    d. 选择g++版本。输入与较新版本g++对应的数字以选择该版本。

       ```bash
       sudo update-alternatives --config g++
       ```

    e. 检查是否成功选择了较新版本的g++：

       ```bash
       g++ --version
       ```

*   安装Python Mech-Eye API：

    ```bash
    sudo pip3 install MechEyeApi
    ```

*   （可选）如果需要构建依赖于OpenCV的示例（请参考上面的示例列表），请安装OpenCV：

    ```bash
    sudo apt-get install libopencv-dev
    sudo apt-get install python3-opencv
    ```

#### 操作说明

1.  导航到示例所在的文件夹。

    ```bash
    cd xxx/area_scan_3d_camera
    ```

2.  运行示例：将 ``sample_name`` 替换为示例的名称。

    ```python
    sudo python3 sample_name.py
    ```

3.  输入您要连接的相机的索引，然后按Enter键。获取的文件将保存到示例所在的文件夹。