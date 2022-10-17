# 小恶魔画画使用说明
## 调用格式为：小恶魔画画 (指定分辨率) (可选的参数) (输入的词条)

例如：小恶魔画画 /p touhou, hakurei reimu

### 指定分辨率：
/p 竖版512*768
/l 横板768*512
/s 方形640*640

### 输入的词条：
词条间以逗号加空格分隔，词条最多225个。{}表示加强，[]表示减弱，可套娃。具体词条可去官网的输入栏测试，会有颜色显示模型对该词条的了解程度。默认在最前面加了masterpiece, high quality这两个。注意不要有中文字符。


## 可选的参数：调用格式为：参数名=具体内容。参数间以空格分隔。

### model：
safe-diffusion            质量较好
（默认）nai-diffusion     包含更多内容（nsfw）
nai-diffusion-furry       beta版

### uc：（要抑制的词条）
（默认）[nsfw, lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry]，相同的大可不必添加。
如需添加请按照如下格式，用中括号括起来：
uc=[big breasts, large breasts]
（如果输入词条有nsfw则会将这里的去除）

## 下方参数如不了解建议保持默认
### seed：
默认随机。用于复现结果，取值范围：0到2^32-1整数
### scale：
默认11。表示符合词条的程度
### sampler：
默认k_euler_ancestral，可选：k_euler, k_lms, plms, ddim。
### 
steps：默认28（目前上限28）。迭代次数，不是越高越好  
详细解释可参考：https://gist.github.com/crosstyan/f912612f4c26e298feec4a2924c41d99

## 使用可选参数的调用格式：
小恶魔画画 /p model=safe-diffusion seed=1341351 nc=[huge breasts, large breasts] sampler=ddim touhou, hakurei reimu