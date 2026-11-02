# GitHub Trending 收藏合集

每周一 / 三 / 五更新。视角固定三问：现在流行什么、它解决了人们什么需求、指向什么未来趋势。往期已报的项目不重复报，新一期放最上面。

---

## 2026-11-02（第五期）｜离线语音听写、手机遥控 AI 队友、给 AI 的轻量浏览器

### 1. cjpais/Handy ＋ anomalyco/hex（合并一条：离线语音听写）
🔗 https://github.com/cjpais/Handy
🔗 https://github.com/anomalyco/hex

按住一个键、说话、松手，文字就直接出现在你正在用的任何应用里，全程本机转写，不上传录音。

【解决了什么需求】打字慢、想用语音输入的人，过去要么忍受云端转写把语音传出去，要么按月付费买听写软件。这两个开源工具把 Whisper 级别的转写装进本机：Handy 功能更全（可换模型、能接 Raycast），Hex 更轻（Mac 有 Apple silicon 安装包，首跑下载模型后就不再联网），都不用订阅、语音不出本机。提醒一句：Mac 上用蓝牙耳机麦克风时 Handy 可能有音质折损，介意的话用内置麦。

### 2. pingdotgg/t3code
🔗 https://github.com/pingdotgg/t3code

用手机 App（或网页、桌面端）遥控你电脑上的 AI 助手：Claude Code、Codex、Cursor、Grok Build 等都能接进来，在手机上看进度、发指令。

【解决了什么需求】AI 干活常常一跑就是半小时，人却被绑在电脑前盯着；出门了就管不了家里的任务。T3 Code 相当于给 AI 队伍配了个遥控器：任务在电脑上跑，你在手机上看、改、拍板。注意：它还很早期，作者自己都说会有 bug，而且要你已有各家助手并登录好——它只是遥控器，不是模型本身。

### 3. lightpanda-io/browser
🔗 https://github.com/lightpanda-io/browser

从零重写、专给 AI 和自动化用的无头浏览器：自称比无头 Chrome 轻 16 倍、快 9 倍，还能用一句话指挥它上网办事，事后把操作存成可重放的脚本。

【解决了什么需求】AI 想上网干活（查价、填表、抓数据），过去只能拖着笨重的 Chrome，又慢又吃内存。Lightpanda 把浏览器瘦身成 AI 的"眼睛和手"。普通人能直接受益的一点是，它能把网页一键转成 Markdown、PDF 或截图，查资料、存网页更顺手。提醒一句：16 倍、9 倍是它自己的基准测试数据，不是第三方实测。

### 4. FlashML-org/FreeToken
🔗 https://github.com/FlashML-org/FreeToken

把数据中心级别的大模型服务搬到个人电脑上：在游戏 PC 上本地跑 290B 参数以上的开源大模型，号称交互速度跟得上。

【解决了什么需求】最强的大模型都在云端、按量付费，想"自己的模型自己跑"的人过去被硬件门槛挡住。FreeToken 专为 MoE 大模型做边缘优化，让消费级显卡也能扛起大模型——"不订阅、数据不出门"的本地路线又往前走了一步。提醒一句：桌面 App 目前只写了 Windows / Linux，没有 Mac 版；且它吃的是 RTX 30 / 40 / 50 系显卡，普通 Mac 用户现阶段更适合围观。

### 5. anthropics/skills
🔗 https://github.com/anthropics/skills

Anthropic 官方公开的 Agent Skills 仓库：技能就是"一文件夹指令＋脚本＋资料"，让 Claude 在特定任务上按固定流程干活，仓库里还公开了 Claude 自己做 Word / PDF / PPT / 表格的那几套技能。

【解决了什么需求】往期报过一堆民间技能包，但普通人一直有个疑问：技能到底有没有标准、会不会哪天就过时？官方仓库加规范等于给技能"转正"：技能从民间插件变成平台标配，连 Claude 做文档的看家本领都摊开给你看怎么做。注意：仓库自标为演示教学用途，部分技能在正式 Claude 里的表现可能不同。

### 6. public-apis/public-apis
🔗 https://github.com/public-apis/public-apis

持续维护的免费 API 大全：按类别收录可免费调用的公开接口，从天气、翻译到动漫、笑话都有。

【解决了什么需求】想自己动手做个小工具（比如每天自动查天气、做个小机器人）的人，第一步往往卡在"去哪找免费数据"。这份清单把全网免费接口按类别整理好，等于给业余折腾者的工具箱配了张索引。提醒一句：它只是清单、不是成品，接口随时可能变，用之前要看一眼每条的说明。

