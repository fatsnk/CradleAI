## 界面预览

<table style="border-collapse: collapse; width: 100%;">
  <tr>
    <td style="text-align: center; padding: 5px;">
      <img src="https://cradleintro.top/app-screenshot.png" alt="APP截图 1" style="max-width: 150px; border: 1px solid #ddd;">
      <br>
    </td>
    <td style="text-align: center; padding: 5px;">
      <img src="https://cradleintro.top/app-screenshot2.png" alt="APP截图 2" style="max-width: 150px; border: 1px solid #ddd;">
      <br>
    </td>
    <td style="text-align: center; padding: 5px;">
      <img src="https://cradleintro.top/app-screenshot3.png" alt="APP截图 3" style="max-width: 150px; border: 1px solid #ddd;">
      <br>
    </td>
    <td style="text-align: center; padding: 5px;">
      <img src="https://cradleintro.top/app-screenshot4.png" alt="APP截图 4" style="max-width: 150px; border: 1px solid #ddd;">
      <br>
    </td>
    <td style="text-align: center; padding: 5px;">
      <img src="https://cradleintro.top/app-screenshot5.png" alt="APP截图 5" style="max-width: 150px; border: 1px solid #ddd;">
      <br>
    </td>
    <td style="text-align: center; padding: 5px;">
      <img src="https://cradleintro.top/app-screenshot6.png" alt="APP截图 6" style="max-width: 150px; border: 1px solid #ddd;">
      <br>
    </td>
  </tr>
</table>

## 答疑/bug反馈/意见反馈：
qq群：1017292082

## 更新日志

0514-1.0.3

**1. 正则表达式增强：**

*   更新了全局正则表达式和局部正则表达式，用于角色绑定。
*   在导入角色卡时会自动导入角色绑定的正则，需要在正则页面绑定保存一下。

**2. 前端卡适配：**

*   支持正则表达式配合前端卡进行游玩。
*   **注意：**
    *   如果前端卡未完全适配移动端，可能会有一些损失。
    *   如果开场白不是标准的 HTML 页面，应用会进行自动补全，但不保证覆盖所有的情况。建议补全为标准 HTML 页面格式后导入。例如：

    ```html
    <!DOCTYPE html>
    <html>
    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
      <title></title>
      <style>
        body { background: #222; color: #f8f8f2; font-family: 'Helvetica', 'Arial', sans-serif; margin: 0; padding: 1em; }
        img, video { max-width: 100%; border-radius: 5px; }
        pre, code { background: #111; color: #fff; border-radius: 4px; padding: 0.2em 0.4em; }
      </style>
    </head>
    <body>
    ${text}
    </body>
    </html>
    ```

**3. 页面日志：**

*   增加了页面日志，用于查看请求消息和结果。

**4. Bug 修复：**

*   修复了导入某些大型角色卡出错的问题。
*   修复了朋友圈一些提示词问题。
*   修复了全局世界书无法保存的问题。
*   修复了全局预设无法修改的问题
*   修复了第一条AI消息删除/编辑出错的问题
  
**5. 界面优化：**

*   支持隐藏顶部栏。
*   优化全局设置页面的响应式布局。
* 
**6. 新增文本宏：**

*   `{{lastusermessage}}`：最新用户消息，等价于已有的 `{{lastmessage}}`。
*   `{{lastcharmessage}}`：最新角色消息。
*   `{{random::A::B...}}`：将被替换为提供的参数中的随机值。例如， `{{random::A::B::C}}` 将被替换为 A 、 B 或 C 中的一个。如果没有提供参数，它将被替换为 0 和 1 之间的随机数。
*   `{{roll::A}}`：将被随机数 1 和 A 之间的数字替换。如果 A 以 `d` 开头，它将被随机数 1 和 A 之间的数字替换，不包含 `d`。

**7. 开场白增强：**

*   支持导入角色卡时导入多个开场白，可以在详情页切换。

**8. 错误处理：**

*   错误请求对应的 user 和 ai 消息条将自动被清除。

**9. 性能优化：**

*   优化了页面的性能和布局，减少卡顿和发热的问题。
*   解决某些设备发信息闪退的问题。
*   减少不必要的日志打印
  
0505：重要修复＆更新

1.修复openai兼容渠道无法使用记忆功能的问题

2.修复角色卡页面视图状态没有持久化的问题

3.改善用户回复角色时，角色分不清社交状态的问题

4.修复消息截断问题（目前暂时没设置maxtoken，回复字数可以通过世界书和预设限制）

5.修复``<summary><detail>``标签无法渲染的问题（在1.0.1中可能造成部分消息因为被此类标签包裹而被丢弃）

6.修复api设置页切换渠道时测试失败/应用失败的问题

更新：

1.全局预设，支持导入和编辑

2.全局世界书，

3.消息编辑，删除，重新生成功能

4.支持添加多个openai兼容渠道

5.支持添加和编辑多个开场白

6.新增 gemini官方渠道的gemini-2.5-flash-preview-04-17

