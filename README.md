# GraduateProject

게임 타이틀 : Building Hacker

장르 : 액션 / 슈팅

플랫폼 : VR

타겟 플레이어 : 20대 남성 성인

게임의 기획적/기술적 특징 : 

# Tracking

이 게임은 VR 플랫폼으로 제작되어, 기존의 게임들과는 다르게 Hand Tracking과 관련된 부분들이 새로이 추가되어야 했습니다.

또한 플레이어의 움직임이 단순히 컨트롤러 조정에 국한되는 것이 아닌, 플레이어가 방을 직접 돌아다니며 이동할 수 있다는 점에서 여러가지 움직임의 상황에 대해 고려할 필요가 있었습니다.

이에따라 새로운 게임 플랫폼인 VR은 그에 걸맞는 새로운 조건들을 제시했고, 그에 맞춘 작업을 위해 추가적인 상황의 판단이 필요했습니다.

# AI

AI의 경우 Behaviour Tree를 사용하여 개발이 되었으며, State에 따라 대기, 순찰, 추적, 공격을 수행하도록 설정되어있습니다.

모든 AI의 이동은 Unity의 Navigation 기능을 통해 개발되었습니다.

또한 캐릭터 애니메이션의 경우에는 Animator 메카님을 통해 개발하여 Behaviour Tree의 State에 맞는 애니메이션이 재생되도록 설정하였습니다.

# 최적화

최적화를 위해 Light의 경우 RealLight를 배제하고 모두 BakedLight를 이용하였으며, 위치별 광원의 경우에는 LightProbe를 이용하여 위치에 따른 광원을 간접적으로 표현할 수 있도록 설정했으며, Reflection Probe를 사용하여 유리와 같은 부분의 반사를 표현했습니다.

또한, Render 자체를 구분하고 Render를 하지 않는 Occlusion Culling을 이용하여 큰 맵을 효과적으로 관리시킬 수 있도록 하여 최적화 시켰습니다.

# 유튜브 링크

https://www.youtube.com/watch?v=nEQKsRHrbvg