【趋势信号】
1. **AI 正在从"云端订阅"向"本机运行"回流。** 离线听写、本机跑 290B 大模型、轻量浏览器同期上榜，指向同一个不满：不想按月付费、不想把语音和数据交出去。本地化不再只是极客偏好，正在变成普通人的卖点。
2. **人的位置从"操作者"退到了"发号施令者"。** 手机遥控电脑上的 AI、一句话指挥浏览器上网办事、官方技能库把流程标准化——人越来越少亲手点鼠标，更多是下指令、看结果、拍板。下一波好用的工具，比的可能是"指令传得顺不顺"。
3. **"技能"正式从民间插件升级为平台基础设施。** 官方技能仓库＋规范公开，意味着技能生态有了标准答案；往期民间技能包的热潮，正在被官方收编成"应用商店"式的标配。对普通人来说，选 AI 助手以后可能像装 App 一样：先看它带了哪些技能。

---

## 2026-10-30（第四期）｜AI 家教、文档变真 PPT、49 人 AI 游戏工作室

### 1. HKUDS/DeepTutor
🔗 https://github.com/HKUDS/DeepTutor

终身个性化 AI 家教工作台：聊天辅导、提问、出题、做研究、可视化、解题、精通路径、沉浸式阅读、视频课都装在一个系统里，还能对着 B 站 / YouTube 视频逐句讲。

自学最大的难受是"没人带"：资料散在各处、练了题没人批改、学完就忘。DeepTutor 把资料库、题库、学习路径和可查可改的记忆拼成一个工作台，相当于请了个记得你进度的家教。注意：试用要配模型或用 Docker 部署，动手门槛比开箱工具高。

### 2. hugohe3/ppt-master
🔗 https://github.com/hugohe3/ppt-master

把文档或一个主题变成真正的、原生可编辑的 PPT：母版、原生形状、带数据的图表、转场动画、按演讲稿生成的配音全有，还能套你自己的.pptx 模板。

做 PPT 的痛点不是"没内容"，而是排版耗时、AI 生成的成品常常是改不动的图片。PPT Master 交出来的是一份能在 PowerPoint 里继续改的真文件，等于把最磨人的排版活先干掉八成。

### 3. Donchitos/Claude-Code-Game-Studios
🔗 https://github.com/Donchitos/Claude-Code-Game-Studios

把 Claude Code 变成一间完整游戏工作室的模板：49 个智能体按总监、部门负责人、专员三层分工，74 个工作流技能，覆盖 Godot、Unity、虚幻三大引擎。

一个人用 AI 做游戏，最容易死在"没结构"上：想到哪写到哪、写一半就乱套、没人质检。这一套把真实工作室的分工和质检流程搬了进来：创意总监把关方向、QA 验过才算完，你只负责拍板。

### 4. milind-soni/OpenMausBot
🔗 https://github.com/milind-soni/OpenMausBot

开源版 Grok Bot / Muse / dots：一个聊天 App 里养一队 AI 同事，每个机器人有自己的模型、自己的电脑、自己接的应用，危险操作动手前先问你。

大厂的个人智能体产品一个接一个，全是封闭订阅、数据放在人家那边，还要抢邀请码。OpenMausBot 把这个产品形态开源重做了一遍：用你自己的模型账号、在你自己的电脑上养一队助手。Mac 有直接可装的安装包。

### 5. thedotmack/claude-mem
🔗 https://github.com/thedotmack/claude-mem

给 AI 智能体的跨会话记忆压缩系统：自动记下每轮会话里 AI 干了什么、压缩成摘要，下次开新会话自动把相关上下文找回来，支持 Claude Code、Codex、Gemini 等多种工具。

AI 最招人烦的毛病之一是"换个会话就失忆"：上次做到哪、踩过什么坑、定过什么规矩，全要重讲一遍。claude-mem 不用你记，它自动记、自动找。注意：默认走它的托管记忆服务，有 30 天免费试用，介意数据出本机的可以选本地模式。

### 6. elayadesign/ai-design-skills ＋ Leonxlnx/taste-skill（合并一条：落地页审美技能包）
🔗 https://github.com/elayadesign/ai-design-skills
🔗 https://github.com/Leonxlnx/taste-skill

一套专做落地页的设计技能包：先问清你要卖什么、再定页面结构和转化文案、最后给出一整套字体、间距、动效的视觉系统；后者是它的灵感来源之一。

