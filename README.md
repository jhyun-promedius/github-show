# the "github show"

## (Target audiences) 우선 이 글을 읽었으면 좋겠는 사람:

   1. GitHub에서 **이슈관리, 프로젝트 대시보드** 같은 용도로 관심 있는 사람.
   2. 위 (1)은 물론 깃헙과 Git을 이용해 소스코드를 다른 사람과 공동 작업을 할 사람.


## 그에 맞춰 이야기 하려는 범위:

   * [Git](https://git-scm.com/) 소스코드 관리 시스템을 소개하지도, 어떻게 잘 쓸 수 있는지 설명 안함.
     * 이 주제는 인터넷에 이미 좋은 문서들이 많아요.
     * 이상의 "_Target audiences_"에서 (2)에 속하는, 소스코드 공동작업에 관심이 있는 분들은 이미
       Git에 약간은 익숙하다는 전제로 이야기할게요.
     * Git 사용법은 코드를 직접 다루는 사람에게는 필요한 지식이지만 모두 알 필요는 없습니다.
     * Git 사용에 대해서는 제게 직접 대화를 걸어주셔도 언제든지 좋습니다.
   * (Git에는 익숙하다는 전제를 갖고) GitHub에서 어떻게 소스코드 공동작업을 정리하는지만 이야기 합니다.


-----

# "Repo을 만들자"

> "Make repo, not war."

새로운 저장소를 만드는데 익숙해지세요. (저희가 사용하는 가격정책에서는 저장소의 갯수, 용량은 무제한입니다.)

저장소가 창피해졌거나 해서 없애고 싶다면 금방 없애거나, 비공개 상태로 만들기 쉬워요. (하지만 그 설명은 이번엔 생략하겠습니다.)

앞으로 이야기 하는 단어들 중에서 조금 혼란스러운 것들만 의미를 정리해볼게요:

단어 | 뜻
-----|-----------
**Repo** 혹은 "**저장소**" | GitHub repository, 깃헙 사용에서 각 프로젝트, 소스코드 모듈 등등을 분리하는 단위
**(GitHub) Project** | 일반적인 "프로젝트"와 달리 고유명사로, 깃헙 Repo의 "Projects" 메뉴 항목. 이슈들을 카테고리별로 옮겨서 분류하고 대시보드를 만들 수 있어요


결국, **Repo** >= **Project** 관계가 생겨요. (한 리포에는 한개 이상의 프로젝트가 딸림.)
'프로젝트'라는 단어가 우리가 흔히 일상적으로 말하는 단어는 범위가 큰데, 여기서는 '대시보드', '이슈들을 내가 원하는 것들만 골라 임의로 배열한 묶음' 정도로 많이 다르니 이걸 갖고 너무 집착하지는 말기로 하죠.



## 화면: Repo을 만들기 위한 여정

이미 작업하는 리포가 있다면 그냥 깃헙에서 *잘* 찾아 들어가시면 됩니다.

하지만 새로운 리포를 만드는데는 매우 복잡한 지식이 필요합니다. 우선 새 리포를 만드는 버튼은 깃헙 화면의 우측 상단에 다음과 같은 '+' 모양 버튼을 클릭해주세요:

![어디에 '+'버튼이 있는가](/images/new-repo.png)


여러가지 항목들이 있지만 이번에는 설명하지 않겠습니다:

'New repository'을 클릭하면 다음과 같은 새로운 리포를 위한 설정을 시작합니다:

![새로운 repo의 설정](/images/new-repo-form.png)


------

# --- 절취선 --- 여기부터는 "소스코드를 갖고 협업하기"에 대한 내용입니다.

