# Robust and Efficient Visual-Inertial Odometry with Multi-plane Priors

This repository contains the implementation for the corresponding paper.

## How to use

For compilation:

* Install the dependencies: Eigen, Ceres Solver and OpenCV.
* Clone the repository.
* Build with `mkdir -p build && cd build && cmake -DCMAKE_BUILD_TYPE=Release  .. && make -j8`, you will need a compiler supporting C++17.
* Tested in Ubuntu 18.04 (with GCC 9.0 and CMake 3.11), and macOS 10.14.

For execution:
* `./roam-pc [data_scheme]://[data_path] [config_yaml_path]`
  * e.g. 
    * For EuRoC Dataset: `build/roam-pc/roam-pc euroc:///Data/EuRoC/V1_01_easy/mav0 config/euroc.yaml`
    * For TUM-VI Dataset: `build/roam-pc/roam-pc tum:///Data/TUM_VI/dataset-room1_512_16/mav0 config/tum_vi.yaml`
* The trajectory will be written in `trajectory.tum`.

## Publication

If you used our work, please kindly cite the following paper.

> **Robust and Efficient Visual-Inertial Odometry with Multi-plane Priors**, Jinyu LiBangbang YangKai HuangGuofeng ZhangHujun Bao, Chinese Conference on Pattern Recognition and Computer Vision (PRCV). Springer, Cham, 2019: 283-295.

## Caveats

* For commercial inquiries, please contact Guofeng Zhang <zhangguofeng(AT)cad.zju.edu.cn>.

## Acknowledgement

This work is affliated with ZJU-SenseTime Joint Lab of 3D Vision, and its intellectual property belongs to SenseTime Group Ltd.

```
Copyright SenseTime. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
