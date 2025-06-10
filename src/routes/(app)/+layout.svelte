<script>
    // No additional script logic needed for this static layout
</script>

<header>
    <div class="search-section">
        <div class="search-bar">
            <input type="text" placeholder="통합검색" />
            <button>검색</button>
        </div>
    </div>
    <nav class="navbar">
        <a href="/" class="logo">
            <img src="/logo.png" alt="Logo" style="height: 40px; filter: invert(1);" />
            <p>이과 커뮤니티 Dell</p>
        </a>
        <ul>
            <li><a href="/">홈</a></li>
            <li><a href="/community">커뮤니티</a></li>
            <li><a href="/qna">문의사항</a></li>
            <li><a href="/resources">자료시</a></li>
        </ul>
    </nav>
</header>

<slot />

<footer class="footer">
    <p>© 2025 이과 커뮤니티 | All Rights Reserved</p>
</footer>

<style>

    /* :global(html, body) {
        margin: 0;
        padding: 0;
        overscroll-behavior: none;
    }

    :global(*) {
        box-sizing: border-box;
    } */

    :root {
        --primary-color: #2c3e50; /* Deep elegant blue */
        --accent-color: #3b82f6; /* Vibrant coral accent */
        --gold-accent: #3b82f6; /* Luxurious gold */
        --text-color: #ecf0f1; /* Soft off-white */
        --bg-color: #ffffff;
        --search-bg: #34495e; /* Darker sophisticated search bg */
        --footer-bg: #2c3e50;
        --footer-text: #bdc3c7;
        --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    header {
        background: var(--primary-color);
        padding: 1rem 2rem;
        padding-top: 1.5rem;
        position: sticky;
        top: 0;
        z-index: 100;
        box-shadow: var(--shadow);
        border-bottom: 2px solid var(--gold-accent);
    }

    .search-section {
        margin-bottom: 1rem;
        text-align: center;
    }

    .search-bar {
        display: inline-flex;
        align-items: center;
        background: var(--search-bg);
        padding: 0.4rem 0.6rem;
        border-radius: 8px;
        box-shadow: var(--shadow);
        border: 1px solid var(--gold-accent);
        transition: transform 0.2s ease;
    }

    .search-bar:hover {
        transform: scale(1.05);
    }

    .search-bar input {
        border: none;
        background: transparent;
        outline: none;
        flex: 1;
        color: var(--text-color);
        font-family: 'Arial', sans-serif;
        font-size: 1rem;
        padding: 0 0.5rem;
    }

    .search-bar button {
        background: var(--accent-color);
        border: none;
        padding: 0.4rem 0.8rem;
        color: var(--text-color);
        cursor: pointer;
        border-radius: 6px;
        font-family: 'Arial', sans-serif;
        font-weight: bold;
        transition: background 0.3s ease;
    }

    .search-bar button:hover {
        background: #2563eb;
    }

    .navbar {
        display: flex;
        align-items: center;
        justify-content: space-between;
        flex-wrap: wrap;
        max-width: 1200px;
        margin: 0 auto;
    }

    .logo {
        display: flex;
        align-items: center;
        text-decoration: none;
        color: white;
        font-size: 1.5rem;
        font-weight: 700;
        letter-spacing: 1px;
    }

    .logo p {
        margin: 0;
        padding: 0 0.8rem;
        text-transform: uppercase;
    }

    nav ul {
        list-style: none;
        display: flex;
        gap: 1.5rem;
        margin: 0;
        padding: 0;
    }

    nav ul li a {
        text-decoration: none;
        color: var(--text-color);
        font-family: 'Arial', sans-serif;
        font-weight: 600;
        font-size: 1.1rem;
        position: relative;
        transition: color 0.3s ease;
    }

    nav ul li a:hover {
        color: var(--accent-color);
    }

    nav ul li a::after {
        content: '';
        position: absolute;
        width: 0;
        height: 2px;
        bottom: -5px;
        left: 0;
        background: var(--accent-color);
        transition: width 0.3s ease;
    }

    nav ul li a:hover::after {
        width: 100%;
    }

    .footer {
        padding: 1.5rem;
        background-color: var(--footer-bg);
        color: var(--footer-text);
        font-size: 0.95rem;
        text-align: center;
        border-top: 2px solid var(--gold-accent);
        box-shadow: var(--shadow);
        
    }

    
</style>