AI 做的宣传页容易一眼假：结构千篇一律、文案像套话、视觉没主次。这套技能把"先想清楚卖点、再动手设计"的工作流钉死，让普通人不用懂设计，也能拿到一张像正经产品官网的落地页。


1. **AI 的形态从"一个助手"变成了"一支队伍"。** 49 人的游戏工作室、一队有电脑的聊天机器人、跨会话的记忆系统同期上榜——竞争点已经不是单个模型多聪明，而是这支队伍分工清不清、记不记得事、有没有自己的电脑干活。
2. **"普通人直接用的成品"压过了底层技术。** 本期最有烟火气的三样——AI 家教、真 PPT、落地页——全是把 AI 塞进学生和打工人的具体活里，而不是拼模型参数。
3. **开源正在正面平替大厂的封闭产品。** OpenMausBot 直接点名 Grok Bot、Muse、dots 做开源版，策略从"发明一个新东西"变成了"把人家的产品形态重做一遍、还给你"。

---

## 2026-10-28（第三期）｜AI 队友工作台、给 AI 立规矩的技能包、AI 审计员与炒股辩论团

### 1. nightly-labs/openbot
🔗 https://github.com/nightly-labs/openbot

本地优先的 AI 队友桌面工作台：给 Codex、Claude、Grok 等不同 AI 各配一个专属工作区，排任务队、传文件、控浏览器，还能让 AI 之间互相协作。

现在用多个 AI，就像同时开十几个互不认识的聊天窗口：每个都要重新交代背景，换一个就断片。OpenBot 相当于给 AI 们租了一间办公室：各自有工位、任务排着队、文件互通，不用每次从头讲起。注意：它自标为开发预览版，权限放得较宽，尝鲜前先看清它的安全说明。

### 2. obra/superpowers ＋ multica-ai/andrej-karpathy-skills（合并一条：给 AI 立规矩）
🔗 https://github.com/obra/superpowers
🔗 https://github.com/multica-ai/andrej-karpathy-skills

两套让 AI 干活先讲方法的技能包：前者是一套完整工作法——先问清你要什么、再出设计、再拆成小任务、分给子智能体执行并逐项复核；后者是把 Karpathy 关于大模型编程常见坑的观察浓缩成一份行为准则。

AI 编程助手最大的毛病是"上来就写代码"：不问需求、不做计划、写偏了也不自知。这两套技能包相当于给 AI 配了项目经理和老手经验：先把事想清楚再动手，普通人提需求时也不容易被 AI 带跑偏。

### 3. cloudflare/security-audit-skill
🔗 https://github.com/cloudflare/security-audit-skill

Cloudflare 出的 AI 安全审计技能：按多阶段流程查代码，最后输出可独立验证、机器可读的审计结论，而不是一句"大概没问题"。

代码安全审计本来是专家活，又贵又慢；而让 AI 随口审代码，最怕的就是结论没法核实。这个技能把审计变成"分阶段、可复查"的流程：每条发现都有证据和验证路径。

### 4. akitaonrails/ai-memory
🔗 https://github.com/akitaonrails/ai-memory

给 AI 编程工具装的长期记忆：用 Git 管理的 Markdown 笔记本做底本，跨 20 多种 AI 工具、跨电脑、跨项目共享同一份记忆，默认不用调用大模型。

每个 AI 工具都有自己的小本子：换个工具、换台电脑、交给同事，之前的上下文就全丢了，又要从头讲架构、讲踩过的坑。ai-memory 相当于一本所有 AI 共用的工作交接本。

### 5. AgriciDaniel/claude-seo
🔗 https://github.com/AgriciDaniel/claude-seo

给 Claude Code 装的通用 SEO 技能包：26 个子技能加 19 个子智能体，覆盖技术 SEO、内容质量、结构化数据、本地 SEO、电商 SEO，还能出 PDF / Excel 报告。

想让自己的网站、店铺或内容被搜到，SEO 是一堆零散又技术化的清单，普通人根本无从下手。这个技能包把整套活打包成"一键可用的专家流程"，不用自己拼清单。

### 6. TauricResearch/TradingAgents
🔗 https://github.com/TauricResearch/TradingAgents

模拟真实交易公司的多智能体炒股框架：基本面、舆情、新闻、技术面四组分析师先出报告，多空两方再辩论，最后由交易员和风控拍板。

单个 AI 给买卖建议像黑箱：不知道它看了什么、漏了什么、风险在哪。TradingAgents 把"投资委员会开会"搬进了程序：先分析、再辩论、再风控，让每一次决策的理由和反对意见都摆在台面上。仅供研究学习，不是投资建议。


