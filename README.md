
## 进度记录
 - 2017-04-27 项目发起，创建GitHub仓库。
 - 2017-09-30 TensorRT 3最近发布，整理一下目前的资源。
 - 2017-10-18 增加博客-使用TensorRT实现leaky relu层
 - 2017-11-11 资源：新增google的INT8开源库
 - 2017-11-25 增加博客-TensorRT Plugin使用方式简介-以leaky relu层为例
 
## Progress Record
 - 2017-04-27 The project was launched to create a GitHub repository.
 - 2017-09-30 TensorRT 3 was recently released to tidy up the current resources.
 - 2017-10-18 Add Blog - Implement the leaky relu layer with TensorRT
 - 2017-11-11 Resources: Add google's INT8 open source library
 - 2017-11-25 Add blog - Introduction to the use of TensorRT Plugin - Take the leaky relu layer as an example

----
## 资源整理
 - [TensorRT 3 RC][1]和[TensorRT 2.1][2] 下载链接
 - [TensorRT 2.1 官方在线文档][3] 
 - NVIDIA 介绍TensorRT的blog-[Deploying Deep Neural Networks with NVIDIA TensorRT][4]
 - GTC 2017介绍TensorRT 的[PPT][5]和[视频][6]，内含INT8 Quantization和Calibration的实现原理。
 - 新增cublas 和 cudnn的INT8 [demo][7]
 - 新增本人在GTC China 2017 Community Corner主题NVIDIA INT8的PPT， [GTC-China-2017-NVIDIA-INT8.pdf][8]
 - 新增google的INT8开源库[gemmlowp][9]，目前支持ARM和CPU优化
 - “子棐之GPGPU”公众号所写的《TensorRT系列》博客，NVIDIA的工程师出的，从入门篇到INT8篇再到FP16篇最后收尾于Custom Layer篇，内容逻辑清楚，干货满满，自愧不如。附四篇博客链接：[TensorRT 系列之入门篇][10]，[TensorRT系列之INT8篇][11]，[TensorRT系列之FP16篇][12]，[TensorRT系列之Custom Layer篇][13]。
 - [《高性能深度学习支持引擎实战——TensorRT》][14]，主要内容：一、TensorRT理论介绍：基础介绍TensorRT是什么；做了哪些优化；为什么在有了框架的基础上还需要TensorRT的优化引擎。二、TensorRT高阶介绍：对于进阶的用户，出现TensorRT不支持的网络层该如何处理；


----
## Resource organization
 - [TensorRT 3 RC][1] and [TensorRT 2.1][2] Download link
 - [TensorRT 2.1 official online documentation][3]
 - NVIDIA introduces TensorRT's blog-[Deploying Deep Neural Networks with NVIDIA TensorRT][4]
 - GTC 2017 introduces TensorRT's [PPT][5] and [Video][6], including the implementation principles of INT8 Quantization and Calibration.
 - Added cublas and cudnn to INT8 [demo][7]
 - Added my PPT for GTC China 2017 Community Corner theme NVIDIA INT8, [GTC-China-2017-NVIDIA-INT8.pdf][8]
 - Added google's INT8 open source library [gemmlowp][9], currently supports ARM and CPU optimization
 - "TensorRT Series" blog written by the "Phito GPGPU" public number, NVIDIA engineers, from the entry article to the INT8 article to the FP16 article finalized in the Custom Layer article, the content logic is clear, the dry goods are full, from It is not as good as it is. Attached to four blog links: [TensorRT series entry] [10], [TensorRT series INT8] [11], [TensorRT series FP16] [12], [TensorRT series Custom Layer][13] .
 - ["High-performance deep learning support engine combat - TensorRT"] [14], main content: First, TensorRT theory introduction: Basic introduction TensorRT is what; what optimization is done; why need TensorRT on the basis of the framework Optimization engine. Second, TensorRT high-level introduction: For advanced users, how to deal with the network layer that TensorRT does not support;
---
## 博客
 - [使用TensorRT实现leaky relu层][15]
 - [TensorRT Plugin使用方式简介-以leaky relu层为例][16]
 
## Blog 
 - [Implementing a leaky relu layer using TensorRT][15]
 - [Introduction to the use of TensorRT Plugin - Take the leaky relu layer as an example] [16] 
 
 
 
 -------

# TensorRT_Tutorial

TensorRT作为NVIDIA推出的c++库，能够实现高性能推理（inference）过程。最近，NVIDIA发布了TensorRT 2.0 Early Access版本，重大更改就是支持INT8类型。在当今DL大行其道的时代，INT8在缩小模型大小、加速运行速度方面具有非常大的优势。Google新发布的TPU就采用了8-bit的数据类型。

