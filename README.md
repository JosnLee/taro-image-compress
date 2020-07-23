# 扩展Taro 的图片选择以及压缩方法


## 安装

npm i taro-image-compress

## 使用
```bash
import {chooseImage,compressImage} from 'taro-image-compress'

###  * 选择文件后并压缩，返回压缩后的文件的base64
### * @param maxFileSize 压缩后的文件的最大值K  例如1500代表的是压缩后最大不超过1500k
### * @param sizeType 图片源默认['original', 'compressed']，原图和压缩图
### * @param sourceType 图片源默认['album', 'camera']，默认图库和照片
### * @returns {PromiseLike<T> | Promise<T>}
 
chooseImage(maxFileSize = 1500, sizeType = ['original', 'compressed'], sourceType = ['album', 'camera']) 
   returns {PromiseLike<T> | Promise<T>}

###  * 选择文件后并压缩，返回压缩后的文件的base64/**
###  * 选择文件后并压缩，返回压缩后的文件的base64 * 压缩图片
###  * 选择文件后并压缩，返回压缩后的文件的base64 * @param filePath 文件路径
###  * 选择文件后并压缩，返回压缩后的文件的base64 * @param quality 压缩图片的比例
###  * 选择文件后并压缩，返回压缩后的文件的base64 * @returns {PromiseLike<{fileName: string, base64: string}> | Promise<{fileName: string, base64: string}>}
 ###  * 选择文件后并压缩，返回压缩后的文件的base64*/


compressImage(filePath, quality = 0.4) 
  returns {PromiseLike<T> | Promise<T>}


```