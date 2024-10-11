[!IMPORTANT]
2024.10.10: Power outage occurred, emergency restoration of file server providing [whl package](https://drive.google.com/file/d/19U_hsLoMrjOlQSzYS3pzWX9fTzyusArP/view?usp=sharing)  
2024.10.8: Version 3.90 added preliminary support for llama-index, version 3.80 added plugin secondary menu function (see wiki for details)  
2024.5.1: Added Doc2x feature for translating PDF papers, [see details](https://github.com/binary-husky/gpt_academic/wiki/Doc2x)  
2024.3.11: Fully supports Chinese large language models like Qwen, GLM, DeepseekCoder! SoVits voice cloning module, [see details](https://www.bilibili.com/video/BV1Rp421S7tF/)  
2024.1.17: When installing dependencies, please choose the **specified versions** in `requirements.txt`. Installation command: `pip install -r requirements.txt`. This project is completely open source and free. You can encourage the development of this project by subscribing to the [online service](https://github.com/binary-husky/gpt_academic/wiki/online).

<br>

<div align=center>
<h1 align="center">
<img src="docs/logo.png" width="40"> GPT Academic Optimization (GPT Academic)
</h1>

[![Github][Github-image]][Github-url]
[![License][License-image]][License-url]
[![Releases][Releases-image]][Releases-url]
[![Installation][Installation-image]][Installation-url]
[![Wiki][Wiki-image]][Wiki-url]
[![PR][PRs-image]][PRs-url]

[Github-image]: https://img.shields.io/badge/github-12100E.svg?style=flat-square
[License-image]: https://img.shields.io/github/license/binary-husky/gpt_academic?label=License&style=flat-square&color=orange
[Releases-image]: https://img.shields.io/github/release/binary-husky/gpt_academic?label=Release&style=flat-square&color=blue
[Installation-image]: https://img.shields.io/badge/dynamic/json?color=blue&url=https://raw.githubusercontent.com/binary-husky/gpt_academic/master/version&query=$.version&label=Installation&style=flat-square
[Wiki-image]: https://img.shields.io/badge/wiki-项目文档-black?style=flat-square
[PRs-image]: https://img.shields.io/badge/PRs-welcome-pink?style=flat-square

[Github-url]: https://github.com/binary-husky/gpt_academic
[License-url]: https://github.com/binary-husky/gpt_academic/blob/master/LICENSE
[Releases-url]: https://github.com/binary-husky/gpt_academic/releases
[Installation-url]: https://github.com/binary-husky/gpt_academic#installation
[Wiki-url]: https://github.com/binary-husky/gpt_academic/wiki
[PRs-url]: https://github.com/binary-husky/gpt_academic/pulls

</div>
<br>

**If you like this project, please give it a Star; if you invent useful shortcuts or plugins, feel free to send pull requests!**

If you like this project, please give it a Star.
Read this in [English](docs/README.English.md) | [日本語](docs/README.Japanese.md) | [한국어](docs/README.Korean.md) | [Русский](docs/README.Russian.md) | [Français](docs/README.French.md). All translations have been provided by the project itself. To translate this project into any arbitrary language with GPT, read and run [`multi_language.py`](multi_language.py) (experimental).
<br>

> [!NOTE]
> 1. The functionality of each file in this project is detailed in the [self-analysis report](https://github.com/binary-husky/gpt_academic/wiki/GPT‐Academic项目自译解报告)`self_analysis.md`. As versions iterate, you can also click on related function plugins at any time to call GPT to regenerate the project's self-analysis report. For common questions, please refer to the wiki.
>    [![Common Installation Method](https://img.shields.io/static/v1?label=&message=常规安装方法&color=gray)](#installation)  [![One-Click Installation Script](https://img.shields.io/static/v1?label=&message=一键安装脚本&color=gray)](https://github.com/binary-husky/gpt_academic/releases)  [![Configuration Instructions](https://img.shields.io/static/v1?label=&message=配置说明&color=gray)](https://github.com/binary-husky/gpt_academic/wiki/项目配置说明) [![wiki](https://img.shields.io/static/v1?label=&message=wiki&color=gray)]([https://github.com/binary-husky/gpt_academic/wiki/项目配置说明](https://github.com/binary-husky/gpt_academic/wiki))
>
> 2. This project is compatible with and encourages experimentation with domestic Chinese large language models such as Tongyi Qianwen, Zhipu GLM, etc. Supports coexistence of multiple api-keys, which can be filled in the configuration file like `API_KEY="openai-key1,openai-key2,azure-key3,api2d-key4"`. When temporarily changing `API_KEY`, enter the temporary `API_KEY` in the input area and press the enter key to submit it to take effect.

<br><br>

<div align="center">

Features (⭐ = recently added features) | Description
--- | ---
⭐[Access New Models](https://github.com/binary-husky/gpt_academic/wiki/%E5%A6%82%E4%BD%95%E5%88%87%E6%8D%A2%E6%A8%A1%E5%9E%8B) | Baidu [Qianfan](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) and Wenxin Yiyan, Tongyi Qianwen [Qwen](https://modelscope.cn/models/qwen/Qwen-7B-Chat/summary), Shanghai AI-Lab [Shusheng](https://github.com/InternLM/InternLM), iFly [Xinghuo](https://xinghuo.xfyun.cn/), [LLaMa2](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf), [Zhipu GLM4](https://open.bigmodel.cn/), DALLE3, [DeepseekCoder](https://coder.deepseek.com/)
⭐Supports mermaid image rendering | Supports generating [flowcharts](https://www.bilibili.com/video/BV18c41147H9/), state transition diagrams, Gantt charts, pie charts, GitGraph, etc. (version 3.7)
⭐Arxiv Paper Fine Translation ([Docker](https://github.com/binary-husky/gpt_academic/pkgs/container/gpt_academic_with_latex)) | [Plugin] One-click [translate arxiv papers](https://www.bilibili.com/video/BV1dz4y1v77A/) with ultra-high quality, currently the best paper translation tool
⭐[Real-time Voice Dialogue Input](https://github.com/binary-husky/gpt_academic/blob/master/docs/use_audio.md) | [Plugin] Asynchronously [listen to audio](https://www.bilibili.com/video/BV1AV4y187Uy/), automatically punctuate, and find opportunities for responses automatically
⭐AutoGen Multi-Agent Plugin | [Plugin] Explore the potential of intelligent emergence with Microsoft AutoGen!
⭐Void Terminal Plugin | [Plugin] Use natural language to directly schedule other plugins of this project
Polishing, translating, code explanation | One-click polishing, translating, finding grammatical errors in papers, and explaining code
[Custom Shortcuts](https://www.bilibili.com/video/BV14s4y1E7jN) | Supports custom shortcuts
Modular Design | Supports powerful [plugins](https://github.com/binary-husky/gpt_academic/tree/master/crazy_functions), plugins support [hot updates](https://github.com/binary-husky/gpt_academic/wiki/%E5%87%BD%E6%95%B0%E6%8F%92%E4%BB%B6%E6%8C%87%E5%8D%97)
[Program Analysis](https://www.bilibili.com/video/BV1cj411A7VW) | [Plugin] One-click analyze Python/C/C++/Java/Lua/... project tree or [self-analysis](https://www.bilibili.com/video/BV1cj411A7VW)
Reading papers, [translating](https://www.bilibili.com/video/BV1KT411x7Wn) papers | [Plugin] One-click interpret latex/pdf papers and generate summaries
Latex Full [Translation](https://www.bilibili.com/video/BV1nk4y1Y7Js/), [Polishing](https://www.bilibili.com/video/BV1FT411H7c5/) | [Plugin] One-click translation or polishing of latex papers
Batch Comment Generation | [Plugin] One-click batch generate function comments
Markdown [Chinese-English Translation](https://www.bilibili.com/video/B
