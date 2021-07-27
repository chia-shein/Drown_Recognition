# OpenPose_Drown
Only for national Chin-Yi University of technology

# 1. Prepare
## 1.1 Check the environment
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
## 1.2 Create new environment
Make sure already install Anaconda.

**if not:**

1. Download the {}.sh file.
2. Install Anaconda: 
```bash
bash./{filename.sh}
```
**Completed install Anacconda:**

Create new environment and activate:
```
conda create -n {env_name} python=3.6.12
conda activate env_name
```

# 2. Install OpenPose
## 2.1 Download OpenPose(Tensorflow version)
```bash
cd src
mkdir githubs
cd githubs
git clone https://github.com/
```
## 2.2 Download Pretrained models(MobileNet-Thin models)
MobileNet-Thin models has been inside, see folder:
```
src/githubs/tf-pose-estimation/models/graph
cmu  mobilenet_thin  mobilenet_v2_large  mobilenet_v2_small
```
Choose to download(CMU models)

Original Version more accuracy but large and long execution time:
```
cd tf-pose-estimation/models/graph/cmu
bash download.sh
```

# Reference:
1. [Chenge Yang, Zhicheng Yu, Feiyu Chen, "Human Pose Estimation Benchmarking and Action Recognition," Deep Learning Project, Winter 2019, Northwestern University, 26-Oct-2019.](https://github.com/ChengeYang/Human-Pose-Estimation-Benchmarking-and-Action-Recognition)
2. [Feiyu Chen, "Human-Pose-Estimation-Benchmarking-and-Action-Recognition,"Deep Learning Project, Winter 2019, Northwestern University, 26-Oct-2019.](https://github.com/felixchenfy/Realtime-Action-Recognition)