1. **AI 的竞争从"单个模型"转向"一支队伍的基础设施"。** 工作台、工作法、长期记忆同期冲榜，说明大家已经不满足于一个聪明的聊天框，开始给 AI 配办公室、配规矩、配交接本。
2. **技能包正在走向"专业职称化"。** 安全审计、SEO、Karpathy 编程经验……技能包不再是通用小帮手，而是直接对标一个专业岗位的工作流。
3. **"一个 AI 说了算"越来越不受信任，"辩论＋证据"成了新标准。** 炒股要多空辩论、安全审计要可验证的发现——人们对 AI 结论的要求，从"给个答案"升级为"把理由和反方意见一起摊开"。

---

## 2026-10-26（第二期）｜开箱即用的 AI 助手、AI 审美课、桌面小鸭与离线文件转换

### 1. makecindy/cindy
🔗 https://github.com/makecindy/cindy

开源、开箱即用的 AI Agent：把多个模型和工具装进一个助手，能在自己的电脑和手机上替你干活。

以前的 AI 助手要么只会聊天，要么装起来门槛高。Cindy 主打"想到就能做到"：不用折腾配置就能上手，还能记住你的习惯、定时跑重复任务，普通人也能拥有一个真正干活的 AI 助手，而不是一个只会回答问题的聊天框。

### 2. Nutlope/hallmark ＋ pbakaus/impeccable（合并一条：AI 的审美课）
🔗 https://github.com/Nutlope/hallmark
🔗 https://github.com/pbakaus/impeccable

两套给 AI 编程工具装的"设计技能包"，专门治 AI 做出来的页面那种一眼假的"AI 味"。

现在人人都能让 AI 做网页，但做出来的东西长得都一个样：紫蓝渐变、卡片套卡片、千篇一律的图标。这两套技能包给 AI 立了审美规矩：48 套风格主题任选、62 条硬性检查规则自动挑刺，让 AI 做出来的页面像真人设计师的手笔。

### 3. pollen-robotics/microduck
🔗 https://github.com/pollen-robotics/microduck

只有 25 厘米、800 克的两足小鸭机器人，会走路、会捡东西、摔倒了自己爬起来，还会嘎嘎叫。

机器人一直给人"实验室里的大玩具"印象，又贵又遥远。Microduck 把强化学习训出来的走路本领装进一只桌面小鸭：手柄一推就走、装上轮子能滚、推倒了自己站起来——AI 从屏幕里走出来，变成桌上一个好玩又看得见摸得着的小伙伴。

### 4. Renhuai123/ziwei-doushu
🔗 https://github.com/Renhuai123/ziwei-doushu

紫微斗数开源排盘引擎：基于倪海厦《天纪》体系，排盘算法、四化系统、格局知识库和古籍原文全公开，10 月 15 日刚更新了 67.5 万张命盘的解读数据集。

想了解紫微斗数的人，过去只能困在各家收费 App 的围墙里，算法是黑盒、解读不知出处。这个项目把"算法是公开的传统智慧，不应该被锁在围墙里"落到实处：排盘逻辑、古籍引证全部摊开，普通人也能免费排盘、对照原文自己看门道。

### 5. KnifeLemon/Filee
🔗 https://github.com/KnifeLemon/Filee

免费开源的离线文件转换器：按住一个键、把文件拖到鼠标旁弹出的"甜甜圈"菜单上，260 多种格式随手转，图片、PDF、Word、视频、电子书全行，不用装 Office、不上传文件。

格式转换是每个打工人都绕不开的琐事：网上转换站要上传文件（隐私悬）、还要看广告、转一次等半天；装一堆软件又占地方。Filee 把转换做成"拖一下就行"的顺手动作，文件全程只留在本机。

### 6. JetBrains/thinkrail
🔗 https://github.com/JetBrains/thinkrail

JetBrains 出的轻量 AI 编程 IDE：围着 pi 智能体搭了一个真正的编辑器，还会越用越懂你的项目。

"vibe coding"（用嘴说需求、让 AI 写代码）火了，但很多工具要么只是个聊天框、要么笨重难用。ThinkRail 把"会自己记项目规矩的助手"和"真正的编辑器"合在一起：任务互不干扰地并行跑、改动能一条条过目再合并——让不会编程的人也能把想法变成软件时，心里更有底。


