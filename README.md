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

## 가장 중요한 내용

   1. 저는 깃헙에 대한 조금의 경험이 있습니다.
   1. 아마도 당신과 같은 사무실 공간에 앉아서 일을 하고 있습니다.
   1. 그리고 대부분 시간에 제게 깃헙에 새로운 프로젝트를 만들거나 실험을 해보고 싶은 내용이 있어 말을 걸어도 물거나 하지 않습니다.


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

'New repository'을 클릭하면 다음과 같은 **새로운 리포를 위한 설정을 시작합니다**:

![새로운 repo의 설정](/images/new-repo-form.png)


   * **Owner** : "Promedius-dev"은 저희 회사 Organization이고, 저기에 리포를 만들면 기본으로 저 Org에 속한 사람들은 모두 접근할 수 있어요.
   * **Repository name** : 적당한 영문명. 파일/디렉토리 이름 규칙처럼 어느 정도 제약이 있습니다. (깃헙이 체크해서 마음에 안들면 알려줍니다)
   * **Public** vs. **Private** : Public은 인터넷에 누구나에게 공개됩니다. Private은 Owner이 Org이라면, 그 Org에 속한 사람들에게만, Owner이 개인 계정이라면 그 개인계정에게만 보이도록 됩니다.

즉, "회사 내부에서만 공유하고 싶은 비밀 소스코드/프로젝트를 관리"하는게 목적이라면:

   1. Owner = Promedius-dev
   2. Repository name: 뭔가 멋진 것으로.
   3. **Private**

...와 같이 선택하시면 됩니다.


------

# 꼭 해보기: Audience type=1에게.

   1. [ ] 새로운 깃헙 리포를 만들어 보세요.
   1. [ ] 만든 리포에 다음과 같은 이슈를 등록해보세요:
      1. "점심 고르기"
	    2. "점심 먹기"
	    3. "인류를 구원하기"
   1. [ ] 만든 이슈들에 적당한 내용을 적어보세요. (자유서술, 3점)
      * 참고: https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax
   1. [ ] 이슈의 본문을 작성하실 때, Drag and Drop으로 이미지를 넣어보세요. (강아지-고양이 사진일 경우 1점, 귀여울 경우 3점)
   1. [ ] 만든 이슈들에 다음 "**Label**", "**Milestone**"을 적절하게 할당해보세요.
      1. Labels: TODO, LUNCHING, DAILY_ROUTINE 중 하나 이상.
      2. Milestones: 다음 중 하나.
         1. Today
         1. Release-Alpha: due date은 2020년 2월 29일으로.
   1. [ ] 위 이슈끼리 관계를 연결하세요: "점심 고르기" 이슈를 "점심 먹기"의 본문이나 코멘트에서 언급하세요.
      * 참고: https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax#referencing-issues-and-pull-requests
   1. [ ] "점심 고르기" 이슈에 저 ( @jhyun-promedius )를 언급하시고, 해당 이슈 본문에 대한 질문과 답변, 논의를 코멘트에서 진행해보세요.

------

# 살펴보기: Projects, Wiki

새로 만든 Repo의 Projects, Wiki 메뉴 항목을 살펴보고,

   1. 이전에 "꼭 해보기"에서 만든 이슈들을 어떻게 프로젝트를 만들고 배열할 수 있는지 살펴보세요.
      * 참고: "칸반 이야기" https://brunch.co.kr/@seonology/6

깃헙에서 위키를 작성하는 것, 위키 페이지끼리 링크를 만드는 것, 위키 페이지에 내용과 첨부 파일/이미지를 넣는 것 정도를 더 검색해보세요.


**간단한 깃헙쑈오가 끝났습니다. 수고하셨습니다.**

------
# --- 절취선 --- 여기부터는 "소스코드를 갖고 협업하기"에 대한 내용입니다.

안녕하세요. 코드를 만지셔야 하는 분들.

여러분들에게도 과제를 드리고 싶습니다.

  1. [ ] 이 저장소( https://github.com/jhyun-promedius/github-show )를 "Fork"해보세요.
  1. [ ] Fork한 저장소는 원래의 저장소와 어떻게 연결되는지 깃헙에서 살펴보고 생각해보세요.
  1. [ ] 각각 개인 계정으로 Fork한 저장소에서 이 파일 `README.md` 파일을 적당히 수정해서, 저에게 "Pull request"을 요청해보세요.
     * "Pull request" 소개: https://wayhome25.github.io/git/2017/07/08/git-first-pull-request-story/
     * 오타나 맞춤법, 띄워씌기가 틀렷거나 한 부분을 고쳐 주셔도 조아여, 아니면 없는 섹션을 추가해서 기여해주셔도 좋습니다.
     * 보내주신 Pull request에서 제가 의견을 드리고 또 그걸 수정하여 Merge하여 결국 이 저장소에 반영할겁니다.

화이팅!

