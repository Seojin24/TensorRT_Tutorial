## Progress Record
 - 2017-04-27 The project was launched to create a GitHub repository.
 - 2017-09-30 TensorRT 3 was recently released to tidy up the current resources.
 - 2017-10-18 Add Blog - Implement the leaky relu layer with TensorRT
 - 2017-11-11 Resources: Add google's INT8 open source library
 - 2017-11-25 Add blog - Introduction to the use of TensorRT Plugin - Take the leaky relu layer as an example

 -------

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
