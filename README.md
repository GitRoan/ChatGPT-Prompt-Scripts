## chatGPT 插件脚本 中文 Prompt 训练对话框

![image](https://user-images.githubusercontent.com/96854855/232969587-555ec793-57de-4c32-9c29-29c1eb6fe156.png)

在油猴中安装该脚本，可以在chatGPT对话框中出现 Prompt 的按钮，支持一键导入对应的角色训练词

帮助你更好的训练chatGPT，回复你的问题

可自行添加 `Prompt`

[让生产力加倍的 ChatGPT 快捷指令](https://github.com/rockbenben/ChatGPT-Shortcut)

或在此项目提`PR`合并

forkfrom：https://github.com/maomao1996/tampermonkey-scripts

forkfrom：https://github.com/rockbenben/ChatGPT-Shortcut

## 🤔 常见问题

### 为什么提示词用英文？

ChatGPT Shortcut 是为方便中文母语人士使用 ChatGPT 而创建的，但是提示词却全部是英文。这是因为相较于中文，ChatGPT 对英文的理解更为出色。即使是国内第一个对话式大型语言模型 MOSS，也承认 MOSS 的英文回答水平比中文高，建议使用英文。（MOSS 已不对外开放）

使用中文提示词可能会得到不错的结果，但是当你再次输入相同的中文提示时，结果可能与之前大相径庭。因为 ChatGPT 对中文的理解每次都不同，所以建议大家在生产力型提示词的输入中使用英文提示词，以保证输出效果。此外，英文提示词带来的回复也很可能是英文的，你可以在提示词结尾添加 `respond in Chinese`，将回复指定为中文。

### 每次都要输入 Promot？

API 中可以将提示词设为「system prompt」，这样后续就不需要输入提示词了，ChatGPT 会按照 system prompt 来执行操作。

在网页版 ChatGPT 中，如果没有切换主提示词，只需用引号将后续回复内容框选即可，这样就不需要每次都输入提示词。当回复内容不符合提示词要求时，说明 ChatGPT 已经忘记了提示词，此时需要重新输入提示词以唤醒它。

### 中文搜索延迟

搜索功能基于 Docusaurus 的 showcase，存在 PC 端中文输入法焦点丢失问题。向 Docusaurus 反馈后，对方表示会尝试修复和 `FWIW, you should not be using Chinese anyway, since the showcase is not localized`。但问题始终没有解决。因此，我将搜索组件分为移动端和 PC 端两类。移动端搜索逻辑保持不变，而屏幕宽度阈值 768px 以上的 PC 端浏览引入 `debounce` 函数解决中文输入问题。但这在 PC 端产生两个问题：一是中文输入需在 800 毫秒内完成；二是 PC 端搜索刷新从即时变为 800 毫秒延迟。若你有更好的解决方案，欢迎提供反馈。

### 输出虚假信息

ChatGPT 虽然非常强大，但并不是万能的。有时它会输出虚假信息。例如，当我需要将上百条信息录入到 ChatGPT Shortcut 中时，我让 ChatGPT 按指定格式转换数据。但是在转换过程中，我发现其中一些信息被 ChatGPT 误写。例如，在文本中一条标签是 `movie critic`，而 ChatGPT 将其更改为 `film critic`。尽管这在文本中不会造成什么影响，但放在代码中会报错。因此，在使用 ChatGPT 时，务必检查其输出内容。

### 提示词不好用

所有提示词均来自互联网，会定期进行更新。虽然我测试过每一条提示词，但实际效果可能因需求而有所偏差。如果你发现任何错误、有创意的想法或有好的提示词，欢迎

此外，提示词不仅能用于工作生产，更重要的是帮助您开拓思路，发散思维，从多个角度考虑问题，并解决人们在思考时容易忽略的问题。