7.Character页面的视图状态可持久化

0502：

0.响应式布局优化

1.修复部分安卓机型无法正确在主页执行下滑手势的问题

2.支持配置OPENAI兼容渠道/hajimi轮询渠道，可以设置自己的中转或者轮询

3.修复了一些局部功能尚不支持openrouter渠道的问题

0501：

1.已修复gemini渠道高级设置模型无法切换的问题

2.支持markdown渲染功能

3.优化角色详情编辑页面的交互

4.支持以下自定义标签的折叠/渲染，如果有不支持的标签，请根据实际适当调整角色卡，以免包裹的文本消失：

```
<thinking> / <think> / <char-think>：思考过程折叠块
<mem>：回忆折叠块
<status> / <StatusBlock> / <statusblock>/<detail>/ <summery>：状态栏块
<websearch>：搜索结果折叠块
<font>：支持 color/face/size 属性的字体标签
<img>：图片标签（支持 image:id 及普通 url）
```

## 主要功能

### 1. 角色管理
- 支持手动、自动创建和导入SillyTavern角色卡，世界书和预设（PNG/JSON格式）。
- 角色可自定义头像、背景、动态立绘视频。
- 管理模式下可批量删除、导出角色数据，支持角色图库和图片生成。

### 2. 智能聊天
- 独立实现了与SillyTavern功能等效的世界书、预设和角色信息系统：
  - **世界书条目管理**：自动注入相关世界设定条目到对话，根据对话关键词智能匹配
  - **预设条目处理**：自定义位置，深度，角色的预设条目
  - **角色信息融合**：无缝整合角色卡、世界书和预设
- 记忆管理系统：
  - 长对话自动总结
  - 智能记忆检索
  - 联网搜索集成
- 支持保存点系统，可随时恢复任意历史对话状态
- 高级交互功能：
  - **作者注释**：支持自定义作者注释和插入深度设置
  - **语音交互**：通过TTS功能让角色说话，带语音增强效果
  - **多媒体消息**：在对话中发送和接收图片，支持图像分析和上下文理解
  - **图片管理**：内置图片缓存系统，方便保存和管理所有对话图片
  - **视觉小说模式**：提供类似视觉小说的沉浸式对话界面
- 高级消息格式化：
  - 富文本支持：处理常见的HTML标签和特殊标签，开发者可自定义需要渲染的标签
  - 自定义标签：支持思考标签、状态块、记忆标签等特殊格式
  - 图片嵌入：支持内联图片显示和全屏查看
- 可视化辅助功能：
  - 完整对话历史查看
  - 自动滚动和手动位置保存

### 3. 朋友圈（Circle）
- 角色和用户可发布动态、图片，支持点赞、评论、转发。
- 朋友圈互动支持 AI 自动生成角色评论、点赞及内心想法展示。
- 支持用户自定义动态发布与图片选择。
- 多模态支持：
  - 图片分析：AI 可以理解并回应带有图片的帖子内容
  - 智能回复：基于图像内容生成相关评论和反馈
- 定时发布系统：
  - 角色可设置多个时间点自动发布朋友圈
  - 基于当前时间生成适合的动态内容
  - 发布后可通过通知提醒用户
- 关系系统集成：
  - 角色互动会动态影响角色间关系
  - 帖子评论和点赞可提升角色间好感度
  - 支持通过朋友圈互动更新角色关系类型（如朋友、熟人、对手等）
- 对话流连接：
  - 朋友圈互动会自动同步到角色的聊天历史
  - 用户在朋友圈的互动可无缝延续到私聊对话
- 互动频率控制：
  - 可自定义角色朋友圈活跃度（低、中、高）
  - 智能管理角色互动频率，避免过度回复
- 可持久化存储所有朋友圈内容，支持帖子管理和删除功能

### 4. 群聊系统
- 支持创建/加入群聊，与多个角色/用户共同对话。
- 群聊支持自定义背景、成员管理、消息同步。

### 5. 记忆与知识管理

- 集成向量记忆系统，自动存储和检索对话相关事实。
- 支持表格插件扩展角色知识。
- 记忆面板可查看和管理角色记忆内容。
- 双系统记忆增强：
  - **结构化表格记忆**：基于模板创建自定义表格，存储角色关系、喜好、事件等结构化信息
  - **向量存储记忆**：自动提取对话要点，存储为向量记忆以供后续对话检索
- 表格记忆管理功能：
  - 多种预设模板：角色关系、事件记录、喜好清单等专用模板
  - 自定义编辑：可添加、删除、修改表格行列数据
  - 与对话深度整合：对话信息自动更新相关表格
- 向量记忆管理功能：
  - 检索优化：智能匹配当前对话最相关的历史记忆
  - 记忆编辑：增加、修改、删除具体记忆条目
  - 记忆导出/导入：支持备份和恢复角色记忆数据
- 记忆优先级控制：自定义记忆处理频率，调节对话中记忆更新和检索的频次
- 性能监控：记忆数据库统计和健康状态监控

