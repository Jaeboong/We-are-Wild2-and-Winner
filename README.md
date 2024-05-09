# Wild2 팀

### 시나리오

```
김지영은 고려대학교 세종캠퍼스의 학생으로, 캠퍼스 내에서 개선이 필요한 사항이나 불만 사항을 학교 관리자에게 알리고자 합니다.
그러기 위해 캠퍼스 신문고 서비스를 이용하려고 합니다.
```

### 기능리스트

1. 게시글 생성 (**`/api/posts/create`**)
    - **요청 방식:** POST
    - **요청 데이터:**
        - **`title`**: 게시글 제목
        - **`content`**: 게시글 내용
    - **응답 데이터:** 생성된 게시글 ID 및 성공 여부 메시지
2. 투표 (**`/api/posts/{post_id}/vote`**)
    - **요청 방식:** POST
    - **요청 데이터:**
        - **`option`**: 투표 옵션
    - **응답 데이터:** 투표 결과 및 성공 여부 메시지
3. 댓글 (**`/api/posts/{post_id}/comments`**)
    - **요청 방식:** POST
    - **요청 데이터:**
        - **`comment`**: 댓글 내용
    - **응답 데이터:** 생성된 댓글 ID 및 성공 여부 메시지
4. 내 정보 페이지 (**`/api/user/profile`**)
    - **요청 방식:** GET
    - **요청 데이터:** 없음
    - **응답 데이터:** 사용자 프로필 정보
5. 설문조사 생성 및 관리 (**`/api/surveys`**)
    - **요청 방식:** POST
    - **요청 데이터:**
        - **`question`**: 설문조사 질문
        - **`options`**: 선택 옵션 (객관식 등)
    - **응답 데이터:** 생성된 설문조사 ID 및 성공 여부 메시지
6. 분석 및 보고 (**`/api/reports`**)
    - **요청 방식:** GET
    - **요청 데이터:** 없음
    - **응답 데이터:** 신문고 내용 분석 보고서 및 시각화 결과
