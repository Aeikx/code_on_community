<script>

</script>

<main>
    <aside class="sidebar">
        <nav>
            <section>
            <h2>수학 커뮤니티</h2>
            <ul>
                <li><a href="/math/basic">수1 수2 미적분</a></li>
                <li><a href="/math/questions">질문 게시판</a></li>
                <li><a href="/math/tips">팁 게시판</a></li>
                <li><a href="/math/info">정보 게시판</a></li>
                <li><a href="/math/challenge">문제 도전!</a></li>
            </ul>
            </section>
            <section>
            <h2>과학 커뮤니티</h2>
            <ul>
                <li><a href="/science/basic">물리 화학 생명 지구</a></li>
                <li><a href="/science/questions">질문 게시판</a></li>
                <li><a href="/science/tips">팁 게시판</a></li>
                <li><a href="/science/info">정보 게시판</a></li>
                <li><a href="/science/challenge">문제 도전!</a></li>
            </ul>
            </section>
        </nav>
    </aside>
    <section class="page">
        <slot />
    </section>
</main>



<style>
    main {
        display: flex;
        height: 100vh;
    }

    .page {
    flex: 1;
    overflow-y: auto; /* 오른쪽 컨텐츠 스크롤 */
    padding: 20px;
    height: 100vh;
    }

    .sidebar {
    width: 200px;
    background-color: #f9f9f9;
    padding: 20px;
    border-right: 1px solid #ddd;
    position: sticky;
    top: 0;
    height: 100vh; /* 뷰포트 높이 고정 */
    overflow-y: auto; /* 사이드바 길어지면 스크롤 */
    flex-shrink: 0;
    }

    .sidebar nav {
    display: flex;
    flex-direction: column;
    gap: 40px;
    }

    .sidebar h2 {
    font-size: 18px;
    margin-bottom: 10px;
    font-weight: bold;
    }

    .sidebar ul {
    list-style: none;
    padding: 0;
    margin: 0;
    }

    .sidebar li {
    margin: 8px 0;
    }

    .sidebar a {
    text-decoration: none;
    color: #333;
    font-size: 16px;
    }

    .sidebar a:hover {
    text-decoration: underline;
    }

</style>