# OpenPose_Drown
Only for national Chin-Yi University of technology

# 1. Prepare
**Devices**:
1. Ubuntu 16.04 LTS
2. Memory: 15.6 GiB
3. Processor: Intel® Core™ i5-9400F CPU @ 2.90GHz × 6
4. Graphics : GeForce RTX 2080/PCIe/SSE2
5. Os Type: 64-bit

**Dependency**:
1. Cuda compilation tools, release 10.0, V10.0.130
2. Cudnn : 7.4.2
3. Python : 3.6.12

Check Cuda Version:
```bash
nvcc -V
```
Check Cuda Version:
```bash
cat /usr/local/cuda/include/cudnn.h | grep CUDNN_MAJOR -A 2
or
cat /usr/include/cudnn.h | grep CUDNN_MAJOR -A 2
```

# 2. 

# Reference:
1. [Chenge Yang, Zhicheng Yu, Feiyu Chen, "Human Pose Estimation Benchmarking and Action Recognition," Deep Learning Project, Winter 2019, Northwestern University, 26-Oct-2019.](https://github.com/ChengeYang/Human-Pose-Estimation-Benchmarking-and-Action-Recognition)
2. [Feiyu Chen, "Human-Pose-Estimation-Benchmarking-and-Action-Recognition,"Deep Learning Project, Winter 2019, Northwestern University, 26-Oct-2019.](https://github.com/felixchenfy/Realtime-Action-Recognition)