本人目前在使用TensorRT进行INT8的探究。已经被TensorRT不完善的文档坑了一次了。所以想自力更生做一个TensorRT Tutorial，主要包括三部分：
 - TensorRT User Guide 翻译；
 - TensorRT samples 介绍分析讲解；
 - TensorRT 使用经验。

使用TensorRT者请先阅读《[TensorRT目前存在的BUG][17]》。

 感谢每一位为该翻译项目做出贡献的同学.
 
 内容来源：
 TensorRT 下载页面：
 https://developer.nvidia.com/nvidia-tensorrt-20-download
 
 TensorRT 文档、Samples
 安装后对应目录中 
 
 ## TensorRT_tutorial 
 As a C++ library from NVIDIA, TensorRT enables high-performance inference processes. Recently, NVIDIA released the TensorRT 2.0 Early Access version, a major change is to support the INT8 type. In today's era of DL, INT8 has a great advantage in reducing the size of the model and speeding up the operation. Google's newly released TPU uses an 8-bit data type.

I am currently using TensorRT for INT8 exploration. The document that has been imperfect by TensorRT has been pitted once. So I want to be a TensorRT Tutorial with my own self-reliance. It mainly consists of three parts:
 - TensorRT User Guide translation;
 - TensorRT samples introduces analytical explanations;
 - TensorRT experience.

If you are using TensorRT, please read "[TensorRT's current BUG][17]".

 Thanks to everyone who contributed to the translation project.
 
 Content source:
 TensorRT download page:
 Https://developer.nvidia.com/nvidia-tensorrt-20-download
 
 TensorRT documentation, Samples
 In the corresponding directory after installation
 
## 参与者（按参与时间排序）
TensorRT User Guide 翻译
 - [LitLeo][18]
 - [MoyanZitto][19]

翻译校对

 - 赵开勇

TensorRT samples 介绍分析讲解
- [LitLeo][20]

TensorRT 使用经验。

欲参与者请加QQ群：483063470

支持捐赠项目




## Participants (sorted by participation time)
TensorRT User Guide Translation
 - [LitLeo][18]
 - [MoyanZitto][19]

Translation proofreading

 - Zhao Kaiyong

TensorRT samples introduces analysis and explanation
- [LitLeo][20]

TensorRT experience.

For participants, please add QQ group: 483063470

Support for donation projects



 <img src="https://raw.githubusercontent.com/LitLeo/blog_pics/master/WeChat_collection.png" width = "200px" height = "200"/>


  [1]: https://developer.nvidia.com/nvidia-tensorrt3rc-download
  [2]: https://developer.nvidia.com/nvidia-tensorrt-download
  [3]: http://docs.nvidia.com/deeplearning/sdk/tensorrt-user-guide/index.html
  [4]: https://devblogs.nvidia.com/parallelforall/deploying-deep-learning-nvidia-tensorrt/
  [5]: http://on-demand.gputechconf.com/gtc/2017/presentation/s7310-8-bit-inference-with-tensorrt.pdf
  [6]: http://on-demand.gputechconf.com/gtc/2017/video/s7310-szymon-migacz-8-bit-inference-with-tensorrt.mp4
  [7]: https://github.com/LitLeo/TensorRT_Tutorial/tree/master/cublas&cudnn_int8_demo
  [8]: https://github.com/LitLeo/TensorRT_Tutorial/blob/master/GTC-China-2017-NVIDIA-INT8.pdf
  [9]: https://github.com/google/gemmlowp
  [10]: https://mp.weixin.qq.com/s/E5qbMsuc7UBnNmYBzq__5Q
  [11]: https://mp.weixin.qq.com/s/wyqxUlXxgA9Eaxf0AlAVzg
  [12]: https://mp.weixin.qq.com/s/nuEVZlS6JfqRQo30S0W-Ww?scene=25#wechat_redirect
  [13]: https://mp.weixin.qq.com/s/xabDoauJc16z3-gpyre8zA
  [14]: https://mp.weixin.qq.com/s/F_VvLTWfg-COZKrQAtOSwg
  [15]: https://github.com/LitLeo/TensorRT_Tutorial/blob/master/blogs/%E4%BD%BF%E7%94%A8TensorRT%E5%AE%9E%E7%8E%B0leaky%20relu%E5%B1%82.md
  [16]: https://github.com/LitLeo/TensorRT_Tutorial/blob/master/blogs/TensorRT%20Plugin%E4%BD%BF%E7%94%A8%E6%96%B9%E5%BC%8F%E7%AE%80%E4%BB%8B-%E4%BB%A5leaky%20relu%E5%B1%82%E4%B8%BA%E4%BE%8B.md
  [17]: https://github.com/LitLeo/TensorRT_Tutorial/blob/master/Bug.md
  [18]: https://github.com/LitLeo
  [19]: https://github.com/MoyanZitto
  [20]: https://github.com/LitLeo
