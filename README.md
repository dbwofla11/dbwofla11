<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,100:2563EB&height=240&section=header&text=Yujaerim%20%7C%20Game%20AI&fontSize=48&fontColor=F8FAFC&fontAlignY=38&desc=Building%20agents%20that%20play%2C%20learn%2C%20and%20adapt&descAlignY=59&descSize=18" alt="Yujaerim profile header" width="100%" />

### 게임을 이해하고, 행동하고, 학습하는 AI를 만들고 있습니다

숭실대학교 VIP Lab 학부연구생 · Game AI · Physical AI · Computer Vision

<a href="https://github.com/dbwofla11"><img src="https://img.shields.io/badge/GitHub-dbwofla11-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
<a href="https://solved.ac/dbwofla11"><img src="https://img.shields.io/badge/Solved.ac-dbwofla11-1F8ACB?style=flat-square" alt="Solved.ac" /></a>

</div>

<br />

## About me

저는 Unity/C#으로 게임을 만들며 생긴 질문을 **데이터, 컴퓨터 비전, 시뮬레이션, 딥러닝**으로 풀어가고 있습니다.

현재는 가상 환경 속에서 사람과 물체를 생성하고, 그 환경에서 에이전트가 보고 움직이며 학습할 수 있는 파이프라인에 관심이 있습니다. 성능 수치만 남기는 것보다 **데이터가 어떻게 만들어졌는지, 어디서 실패하는지, 다음 사람이 어떻게 재현하는지**까지 기록하는 일을 좋아합니다.

## What I am building

```text
LLM prompt → Scene Graph → Unity Digital Twin → Mesh / Material
                                      ↓
SMPL shape + pose → motion mesh sequence → wireless simulation interface
```

가상 주거환경과 SMPL 기반 사람 애니메이션을 각각 검증한 뒤, 두 축을 하나의 시뮬레이션 씬으로 통합하는 연구를 진행하고 있습니다. 최종적으로는 실제 환경과 가상 환경에서 생성한 WiFi CSI·mmWave·Depth 데이터를 비교해, 가상 데이터가 3D human pose 추정에 얼마나 유효한지 확인하는 것이 목표입니다.

## Featured work

