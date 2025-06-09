<script>

</script>

<header>
    <nav class="navbar">
        <a href="/" class="logo">
            <img src="logo.png" alt="" style="height: 40px; padding-bottom: 0.3rem;">
            <p>이과 커뮤니티 Dell</p>
        </a>
        <ul>
            <li><a href="/">홈</a></li>
            <li><a href="/community">커뮤니티</a></li>
            <li><a href="/qna">문의사항</a></li>
            <li><a href="/resources">자료실</a></li>
        </ul>
    </nav>
</header>

<slot />

<footer class="footer">
    <p>&copy; 2025 이과 커뮤니티</p>
</footer>

<style>

    :root {
        --signature-color: #ccff00; 
        --text-color: #000;
        --bg-color: #ffffff;
        --footer-bg: #fafafa;
        --footer-text: #777;
    }

    header {
        background: var(--signature-color);
        padding: 0.5rem 2rem;
        position: sticky;
        top: 0;
        z-index: 100;
    }

    .navbar {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .logo {
        align-items: center;
        display: flex;
        text-decoration: none;
        color: #000;
        font-weight: bold;
        font-size: 1.4rem;
    }

    .logo p {
        margin: 0;
        padding: 0rem 0.5rem;
    }

    nav ul {
        flex: 1;
        align-items: center;
        justify-content: flex-end;
        list-style: none;
        display: flex;
        gap: 2rem;
    }

    nav ul li a {
        text-decoration: none;
        color: #000;
        font-weight: 600;
        font-size: 1.1rem;
    }

    nav ul li a:hover {
        text-decoration: underline;
    }

    .footer {
        padding: 1.5rem 2rem;
        background-color: var(--footer-bg);
        color: var(--footer-text);
        font-size: 0.9rem;
        text-align: center;
        border-top: 1px solid #e0e0e0;
        margin-top: 3rem;
    }
</style>
