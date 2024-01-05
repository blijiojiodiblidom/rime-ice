# 雾凇拼音

功能齐全，词库体验良好，长期更新修订。

<br>

[RIME(Rime Input Method Engine) / 中州韵输入法引擎](https://rime.im/) 是一个跨平台的输入法算法框架。

这里是 Rime 的一份配置仓库。雾凇拼音提供了一套开箱即用的完整配置，包含了输入方案（全拼、双拼）、长期维护的词库及各项扩展功能。用户需要下载平台对应的前端，并将此配置放到配置目录。

详细介绍：[Rime 配置：雾凇拼音](https://dvel.me/posts/rime-ice/)

[常见问题](https://github.com/iDvel/rime-ice/issues/133)

[更新日志](./others/CHANGELOG.md)

<br>

## 基本套路

- 简体 | 全拼 | 双拼
- 主要功能
  - [melt_eng](https://github.com/tumuyan/rime-melt) 英文输入
  - [优化英文输入体验](https://dvel.me/posts/make-rime-en-better/)
  - [两分输入法](http://cheonhyeong.com/Simplified/download.html) 拼字
  - 自整理的 Emoji
  - [以词定字](https://github.com/BlindingDark/rime-lua-select-character)
  - [长词优先](https://github.com/tumuyan/rime-melt/blob/master/lua/melt.lua)
  - [Unicode](https://github.com/shewer/librime-lua-script/blob/main/lua/component/unicode.lua)
  - [数字、人民币大写](https://wb98.gitee.io/)
  - 日期、时间、星期
  - 常见错音错字提示
  - 所有标点符号直接上屏，/ 模式改为 v 模式，/ 直接上屏
  - 增加了许多拼音纠错
- 简体字表、词库
  - [《通用规范汉字表》](https://github.com/iDvel/The-Table-of-General-Standard-Chinese-Characters)
  - [华宇野风系统词库](http://bbs.pinyin.thunisoft.com/forum.php?mod=viewthread&tid=30049)
  - [清华大学开源词库](https://github.com/thunlp/THUOCL)
  - [《现代汉语常用词表》](https://gist.github.com/indiejoseph/eae09c673460aa0b56db)
  - [《现代汉语词典》](https://forum.freemdict.com/t/topic/12102)
  - [《同义词词林》](https://forum.freemdict.com/t/topic/1211)
  - [《新华成语大词典》](https://forum.freemdict.com/t/topic/11407)
  - [腾讯词向量](https://ai.tencent.com/ailab/nlp/en/download.html)
- 词库修订
  - 校对大量异形词、错别字、错误注音
  - 全词库完成注音
  - 同义多音字注音

<br>

## 长期维护词库

主要维护的词库：

- `8105` 字表。
- `base` 基础词库。
- `ext` 扩展词库，小词库。
- `tencent` 扩展词库，大词库。
- Emoji

维护内容主要是异形词、错别字的校对，错误注音的修正，缺失的常用词汇的增添，词频的调整。

<br>

## 使用说明

⚠️ 单独使用词库注意事项：`rime_ice.dict.yaml` 下面包含了大写字母，这和配置有些许绑定，可以直接删除，详细说明：[#356](https://github.com/iDvel/rime-ice/issues/356)

雾凇拼音中多个文件可能与其他方案同名冲突，如果是新手想一键安装，建议备份原先配置，清空配置目录再导入。

配置目录为小狼毫的 `%APPDATA%\Rime`，鼠须管的 `~/Library/Rime`，可通过右键菜单栏图标打开。

### 手动安装

将仓库所有文件复制粘贴到配置目录，重新部署。

<br>

## 感谢 ❤️

感谢上述提到的词库、方案及功能参考。

感谢 [@Huandeep](https://github.com/Huandeep) 整理的多个词库。

感谢 [@Mirtle](https://github.com/mirtlecn) 完善的多个功能。

感谢所有贡献者。

搜狗转 Rime：[lewangdev/scel2txt](https://github.com/lewangdev/scel2txt)

大量参考：

- [校对标准论坛](http://www.jiaodui.com/bbs/)
- [汉典](https://www.zdic.net/)
- [成语典](https://dict.idioms.moe.edu.tw/)

Thanks to JetBrains for the OSS development license.

[![JetBrains](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)](https://jb.gg/OpenSourceSupport)

<br>

## 赞助 ☕

如果觉得项目不错，可以请 [Dvel](https://github.com/iDvel/rime-ice) 吃个煎饼馃子。
