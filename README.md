# ComfyUI Workflows

按实际模型加载节点和用途整理的 ComfyUI 工作流。整理日期：2026-11-01。

## 目录

`workflows/<模型系列>/<用途>/<Current|Archive|Legacy|Drafts>/工作流.json`

Mixed-Models 表示画布中包含多个生成模型系列；并不表示每条路线都会执行。VLM-Caption 表示反推/Caption 的多模态模型组合。Model-Agnostic 表示未包含生成模型加载节点。

## 使用

1. 下载所需 JSON，拖入 ComfyUI。
2. 依据 catalog.json 的 model_files 和 node_types 安装模型及自定义节点。
3. 重新选择输入图片、文本文件、输出目录和本地服务地址。
4. 从 Current 开始；Archive/Legacy/Drafts 保留供比较和兼容性检查。

## 发布处理

保留节点、连线、控件参数及子图定义；公开副本移除了凭据字段值、机器绝对路径、本地服务地址、内嵌图像数据，并将敏感示例提示词替换为中性提示词。占位值需按本机环境重新配置。原始文件未改动。敏感命名的生成工作流、私人 Collector 场景、未连线草稿、数据库、图片、权重、批次执行快照及开发测试材料未公开。完全相同的发布副本只保留一份。

仅完成 JSON、图结构保留与发布内容静态检查；未逐工作流执行，不保证模型资源齐全或运行成功。模型和节点的许可由各自作者决定，本仓库不附带其权重或代码，也不代其授予许可。

## 工作流索引