1. **AI 正在从"会聊天"变成"会干活、还会长记性"。** Cindy 开箱即干活、ThinkRail 越用越懂你的项目，竞争点从"模型多聪明"转向"助手多省心"。
2. **"AI 味"成了新的嫌弃点，审美开始有标准答案。** Hallmark 和 Impeccable 同期冲榜，说明大家已经不满足于"AI 能做出来"，开始挑"做得好不好看、像不像人做的"。
3. **好玩的、摸得着的 AI 正在破圈。** 桌面小鸭机器人、紫微斗数开源排盘、拖一下就转格式的工具——本期最有烟火气的三样都不是给程序员的。

---

## 2026-10-23（第一期）｜AI 技能包、本地化工具、电视去广告

### 1. Gathin23/cleanyourtv
🔗 https://github.com/Gathin23/cleanyourtv

同一 Wi-Fi 下远程给安卓电视"洗澡"：去广告、去臃肿，换一个干净的桌面。

智能电视开机广告、桌面被推荐位和预装应用霸占是普遍怨念。它用 ADB 脚本先备份，再关掉遥测、赞助行和预装应用（不卸载任何东西），装一个只有四个应用坞的极简启动器，还有一键还原脚本兜底。

### 2. peach-mitao/peach
🔗 https://github.com/peach-mitao/peach

桌面应用，把散落在本地硬盘和 115 / PikPak / OneDrive 等网盘里的个人影视收藏汇成一个私人影库。

片子存在各处、找片翻半天。它读取已有的 NFO 和海报、补全缺失的元数据，全屏海报墙播放、支持字幕搜索；观看记录和设置只存在本机。

### 3. debpalash/VoiceStudio
🔗 https://github.com/debpalash/VoiceStudio

完全本地运行的开源版 ElevenLabs：声音克隆、声音设计、视频配音、听写、转录、有声书制作，支持 646 种语言。

想做播客、有声书、视频配音的人，要么按月付订阅费，要么把自己的声音传到云端。它一次装好全本地跑，不花钱也不上传，普通人也能玩配音。

### 4. anthropics/knowledge-work-plugins ＋ anthropics/claude-plugins-official（合并一条：Claude 插件生态）
🔗 https://github.com/anthropics/knowledge-work-plugins
🔗 https://github.com/anthropics/claude-plugins-official

Anthropic 官方出的两套 Claude 插件：前者专为知识工作者（写文档、做表格、整理资料）准备；后者是官方维护的高质量 Claude Code 插件目录。

普通人用 AI 的痛点从"不会写提示词"变成了"想让它真干活"。插件把"写周报、整理表格、处理文档"变成可一键安装的技能包，不用懂代码也能给 AI 加装备。

### 5. storytold/photocraft
🔗 https://github.com/storytold/photocraft

用纯 Rust 从零重写的 Photoshop：图层、蒙版、调整图层、文字、画笔全有，能打开、编辑、保存真正的 PSD 文件。

Adobe 订阅越来越贵、软件越来越臃肿。开源社区想证明一件事：大厂的核心软件也能被干净重写一次——而且每个操作都是命令，界面、命令行、MCP 都能驱动它。

### 6. morluto/rea
🔗 https://github.com/morluto/rea

让 AI 代理逆向工程任意软件：原生二进制走 Hopper / Ghidra，JS / Electron 应用、.NET 程序集、网站都能看，全本地分析，最后解释"某个功能是怎么实现的"，附证据和结论边界。

想学透一个软件怎么工作，但没源码、看不懂代码。它把"读代码"变成"直接问 AI"，还把分析限定在本地、结论带上可信度说明。

### 7. Ebony-Vinyl/dsh-our-free-model
🔗 https://github.com/Ebony-Vinyl/dsh-our-free-model

DeepSeek Harness（dsh）终端的一个插件：装上后模型列表直接填满免费前沿模型（DeepSeek V4.1 Flash、Kimi K3 等），免登录、免 API key，还带本地中转端口给别的工具调用。

想免费用上强模型，又不想注册一堆账号、到处找 key、担心用量被记账。它把免费通道聚合好，用量统计只留本机。


1. **"技能包"正在成为 AI 落地的标准件。** 本期半数以上热门是 skill / plugin：给代码审计的 skill、给知识工作者的插件、官方插件目录……AI 的竞争从"模型更强"转向"开箱即用的技能更多"。
2. **本地化、去订阅是一股明确的回潮。** 本地配音工作站、开源重写 Photoshop、电视去臃肿工具，都在回答同一个不满：不想按月付费、不想被广告和臃肿绑架。
3. **AI 的能力边界在向"理解软件本身"延伸。** rea 让 AI 读懂没有源码的软件——AI 正在从"写代码的工具"变成"能自己研究软件的同事"。
