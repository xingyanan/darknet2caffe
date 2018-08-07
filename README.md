# Darknet to Caffe
darknet转caffe简化版本、修改了原版转成的caffemodel结果错误的bug，删除了pytorch依赖项，仅作darknet转caffe用
### 环境
    python2.7
### 依赖库：
    pycaffe
    numpy
### Quick Start：
    python darknet2caffe.py DARKNET_CFG DARKNET_WEIGHTS
### Tips：
darknet中的pooling层是same pooling 向矩阵右下方padding与caffe中pooling的方式不同，需要把转成的prototxt最后一层max pooling 的size改为1，才能保证caffe的输出结果与darknet一致，亲测yolov2-tiny可用
    