### 6. TTS 增强
- 支持文本转语音（TTS）功能，可增强语音互动体验。
- TTS 增强器可自定义语音参数。
- 当前版本需开发者自行配置 TTS 服务端点（后续更新将支持前端自主配置 TTS 端点）。
- 支持多种语音控制功能：
  - 语音播放/暂停控制
  - 增强模式音质提升
  - 多角色不同语音模板
  - 自动缓存已生成语音，减少重复请求

### 7. 图片生成与管理
- 支持 NovelAI 图片生成，自动根据对话上下文生成角色场景背景。
- 角色图库侧边栏可管理、收藏、设置图片为头像/背景。
- 高级标签系统：
  - 支持智能分类的标签选择器，包含上百种分类标签
  - 支持标签加权与降权
  - 固定标签功能，可锁定重要特征标签
  - 角色标签从预设库中选择，确保精确的角色识别
  - 艺术家风格参考，可选择不同艺术家样式
  - 自定义提示词输入，支持复杂描述
  - "Roll"功能可随机生成标签组合获得灵感
- 多模型支持：
  - Animagine 4：默认图像生成引擎（需开发者自定义服务端点）
  - NovelAI：支持更精细的控制和多角色场景
- 高级生成设置：
  - 多种图像尺寸预设：肖像、横向、方形、大型
  - 可自定义步数、采样器、噪声调度等专业参数
  - 支持Seed值管理，可使用相同Seed重现图像
- 多角色场景控制（NovelAI）：
  - 位置控制系统，可精确定位多个角色在图像中的位置
  - 支持为场景中的每个角色设置独立提示词
  - 多角色互动姿势和表情控制
- 生成结果处理：
  - 一键设置为角色头像或背景图
  - 自动保存到角色图库
  - 可查看和复制生成参数，方便再次使用相同配置

### 8. 其他功能
- 支持 API 设置、模型预算、存储管理、社区入口等扩展功能。
- 支持多种主题与界面自定义。

## 部署方法

本应用基于 [Expo](https://expo.dev/) 框架开发，推荐使用 EAS Build 进行打包和部署：

1. **Android 平台打包**  
   在项目根目录下执行以下命令，通过 EAS 构建 Android 安装包（APK 或 AAB）：
   ```bash
   eas build --platform android
   ```
   构建完成后，可在 Expo 控制台下载生成的安装包进行分发或安装。

2. **iOS 平台打包**  
   亦可通过如下命令为 iOS 平台生成 IPA 包：
   ```bash
   eas build --platform ios
   ```
   但目前尚未在苹果设备真机环境下充分测试，建议谨慎用于生产环境。

> **注意**：请确保已正确配置 Expo 账户、EAS CLI 及相关平台证书。详细配置与分发流程请参考 [Expo 官方文档](https://docs.expo.dev/build/introduction/)。

## 当前限制

### API支持
- 当前版本仅支持Gemini和OpenRouter API渠道
- 计划在后续版本中添加对更多官方API渠道的支持，如ChatGPT、Claude等
- 图像生成功能目前仅支持NovelAI，计划增加更多选择

### 其他已知问题
- 部分高级功能需要开发者自行配置服务端点
- 记忆向量数据库在大量数据时可能有性能瓶颈
- 某些功能在网络不稳定时可能响应较慢

## 许可证

本项目基于 [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) 许可开源，需遵守以下规则：

- **署名** — 您必须给出适当的署名，提供指向本协议的链接，并指明是否（对原作）作了修改。您可以以任何合理方式进行，但不得以任何方式暗示许可方认可您或您的使用。
- **非商业性使用** — 您不得将本作品用于商业目的，包括但不限于任何形式的商业倒卖、SaaS、API 付费接口、二次销售、打包出售、收费分发或其他直接或间接盈利行为。

## 声明

-本项目是一个非商业的开源前端工具，任何人可自行上传代码在EXPO平台打包和安装，或进行原生的apk构建。

-现在和将来都不会提供任何角色卡上传或分享的功能或平台，如角色卡作者声明了不可以在SillyTavern之外的软件上导入角色卡，请勿在项目中导入角色卡。

-禁止任何形式的商业倒卖、SaaS、API 付费接口、二次销售、打包出售、收费分发或其他直接或间接盈利行为。

-禁止将本项目打包上传任何应用商店。

## 引用项目

1. 表格记忆：`https://github.com/muyoou/st-memory-enhancement`，在此感谢作者的代码分享，请大家多多支持原作者。

2. mem0：`https://github.com/mem0ai/mem0` 基于 [Apache-2.0 license](https://www.apache.org/licenses/LICENSE-2.0) 许可。

3. OpenAI-adapter：感谢hajimi作者提供测试渠道，项目地址：`https://github.com/wyeeeee/hajimi` 


## 赞助

如果您喜欢本项目并希望支持作者，可以请我喝一杯咖啡：

[请作者喝一杯咖啡](https://cradleintro.top/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20250430201333.png)
