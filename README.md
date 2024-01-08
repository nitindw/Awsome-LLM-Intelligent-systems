# <p align=center>`Awsome-LLM-Intelligent-systems`<br>
This repo contains a curated list of resources on LLM for Intelligent systems( Autonomous driving, Robotics ..etc) , arranged chronologically. We regularly update it with the latest papers and their corresponding open-source implementations.

## Table of Contents

- [Perception](#LEARNING-APPROACHES)
- [Planning](#EXPLAINABILITY)
- [Control](#EVALUATION)
- [Simulation Frameworks](#SAFETY)
- [Datasets](#Large-Language-Models-in-autonomous-driving)
- [CITATION](#Citation)

# Perception
The following are the different Perception approaches of LLM 

## Perception

- [**Driving with LLMs: Fusing Object-Level Vector Modality for Explainable Autonomous Driving**](https://browse.arxiv.org/abs/2310.01957) [arXiv 2023] <br> Long Chen, Oleg Sinavski, Jan Hünermann, Alice Karnsund, Andrew James Willmott, Danny Birch, Daniel Maund, Jamie Shotton <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/wayveai/Driving-with-LLMs)
  - Backbone: LLaMA
  - Modality: Vector, Language
  - Output: Answer, Actions
- [**Talk2BEV: Language-Enhanced Bird's Eye View Maps**](https://arxiv.org/abs/2310.02251) [arXiv 2023] <br> Vikrant Dewangan, Tushar Choudhary, Shivam Chandhok, Shubham Priyadarshan, Anushka Jain, Arun K. Singh, Siddharth Srivastava, Krishna Murthy Jatavallabhula, K. Madhava Krishna <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/llmbev/talk2bev)
  - Backbone: Flan5XXL, Vicuna-13b
  - Modality: Vision Language
  - Output: Answer


## Planning
- [**Talk2BEV: Language-Enhanced Bird's Eye View Maps**](https://arxiv.org/abs/2310.02251) [arXiv 2023] <br> Vikrant Dewangan, Tushar Choudhary, Shivam Chandhok, Shubham Priyadarshan, Anushka Jain, Arun K. Singh, Siddharth Srivastava, Krishna Murthy Jatavallabhula, K. Madhava Krishna <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/llmbev/talk2bev)
  - Backbone: Flan5XXL, Vicuna-13b
  - Modality: Vision Language
  - Output: Answer
- [**GAIA-1: A Generative World Model for Autonomous Driving**](https://arxiv.org/abs/2309.17080) [arXiv 2023] <br> AnthonyHu, LloydRussell, HudsonYeo, ZakMurez, GeorgeFedoseev,AlexKendall,JamieShotton,andGianlucaCorrado. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/taesiri/ArXivQA/blob/main/papers/2309.17080.md)
  - Backbone: GAIA generative model
  - Modality: Vision Language
  - Output: Video
 - [**Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents**](https://arxiv.org/abs/2201.07207) [arXiv 2022] <br> WenlongHuang,PieterAbbeel,DeepakPathak, andIgor Mordatch. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/huangwl18/language-planner)
  - Backbone: GPT-3 Codex
  - Modality: Language
  - Output: proposal
- [**Dilu: Aknowledge-driven approach to autonomous drivingwith large languagemodels**](https://arxiv.org/abs/2309.16292) [arXiv 2023] <br> LichengWen, Daocheng Fu, XinLi, XinyuCai, Tao Ma, PinlongCai,MinDou, BotianShi, LiangHe, and YuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Action
- [**Drive as you speak: Enabling human-like interaction with large language models in autonomous vehicles**](https://openaccess.thecvf.com/content/WACV2024W/LLVM-AD/html/Cui_Drive_As_You_Speak_Enabling_Human-Like_Interaction_With_Large_Language_WACVW_2024_paper.html) [WACV Workshops 2024] <br> CanCui,YunshengMa,XuCao,WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: code
- [**Receive,Reason,andReact:Drive as You Say with Large Language Models in Autonomous Vehicles**](https://arxiv.org/abs/2310.08034) [arXiv 2023] <br> CanCui,YunshengMa,XuCao,WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: Answer
- [**Drive Like a Human:Rethinking Autonomous Driving with Large Language Models**](https://arxiv.org/abs/2307.07162) [arXiv 2023] <br> DaochengFu,XinLi,LichengWen,MinDou,PinlongCai, BotianShi,andYuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DriveLikeAHuman)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Answer
- [**Learning to Drive with GPT**](https://arxiv.org/abs/2310.01415) [arXiv 2023] <br> JiagengMao, Yuxi Qian, HangZhao, andYueWang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PointsCoder/GPT-Driver)
  - Backbone: GPT-3.5
  - Modality: Vision Language
  - Output: Route
## Control

- [**Driving with LLMs: Fusing Object-Level Vector Modality for Explainable Autonomous Driving**](https://browse.arxiv.org/abs/2310.01957) [arXiv 2023] <br> Long Chen, Oleg Sinavski, Jan Hünermann, Alice Karnsund, Andrew James Willmott, Danny Birch, Daniel Maund, Jamie Shotton <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/wayveai/Driving-with-LLMs)
  - Backbone: LLaMA
  - Modality: Vector, Language
  - Output: Answer, Actions
- [**Dilu: Aknowledge-driven approach to autonomous driving with large language models**](https://arxiv.org/abs/2309.16292) [arXiv 2023] <br> LichengWen, Daocheng Fu, XinLi, XinyuCai, Tao Ma, PinlongCai,MinDou, BotianShi, LiangHe, and YuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4.0
  - Modality: Language
  - Output: Action
- [**Receive,Reason,andReact:Drive as You Say with Large Language Models in Autonomous Vehicles**](https://arxiv.org/abs/2310.08034) [arXiv 2023] <br> CanCui,YunshengMa,XuCao,WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: Answer
- [**Drive Like a Human:Rethinking Autonomous Driving with Large Language Models**](https://arxiv.org/abs/2307.07162) [arXiv 2023] <br> DaochengFu,XinLi,LichengWen,MinDou,PinlongCai, BotianShi,andYuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DriveLikeAHuman)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Answer
