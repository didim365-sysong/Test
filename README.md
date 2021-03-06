---
description: 메인페이지 테스트를 위해 Tensorflow 내용을 insert 하였습니다.
---

# 메인페이지

tensorflow.org 문서를 한글로 번역하여 깃북으로 제공하기 위한 레파지토리입니다.

작업하려는 부분을 깃허브의 이슈에 등록하고 자유롭게 진행하려고 합니다. 여러 사람이 모여 진행을 하다보면 자연스럽게 어느정도 규칙적인 리듬을 가지게 될 수 있을거라 생각합니다. 이 프로젝트는 페이스북 [텐서플로우 그룹](https://www.facebook.com/groups/TensorFlowKR/)과 함께 진행하고 있습니다. 많은 분들이 참여해 주셨으면 좋겠습니다.

깃허브의 주소는 [https://github.com/tensorflowkorea/tensorflow-kr](https://github.com/tensorflowkorea/tensorflow-kr) 입니다.

깃북의 주소는 [https://tensorflowkorea.gitbooks.io/tensorflow-kr](https://tensorflowkorea.gitbooks.io/tensorflow-kr) 입니다.

깃허브의 작업 방법에 대해서는 [블로그 포스팅](https://tensorflowkorea.wordpress.com/2016/06/01/텐서플로우-문서-한글화/)을 참고해 주세요.

감사합니다.

## 번역 및 마크다운 참고사항

### 번역 범위

현재 텐서플로우는 버전이 빠르게 변하고 있어서 API 문서가 자주 변경됩니다. 따라서 가능하시면 api\_docs 폴더 이외의 다른 문서를 먼저 번역하는 것이 합리적으로 생각됩니다. 각 폴더별 번역 진행 상황은 [@hunkim](https://github.com/hunkim) 님께서 작업해 주신 [progress.md](https://github.com/didim365-sysong/Didimnow/tree/7f72501e401f79ba8fc30ec387d7a50f8f80b0b5/progress.md) 파일을 참고해 주세요. api\_docs 문서를 제외하고 번역이 완료되면 몇명이서 전체 번역을 다듬으려고 합니다. 이 때 필요한 자원봉사자를 페이스북 텐서플로우 그룹을 통해 신청받으려고 합니다.

### 버전 관리 안내

텐서플로우 버전이 업데이트 되면서 번역된 문서 간의 버전 차이가 있을 수 있습니다. master 브랜치에는 v0.9의 영문 문서가 들어가 있습니다. 그리고 master 브랜치외에 r0.9, r0.10 두개의 브랜치가 추가 되었습니다. 각각 v0.9, v0.10의 영문 문서가 담겨 있습니다. 두개의 브랜치를 비교하면서 기 번역된 문서를 업데이트 하거나 새로운 번역 문서를 추가할 수 있습니다.

master 브랜치의 번역 문서는 아래와 같이 번역된 버전을 제목 아래에 적어 주십시요. 만약 버전이 적혀있지 않을 경우에는 v0.9로 간주합니다.

```text
# 순환 신경망(Recurrent Neural Networks)
(v0.9)
```

### 아래 pip-installation의 경우처럼 페이지내 이동을 위해서 네임드 앵커 태그가 없이 사용만 되는 경우가 있습니다.

```text
*  [Pip 설치](#pip-installation): 이 방식으로 텐서플로우를 설치하거나 업그레이드할 때는
   이 전에 작성했던 파이썬 프로그램에 영향을 미칠 수 있습니다.
```

이럴 때에는 pip-installation 이 가리키는 위치에 네임드 앵커 태그를 넣어주시면 됩니다.

```text
...
<a id="pip-installation"></a>
## Pip Installation
...
```

