# 小恶魔（Koakuma）
一个东方主题的QQ群聊机器人。QQ：2705296421，可以加好友拉入群聊，或联系我处理(QQ：2834993398)。

## 使用方法
发送“小恶魔（指令）”，例如“小恶魔抽卡”。有附带参数的指令在指令名称后加空格后输入，例如“小恶魔识图 [某张图片]”。

## 功能指令列表
### 画画
使用Novelai生成图片，具体使用方法见[说明](https://github.com/zxxsmart/koakuma/blob/main/ai_image_readme.md)。（调用的官网，大概不久后会到期）

### 识图
需要参数：一张图片（可后续再发送）。使用[DeepDanbooru](https://github.com/KichangKim/DeepDanbooru)预测该图片的tag，返回其可能含有的角色（东方角色有中文翻译）。

### 原曲识别
原曲识别小游戏。可选参数：指定难度为E，N，H，L，默认为N。返回一段东方音乐的随机切片（群语音形式），50s内回答名称（中文日文英文部分均可），答对者获得相应积分，没有人答对则公布答案。

### 排行榜
返回群里原曲识别游戏的排行榜。

### 翻译
需要参数：一张图片（可后续再发送）。使用有道翻译，返回该图片的翻译（图片形式）。

### 搜图
需要参数：一张图片（可后续再发送）。使用[SauceNao](https://saucenao.com/)搜索该图片，返回结果。

### 随个老婆/随个角色
发送一个随机东方角色的介绍。可选参数“完整”：额外发送一段一设资料。

### 随个音乐
发送一个随机东方音乐与其出处。

### 抽卡
发送一个随机符卡名称和使用者。

### 随个机体
需要参数：作品名（可后续再发送）。返回一个该作品的随机机体。支持自然语言调用，例如句子中包含小恶魔、风神录和机体三个关键词，则会返回一个风神录的机体。

### 随个pnd/随个p榜
发送一个随机的[PND分数榜](https://thscore.pndsng.com/index.php)记录。


## 播报类功能
需要联系我在指定群内开启。
### 复读机
默认开启，复读群消息。

### 东方日历
定时播报当天的东方主题日，资料来自[TouhouCalendarBot](https://github.com/TouhouCalendar/TouhouCalendarBot)

### 最新PND榜
播报最新的一条[PND分数榜](https://thscore.pndsng.com/index.php)记录。

### B站直播间
播报开播信息。

还有个比较搞笑的聊天功能，@小恶魔 + 一些英文内容可以聊天，

### 还有些暂时废弃的功能