
[Role] 너는 PSSLAB의 AX² System 전문 웹 개발자야. 제공된 contents_db.md(상세 데이터베이스)를 분석하여 웹사이트 전체를 업데이트해.

[Input Files]

contents_db.md: 상세 설명(Summary_EN/KR)이 포함된 통합 DB.

index.html, article.html, report.html, paper.html 소스 코드.

[Instructions]

1. index.html 업데이트:

[Hero Slides]와 [Update] 섹션을 최신화해.

[Article/Report/Paper] 리스트에 신규 항목을 추가해 (여기서는 제목과 링크만 사용).

2. 하위 페이지(article/report/paper.html) 업데이트 (중요):

MD 파일의 각 섹션(Article, Report, Paper)에 있는 항목들을 해당 파일의 `` 구역에 반영해.

포스트 블록 생성: 각 항목마다 아래 형식을 지켜서 추가해.

HTML

<article class="post-block" id="post-[ID]">
    <div class="post-header">
        <h2>[Title]</h2>
        <span class="post-date">[Date]</span>
    </div>
    <div class="summary-content">
        [Summary_EN]
        <div class="summary-kr">[Summary_KR]</div>
    </div>
    <button onclick="openRequestModal('[Title]')" class="btn-request">Request Full Version (PDF)</button>
</article>
ID 매칭: id="post-[날짜/ID]"가 index.html의 링크 주소와 정확히 일치해야 해.

3. 기술적 제약 조건:

기존의 미니멀 모달(Modal) 기능과 CSS 레이아웃은 그대로 유지해.

모든 파일의 업데이트가 완료되면 수정된 전체 코드를 출력해줘.