| 模型 | 用途 | 状态 | 工作流 | 节点/连线 |
| --- | --- | --- | --- | --- |
| Anima | Batch-Text-to-Image | Current | [批量文生图.json](workflows/Anima/Batch-Text-to-Image/Current/%E6%89%B9%E9%87%8F%E6%96%87%E7%94%9F%E5%9B%BE.json) | 78/128 |
| Anima | Batch-Text-to-Image | Current | [批量文生图1n.json](workflows/Anima/Batch-Text-to-Image/Current/%E6%89%B9%E9%87%8F%E6%96%87%E7%94%9F%E5%9B%BE1n.json) | 81/134 |
| Anima | Batch-Text-to-Image | Current | [批量文生图2n.json](workflows/Anima/Batch-Text-to-Image/Current/%E6%89%B9%E9%87%8F%E6%96%87%E7%94%9F%E5%9B%BE2n.json) | 81/134 |
| Anima | Batch-Text-to-Image | Current | [批量文生图3n.json](workflows/Anima/Batch-Text-to-Image/Current/%E6%89%B9%E9%87%8F%E6%96%87%E7%94%9F%E5%9B%BE3n.json) | 81/134 |
| Anima | Batch-Text-to-Image | Current | [批量文生图4n.json](workflows/Anima/Batch-Text-to-Image/Current/%E6%89%B9%E9%87%8F%E6%96%87%E7%94%9F%E5%9B%BE4n.json) | 81/134 |
| Anima | Batch-Text-to-Image | Legacy | [sfw批量文生图_legacy.json](workflows/Anima/Batch-Text-to-Image/Legacy/sfw%E6%89%B9%E9%87%8F%E6%96%87%E7%94%9F%E5%9B%BE_legacy.json) | 78/128 |
| Anima | Image-to-Image | Archive | [单图快速图生图.json](workflows/Anima/Image-to-Image/Archive/%E5%8D%95%E5%9B%BE%E5%BF%AB%E9%80%9F%E5%9B%BE%E7%94%9F%E5%9B%BE.json) | 21/24 |
| Anima | Image-to-Image | Archive | [批量图生图_D站bkp.json](workflows/Anima/Image-to-Image/Archive/%E6%89%B9%E9%87%8F%E5%9B%BE%E7%94%9F%E5%9B%BE_D%E7%AB%99bkp.json) | 191/301 |
| Anima | Image-to-Image | Current | [批量图生图_D站.json](workflows/Anima/Image-to-Image/Current/%E6%89%B9%E9%87%8F%E5%9B%BE%E7%94%9F%E5%9B%BE_D%E7%AB%99.json) | 200/315 |
| Anima | Image-to-Image | Legacy | [批量图生图_D站_legacy.json](workflows/Anima/Image-to-Image/Legacy/%E6%89%B9%E9%87%8F%E5%9B%BE%E7%94%9F%E5%9B%BE_D%E7%AB%99_legacy.json) | 200/315 |
| Anima | Image-to-Image | Legacy | [批量图生图_D站bkp_legacy.json](workflows/Anima/Image-to-Image/Legacy/%E6%89%B9%E9%87%8F%E5%9B%BE%E7%94%9F%E5%9B%BE_D%E7%AB%99bkp_legacy.json) | 191/301 |
| Anima | Inpainting | Archive | [单图局部重绘bkp.json](workflows/Anima/Inpainting/Archive/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98bkp.json) | 144/200 |
| Anima | Inpainting | Current | [单图局部重绘.json](workflows/Anima/Inpainting/Current/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98.json) | 161/229 |
| Anima | Inpainting | Drafts | [单图局部重绘_V2.2.10_前端兼容修正版.json](workflows/Anima/Inpainting/Drafts/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98_V2.2.10_%E5%89%8D%E7%AB%AF%E5%85%BC%E5%AE%B9%E4%BF%AE%E6%AD%A3%E7%89%88.json) | 181/250 |
| Anima | Inpainting | Drafts | [单图局部重绘_V2.2.7_自动多轮.json](workflows/Anima/Inpainting/Drafts/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98_V2.2.7_%E8%87%AA%E5%8A%A8%E5%A4%9A%E8%BD%AE.json) | 149/206 |
| Anima | Inpainting | Drafts | [单图局部重绘_V2.2.8R1_简化轮次命名_种子模式.json](workflows/Anima/Inpainting/Drafts/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98_V2.2.8R1_%E7%AE%80%E5%8C%96%E8%BD%AE%E6%AC%A1%E5%91%BD%E5%90%8D_%E7%A7%8D%E5%AD%90%E6%A8%A1%E5%BC%8F.json) | 174/237 |
| Anima | Inpainting | Drafts | [单图局部重绘_V2.2.8_每轮保存_每轮路线.json](workflows/Anima/Inpainting/Drafts/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98_V2.2.8_%E6%AF%8F%E8%BD%AE%E4%BF%9D%E5%AD%98_%E6%AF%8F%E8%BD%AE%E8%B7%AF%E7%BA%BF.json) | 181/250 |
| Anima | Inpainting | Drafts | [单图局部重绘_V2.2.9_每轮保存_轮次命名_种子模式.json](workflows/Anima/Inpainting/Drafts/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98_V2.2.9_%E6%AF%8F%E8%BD%AE%E4%BF%9D%E5%AD%98_%E8%BD%AE%E6%AC%A1%E5%91%BD%E5%90%8D_%E7%A7%8D%E5%AD%90%E6%A8%A1%E5%BC%8F.json) | 181/250 |
| Anima | Inpainting | Drafts | [单图局部重绘_上传版_简化多轮修正版.json](workflows/Anima/Inpainting/Drafts/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98_%E4%B8%8A%E4%BC%A0%E7%89%88_%E7%AE%80%E5%8C%96%E5%A4%9A%E8%BD%AE%E4%BF%AE%E6%AD%A3%E7%89%88.json) | 157/220 |
| Anima | Inpainting | Drafts | [局部重绘V2.2.6_双Rerouter整理版.json](workflows/Anima/Inpainting/Drafts/%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98V2.2.6_%E5%8F%8CRerouter%E6%95%B4%E7%90%86%E7%89%88.json) | 152/207 |
| Anima | Inpainting | Legacy | [单图局部重绘_legacy.json](workflows/Anima/Inpainting/Legacy/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98_legacy.json) | 161/229 |
| Anima | Inpainting | Legacy | [单图局部重绘bkp_legacy.json](workflows/Anima/Inpainting/Legacy/%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98bkp_legacy.json) | 144/200 |
| Anima | LoRA-Review | Current | [LoRa测试2_评审_文件夹.json](workflows/Anima/LoRA-Review/Current/LoRa%E6%B5%8B%E8%AF%952_%E8%AF%84%E5%AE%A1_%E6%96%87%E4%BB%B6%E5%A4%B9.json) | 35/48 |
| Anima | LoRA-Review | Current | [LoRa测试2_评审_权重.json](workflows/Anima/LoRA-Review/Current/LoRa%E6%B5%8B%E8%AF%952_%E8%AF%84%E5%AE%A1_%E6%9D%83%E9%87%8D.json) | 34/45 |
| Anima | LoRA-Review | Current | [LoRa测试2_评审_种子.json](workflows/Anima/LoRA-Review/Current/LoRa%E6%B5%8B%E8%AF%952_%E8%AF%84%E5%AE%A1_%E7%A7%8D%E5%AD%90.json) | 34/44 |
| Anima | LoRA-Testing | Current | [LoRA-Text-CLIP_单图简易文生图.json](workflows/Anima/LoRA-Testing/Current/LoRA-Text-CLIP_%E5%8D%95%E5%9B%BE%E7%AE%80%E6%98%93%E6%96%87%E7%94%9F%E5%9B%BE.json) | 28/32 |
| Anima | LoRA-Testing | Current | [LoRa测试2.json](workflows/Anima/LoRA-Testing/Current/LoRa%E6%B5%8B%E8%AF%952.json) | 27/31 |
| Anima | LoRA-Testing | Current | [LoRa测试2_LoRA文件夹并行.json](workflows/Anima/LoRA-Testing/Current/LoRa%E6%B5%8B%E8%AF%952_LoRA%E6%96%87%E4%BB%B6%E5%A4%B9%E5%B9%B6%E8%A1%8C.json) | 27/32 |
| Anima | LoRA-Testing | Current | [LoRa测试（文生图 ）.json](workflows/Anima/LoRA-Testing/Current/LoRa%E6%B5%8B%E8%AF%95%EF%BC%88%E6%96%87%E7%94%9F%E5%9B%BE%20%EF%BC%89.json) | 27/31 |
| Anima | LoRA-Testing | Current | [同Lora多prompt测试.json](workflows/Anima/LoRA-Testing/Current/%E5%90%8CLora%E5%A4%9Aprompt%E6%B5%8B%E8%AF%95.json) | 29/33 |
| Anima | LoRA-Testing | Current | [多Lora同prompt测试.json](workflows/Anima/LoRA-Testing/Current/%E5%A4%9ALora%E5%90%8Cprompt%E6%B5%8B%E8%AF%95.json) | 29/33 |
| Anima | LoRA-Testing | Current | [多Lora同prompt测试_双K采样器_一键Turbo.json](workflows/Anima/LoRA-Testing/Current/%E5%A4%9ALora%E5%90%8Cprompt%E6%B5%8B%E8%AF%95_%E5%8F%8CK%E9%87%87%E6%A0%B7%E5%99%A8_%E4%B8%80%E9%94%AETurbo.json) | 37/49 |
| Anima | Prompt-Tools | Current | [提示词并行追加_Anima测试.json](workflows/Anima/Prompt-Tools/Current/%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B9%B6%E8%A1%8C%E8%BF%BD%E5%8A%A0_Anima%E6%B5%8B%E8%AF%95.json) | 12/13 |
| Anima | Text-to-Image | Archive | [单图高级文生图.json](workflows/Anima/Text-to-Image/Archive/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE.json) | 70/105 |
| Anima | Text-to-Image | Current | [单图简易文生图 2-V3测试.json](workflows/Anima/Text-to-Image/Current/%E5%8D%95%E5%9B%BE%E7%AE%80%E6%98%93%E6%96%87%E7%94%9F%E5%9B%BE%202-V3%E6%B5%8B%E8%AF%95.json) | 30/33 |
| Anima | Text-to-Image | Current | [单图简易文生图 2.json](workflows/Anima/Text-to-Image/Current/%E5%8D%95%E5%9B%BE%E7%AE%80%E6%98%93%E6%96%87%E7%94%9F%E5%9B%BE%202.json) | 29/32 |
| Anima | Text-to-Image | Current | [单图简易文生图.json](workflows/Anima/Text-to-Image/Current/%E5%8D%95%E5%9B%BE%E7%AE%80%E6%98%93%E6%96%87%E7%94%9F%E5%9B%BE.json) | 26/29 |
| Anima | Text-to-Image | Current | [简易基本文生图流.json](workflows/Anima/Text-to-Image/Current/%E7%AE%80%E6%98%93%E5%9F%BA%E6%9C%AC%E6%96%87%E7%94%9F%E5%9B%BE%E6%B5%81.json) | 13/14 |
| Anima | Text-to-Image | Drafts | [单图简易文生图 2-livecheck.json](workflows/Anima/Text-to-Image/Drafts/%E5%8D%95%E5%9B%BE%E7%AE%80%E6%98%93%E6%96%87%E7%94%9F%E5%9B%BE%202-livecheck.json) | 27/30 |
| Anima | Text-to-Image | Drafts | [单图简易文生图 2-光照接线草稿.json](workflows/Anima/Text-to-Image/Drafts/%E5%8D%95%E5%9B%BE%E7%AE%80%E6%98%93%E6%96%87%E7%94%9F%E5%9B%BE%202-%E5%85%89%E7%85%A7%E6%8E%A5%E7%BA%BF%E8%8D%89%E7%A8%BF.json) | 27/28 |
| Anima | Text-to-Image | Legacy | [单图高级文生图_legacy.json](workflows/Anima/Text-to-Image/Legacy/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE_legacy.json) | 70/105 |
| Anima | Upscaling | Drafts | [单图高级文生图 v2-单次模型放大.json](workflows/Anima/Upscaling/Drafts/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE%20v2-%E5%8D%95%E6%AC%A1%E6%A8%A1%E5%9E%8B%E6%94%BE%E5%A4%A7.json) | 22/24 |
| Mixed-Models | Text-to-Image | Current | [单图高级文生图.json](workflows/Mixed-Models/Text-to-Image/Current/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE.json) | 87/168 |
| Mixed-Models | Text-to-Image | Drafts | [单图高级文生图 v2.json](workflows/Mixed-Models/Text-to-Image/Drafts/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE%20v2.json) | 75/148 |
| Mixed-Models | Text-to-Image | Drafts | [单图高级文生图.json](workflows/Mixed-Models/Text-to-Image/Drafts/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE.json) | 78/153 |
| Mixed-Models | Text-to-Image | Drafts | [单图高级文生图_Anima_Base-Turbo可切换.json](workflows/Mixed-Models/Text-to-Image/Drafts/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE_Anima_Base-Turbo%E5%8F%AF%E5%88%87%E6%8D%A2.json) | 95/170 |
| Mixed-Models | Text-to-Image | Drafts | [单图高级文生图_Anima_Base-Turbo简化预览模式.json](workflows/Mixed-Models/Text-to-Image/Drafts/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE_Anima_Base-Turbo%E7%AE%80%E5%8C%96%E9%A2%84%E8%A7%88%E6%A8%A1%E5%BC%8F.json) | 94/167 |
| Mixed-Models | Text-to-Image | Drafts | [单图高级文生图__da285f71.json](workflows/Mixed-Models/Text-to-Image/Drafts/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE__da285f71.json) | 78/150 |
| Mixed-Models | Text-to-Image | Drafts | [单图高级文生图_含Turbo模式.json](workflows/Mixed-Models/Text-to-Image/Drafts/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE_%E5%90%ABTurbo%E6%A8%A1%E5%BC%8F.json) | 89/165 |
| Mixed-Models | Text-to-Image | Legacy | [单图高级文生图 v2_legacy.json](workflows/Mixed-Models/Text-to-Image/Legacy/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE%20v2_legacy.json) | 76/149 |
| Mixed-Models | Text-to-Image | Legacy | [单图高级文生图_含Turbo模式.Legacy.json](workflows/Mixed-Models/Text-to-Image/Legacy/%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE_%E5%90%ABTurbo%E6%A8%A1%E5%BC%8F.Legacy.json) | 78/150 |
| Model-Agnostic | Camera | Drafts | [CameraDirector_Simple_Workflow.json](workflows/Model-Agnostic/Camera/Drafts/CameraDirector_Simple_Workflow.json) | 3/2 |
| Model-Agnostic | Camera | Legacy | [CameraDirector_Simple_Workflow_legacy.json](workflows/Model-Agnostic/Camera/Legacy/CameraDirector_Simple_Workflow_legacy.json) | 4/2 |
| Model-Agnostic | Image-Moderation | Archive | [NSFW V2 图片列表示例.json](workflows/Model-Agnostic/Image-Moderation/Archive/NSFW%20V2%20%E5%9B%BE%E7%89%87%E5%88%97%E8%A1%A8%E7%A4%BA%E4%BE%8B.json) | 8/8 |
| Model-Agnostic | Image-Moderation | Archive | [NSFW V3 高分辨率图片列表示例.json](workflows/Model-Agnostic/Image-Moderation/Archive/NSFW%20V3%20%E9%AB%98%E5%88%86%E8%BE%A8%E7%8E%87%E5%9B%BE%E7%89%87%E5%88%97%E8%A1%A8%E7%A4%BA%E4%BE%8B.json) | 8/8 |
| Model-Agnostic | Prompt-Tools | Current | [TXT读取与提示词列表.json](workflows/Model-Agnostic/Prompt-Tools/Current/TXT%E8%AF%BB%E5%8F%96%E4%B8%8E%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%88%97%E8%A1%A8.json) | 4/3 |
| Model-Agnostic | Prompt-Tools | Current | [提示词并行追加_串联文本预览.json](workflows/Model-Agnostic/Prompt-Tools/Current/%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B9%B6%E8%A1%8C%E8%BF%BD%E5%8A%A0_%E4%B8%B2%E8%81%94%E6%96%87%E6%9C%AC%E9%A2%84%E8%A7%88.json) | 3/2 |
| Model-Agnostic | Upscaling | Archive | [放大模块.json](workflows/Model-Agnostic/Upscaling/Archive/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97.json) | 43/68 |
| Model-Agnostic | Upscaling | Archive | [放大模块v2.json](workflows/Model-Agnostic/Upscaling/Archive/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v2.json) | 56/86 |
| Model-Agnostic | Upscaling | Archive | [放大模块v2单图版.json](workflows/Model-Agnostic/Upscaling/Archive/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v2%E5%8D%95%E5%9B%BE%E7%89%88.json) | 55/84 |
| Model-Agnostic | Upscaling | Archive | [放大模块v3.json](workflows/Model-Agnostic/Upscaling/Archive/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v3.json) | 108/153 |
| Model-Agnostic | Upscaling | Archive | [放大模块v3_简化版.json](workflows/Model-Agnostic/Upscaling/Archive/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v3_%E7%AE%80%E5%8C%96%E7%89%88.json) | 38/66 |
| Model-Agnostic | Upscaling | Current | [放大模块v3_子图简化版.json](workflows/Model-Agnostic/Upscaling/Current/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v3_%E5%AD%90%E5%9B%BE%E7%AE%80%E5%8C%96%E7%89%88.json) | 38/66 |
| Model-Agnostic | Upscaling | Current | [简易图像放大.json](workflows/Model-Agnostic/Upscaling/Current/%E7%AE%80%E6%98%93%E5%9B%BE%E5%83%8F%E6%94%BE%E5%A4%A7.json) | 4/3 |
| Model-Agnostic | Upscaling | Drafts | [放大模块v2.json](workflows/Model-Agnostic/Upscaling/Drafts/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v2.json) | 54/83 |
| Model-Agnostic | Upscaling | Legacy | [放大模块_legacy.json](workflows/Model-Agnostic/Upscaling/Legacy/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97_legacy.json) | 43/68 |
| Model-Agnostic | Upscaling | Legacy | [放大模块v2_legacy.json](workflows/Model-Agnostic/Upscaling/Legacy/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v2_legacy.json) | 56/86 |
| Model-Agnostic | Upscaling | Legacy | [放大模块v3_legacy.json](workflows/Model-Agnostic/Upscaling/Legacy/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v3_legacy.json) | 108/153 |
| Model-Agnostic | Upscaling | Legacy | [放大模块v3_子图简化版_legacy.json](workflows/Model-Agnostic/Upscaling/Legacy/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v3_%E5%AD%90%E5%9B%BE%E7%AE%80%E5%8C%96%E7%89%88_legacy.json) | 38/66 |
| Model-Agnostic | Upscaling | Legacy | [放大模块v3_简化版_legacy.json](workflows/Model-Agnostic/Upscaling/Legacy/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v3_%E7%AE%80%E5%8C%96%E7%89%88_legacy.json) | 38/66 |
| Qwen-Image-2.1 | Text-to-Image | Current | [Qwen-Image-2.1_01_文生图_1024.json](workflows/Qwen-Image-2.1/Text-to-Image/Current/Qwen-Image-2.1_01_%E6%96%87%E7%94%9F%E5%9B%BE_1024.json) | 9/8 |
| Qwen-Image-2.1 | Text-to-Image | Current | [Qwen-Image-2.1_02_透明PNG文生图.json](workflows/Qwen-Image-2.1/Text-to-Image/Current/Qwen-Image-2.1_02_%E9%80%8F%E6%98%8EPNG%E6%96%87%E7%94%9F%E5%9B%BE.json) | 9/8 |
| Qwen-Image-2.1 | Utilities | Current | [Qwen-Image-2.1_03_单图编辑.json](workflows/Qwen-Image-2.1/Utilities/Current/Qwen-Image-2.1_03_%E5%8D%95%E5%9B%BE%E7%BC%96%E8%BE%91.json) | 9/10 |
| Qwen-Image-2.1 | Utilities | Current | [Qwen-Image-2.1_04_多参考图编辑.json](workflows/Qwen-Image-2.1/Utilities/Current/Qwen-Image-2.1_04_%E5%A4%9A%E5%8F%82%E8%80%83%E5%9B%BE%E7%BC%96%E8%BE%91.json) | 10/10 |
| SDXL-Illustrious | Upscaling | Current | [放大模块v4.json](workflows/SDXL-Illustrious/Upscaling/Current/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v4.json) | 51/106 |
| SDXL-Illustrious | Upscaling | Legacy | [放大模块v4_legacy.json](workflows/SDXL-Illustrious/Upscaling/Legacy/%E6%94%BE%E5%A4%A7%E6%A8%A1%E5%9D%97v4_legacy.json) | 51/106 |
| VLM-Caption | Caption | Current | [本地反推.json](workflows/VLM-Caption/Caption/Current/%E6%9C%AC%E5%9C%B0%E5%8F%8D%E6%8E%A8.json) | 22/28 |
| VLM-Caption | Caption | Drafts | [Photoreal_Batch_Caption_QwenImage_ZImage_v1.json](workflows/VLM-Caption/Caption/Drafts/Photoreal_Batch_Caption_QwenImage_ZImage_v1.json) | 7/11 |
| VLM-Caption | Caption | Drafts | [Universal_Batch_Caption_Exporter_v1.json](workflows/VLM-Caption/Caption/Drafts/Universal_Batch_Caption_Exporter_v1.json) | 24/35 |
| Z-Image | Image-to-Image | Current | [Z-Image批量图生图.json](workflows/Z-Image/Image-to-Image/Current/Z-Image%E6%89%B9%E9%87%8F%E5%9B%BE%E7%94%9F%E5%9B%BE.json) | 174/278 |
| Z-Image | Image-to-Image | Legacy | [Z-Image批量图生图_legacy.json](workflows/Z-Image/Image-to-Image/Legacy/Z-Image%E6%89%B9%E9%87%8F%E5%9B%BE%E7%94%9F%E5%9B%BE_legacy.json) | 174/278 |
| Z-Image | Inpainting | Current | [Z-Image单图局部重绘.json](workflows/Z-Image/Inpainting/Current/Z-Image%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98.json) | 154/219 |
| Z-Image | Inpainting | Legacy | [Z-Image单图局部重绘_legacy.json](workflows/Z-Image/Inpainting/Legacy/Z-Image%E5%8D%95%E5%9B%BE%E5%B1%80%E9%83%A8%E9%87%8D%E7%BB%98_legacy.json) | 154/219 |
| Z-Image | Text-to-Image | Current | [Z-Image单图高级文生图.json](workflows/Z-Image/Text-to-Image/Current/Z-Image%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE.json) | 55/94 |
| Z-Image | Text-to-Image | Legacy | [Z-Image单图高级文生图_legacy.json](workflows/Z-Image/Text-to-Image/Legacy/Z-Image%E5%8D%95%E5%9B%BE%E9%AB%98%E7%BA%A7%E6%96%87%E7%94%9F%E5%9B%BE_legacy.json) | 55/94 |
