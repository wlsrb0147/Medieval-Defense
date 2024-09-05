# 목차

1. 프로젝트 설명
2. pdf파일 / 시연영상
3. 제작과정 및 로직

# 1. 프로젝트 설명
중세시대의 좀비 액션게임을 제작하였습니다.</br>
플레이어는 트랩을 설치하거나, 활 또는 검을 이용하여 적을 처치합니다</br>
적은 5종류의 좀비와 1종의 보스가 있으며, 보스를 잡을경우 게임이 종료됩니다.</br>

저는 레벨 디자인 및 레벨 시퀀스, NPC 기초시스템 제작을 담당하였습니다.</br>

# 2. pdf파일 / 시연영상, 시연 방법

pdf 파일 : https://drive.google.com/file/d/1Bci_4wUgLTYvMpogvJuFYjQqZ_Md_1BF/view?usp=sharing</br>

시연 영상 : https://youtu.be/gmzcJQ1fW20?si=tligykyq4C6KI9hz</br>

Contents/01_Level/M_Entry_01 을 실행하면 됩니다.</br>
Numpad 7을 누르면 레벨시퀀스가 스킵됩니다.</br>
맵 정면의 끝에있는 보스를 처치하면 게임이 클리어됩니다.</br>
보스는 Numpad /를 누르면 즉사합니다.</br>

# 3. 제작 결과물

### 레벨 시퀀스 재생 위치</br>
![image](https://github.com/user-attachments/assets/a70d5990-b219-4234-87ff-d0fbbf4d3f70)</br>
BP_Scene Trigger : Content/02_Actor/04_Trigger/BP_SceneTrigger.uasset</br>
BP_BossTrigger : Content/02_Actor/05_FieldObject/BP_BossTrigger.uasset</br>
MorigeshPlayerCharacter :Content/ParagonMorigesh/Characters/Heroes/Morigesh/MorigeshPlayerCharacter.uasset</br>
GI : Content/00_Game/GI_TempGI.uasset</br>

### 레벨 시퀀스 위치</br>
Content/06_LevelSequence의 01,02,03,04 - Root 파일</br>

### Spline Wall</br>
오브젝트의 Spline에 따라 Mesh가 배치됩니다. </br>
![image](https://github.com/user-attachments/assets/f1abe95a-9354-41e9-b45e-1c5d7f7ad484)</br>
위치 : Content/02_Actor/05_FieldObject/BP_SplineWall3.uasset - OnConstruct</br>

### 엔피씨 대화</br>
![image](https://github.com/user-attachments/assets/1313cddb-5d00-429d-be58-e30924be7182)</br>
04_Widget/01_Widget/WBP_NPCConversation.uasset - 이벤트 그래프</br>

### 모델링한 작업물들 - Content/09_Materials/04_StaticMesh</br>

![image](https://github.com/user-attachments/assets/c349f1f5-ab37-4368-9147-0bb08b9ef0b2)</br>
![image](https://github.com/user-attachments/assets/f3c0101e-2c09-4b7f-a1a4-b737968a05d6)</br>

타워 : Content/09_Materials/04_StaticMesh/Tower/Complete</br>
성벽 : Content/09_Materials/04_StaticMesh/Wall/Wall_complete</br>
수문 : Content/09_Materials/04_StaticMesh/BaseMesh/SM_Portcullis2.uasset</br>

### 반복을 감춘 Landscape Material</br>
![image](https://github.com/user-attachments/assets/3cd3abbf-eeff-4fe6-a565-e554bc6041d4)</br>

경로 : Content/09_Materials/01_MaterialInstance/MI_BlendMaterial.uasset</br>

### 패턴을 반복시킨 성벽과 타워의 Material</br>
![image](https://github.com/user-attachments/assets/11885b8c-9c71-4e5e-81dd-924c80716769)</br>
경로
Content/09_Materials/01_MaterialInstance/MI_TowerWall.uasset</br>
Content/09_Materials/01_MaterialInstance/MI_Wall.uasset</br>