| Project | What I explored | Stack |
| --- | --- | --- |
| [MM-Fi × Sionna RT](https://github.com/dbwofla11/Comvision_Lab_MMFI_DTpose_withSionna) | 실제 주거환경과 가상 환경을 연결해 WiFi CSI 기반 3D human pose 연구의 데이터·시뮬레이션 파이프라인을 설계했습니다. | `Python` `PyTorch` `TensorFlow` `Sionna RT` |
| [LCK Efficiency Analysis](https://github.com/dbwofla11/LCK-Efficiency-Analysis) | Oracle's Elixir와 Riot API 데이터를 바탕으로 선수 기여도(WAR), 자원 대비 효율, 메타 적응력을 분석했습니다. | `Python` `Pandas` `XGBoost` `SHAP` |
| [Fx-Fighter: EXIT](https://github.com/dbwofla11/Fx-Fighter_EXITgame) | 여름 게임 공모전에서 게임 루프와 플레이 경험을 직접 설계하고 구현했습니다. | `Unity` `C#` |
| [DeepLearning Training](https://github.com/dbwofla11/DeepLearning_Training) | ANN부터 Transformer 계열까지 밑바닥 구현을 통해 딥러닝 모델의 내부 동작을 공부했습니다. | `Python` `NumPy` `Jupyter` |
| [Campus Rent Analysis](https://github.com/dbwofla11/campus-rent-analysis) | 대학가 월세 데이터를 수집·정리하고 지역별 주거비 패턴을 분석했습니다. | `Python` `Pandas` `Jupyter` |

<details>
<summary><b>Research notes: SMPL · HoloDeck · Physical AI</b></summary>

<br />

- **SMPL**: 체형 파라미터 β와 자세 θ를 넣어 6,890개 정점의 사람 메쉬를 생성하는 forward pass를 NumPy로 직접 구현하고, 공식 구현과 최대 오차 `4.44e-16`으로 대조했습니다.
- **Motion generation**: 걷기·앉기·손 흔들기 동작을 절차적으로 생성하고, waypoint별 프레임 메쉬 시퀀스로 내보내는 파이프라인을 만들었습니다.
- **HoloDeck / AI2-THOR**: LLM 출력 가드레일, Scene Graph, Unity Digital Twin, Mesh export까지 이어지는 절차적 환경 생성 흐름을 재현했습니다.
- **검증 기준**: 좌표계·스케일·바닥 접지·가구 관통 여부·좌석 정렬을 렌더링과 self-check로 확인하며, “생성된다”에서 끝나지 않고 “시뮬레이션 입력으로 쓸 수 있는가”를 확인합니다.

</details>

## Learning roadmap

| Area | Topics I am studying |
| --- | --- |
| Representation learning | Self-supervised learning, SimCLR, BYOL, DINO, JEPA, linear probe, UMAP |
| Generative models | GAN, VAE, diffusion, DDPM, latent diffusion, motion generation |
| World models & Physical AI | World model, latent dynamics, digital twin, simulation, HoloDeck, AI2-THOR, Sionna RT |
| Agents & reinforcement learning | MDP, value function, Q-learning, DQN, PPO, planning, memory, tool use |
| Game systems | FSM, Behavior Tree, Utility AI, pathfinding, NPC interaction, player telemetry |

## Toolbox

<div align="center">

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch" />
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow" />
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="scikit-learn" />
<br />
<img src="https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white" alt="Unity" />
<img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white" alt="C Sharp" />
<img src="https://img.shields.io/badge/Blender-E87D0D?style=for-the-badge&logo=blender&logoColor=white" alt="Blender" />
<img src="https://img.shields.io/badge/Sionna%20RT-111827?style=for-the-badge" alt="Sionna RT" />
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />

</div>

## Repository archive

공부·프로젝트·백업 저장소를 분야별로 정리했습니다. 대표 작업은 위에, 전체 기록은 아래에 남겨두었습니다.

<details>
<summary><b>Game development & Unity</b></summary>

- [Fx-Fighter_EXITgame](https://github.com/dbwofla11/Fx-Fighter_EXITgame) · 게임 공모전
- [unity_study_private_repo](https://github.com/dbwofla11/unity_study_private_repo) · C# 기초와 게임 만들기
- [go_to_bed](https://github.com/dbwofla11/go_to_bed) · SSCC 해커톤
- [Test_gitgitKal](https://github.com/dbwofla11/Test_gitgitKal) · 칼레이도 게임 개발
- [unity_study_Datastruct](https://github.com/dbwofla11/unity_study_Datastruct) · Unity 자료구조 스터디

</details>

<details>
<summary><b>Data, AI & deep learning</b></summary>

- [Comvision_Lab_MMFI_DTpose_withSionna](https://github.com/dbwofla11/Comvision_Lab_MMFI_DTpose_withSionna) · WiFi CSI 3D pose
- [LCK-Efficiency-Analysis](https://github.com/dbwofla11/LCK-Efficiency-Analysis) · LCK 데이터 분석
- [deepLearning_project](https://github.com/dbwofla11/deepLearning_project) · 딥러닝 기반 렌즈 노이즈 제거
- [DeepLearning_Training](https://github.com/dbwofla11/DeepLearning_Training) · ANN부터 Transformer까지
- [campus-rent-analysis](https://github.com/dbwofla11/campus-rent-analysis) · 대학가 월세 분석
- [DaconBaseLine_LLM-gemma-7b-](https://github.com/dbwofla11/DaconBaseLine_LLM-gemma-7b-) · NLP·Transformer·LLM 학습
- [DataStructor](https://github.com/dbwofla11/DataStructor) · 자료구조 실습
- [baekjoon_study](https://github.com/dbwofla11/baekjoon_study) · 알고리즘 문제 풀이
- [aima-python](https://github.com/dbwofla11/aima-python) · 인공지능 입문 과제

</details>

<details>
<summary><b>Web, service & application</b></summary>

- [Project_Lilac_Front](https://github.com/dbwofla11/Project_Lilac_Front) · 라일락 프로젝트 프론트엔드
- [Project_Lilac_Back](https://github.com/dbwofla11/Project_Lilac_Back) · 라일락 프로젝트 백엔드
- [job-front](https://github.com/dbwofla11/job-front) · JOB 프로젝트 프론트엔드
- [Front_component](https://github.com/dbwofla11/Front_component) · Next.js 컴포넌트 모음
- [APP_developing_back](https://github.com/dbwofla11/APP_developing_back) · 앱 개발 공모전 백엔드
- [2023-2-spring-study](https://github.com/dbwofla11/2023-2-spring-study) · Spring Boot 스터디
- [2023-1-java-study](https://github.com/dbwofla11/2023-1-java-study) · Java 스터디

</details>

<details>
<summary><b>CS foundations & open-source practice</b></summary>

- [CPP_repo](https://github.com/dbwofla11/CPP_repo) · 고급 프로그래밍
- [system_programing_backup](https://github.com/dbwofla11/system_programing_backup) · 시스템 프로그래밍
- [open_repo](https://github.com/dbwofla11/open_repo) · 오픈소스 기초설계
- [2023-2-existing-members-renew](https://github.com/dbwofla11/2023-2-existing-members-renew) · 동아리 프로젝트
- [discord.py](https://github.com/dbwofla11/discord.py) · Discord API 학습

</details>

## GitHub activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=dbwofla11&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github&include_all_commits=true" height="165" alt="GitHub stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=dbwofla11&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" height="165" alt="Top languages" />

</div>

<br />

<div align="center">

함께 만들고, 측정하고, 검증하는 일을 좋아합니다.

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2563EB,100:0F172A&height=120&section=footer" alt="profile footer" width="100%" />

</div>
