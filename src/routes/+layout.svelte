<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to Homepage">Егор Тохтуев</a>
        <div class="nav-links">
            <a href="/about" class="link">Студент СГХТ</a>
            <a href="/blog" class="link">Живу в России</a>
            <a href="/projects" class="link">Портфолио</a>
            <a href="/contact" class="link">Незнаю</a>
        </div>
    </div>
</nav>

<div class="container">
    <!-- Page will be injected below -->
    <slot></slot>
</div>

<style>
    .container {
        max-width: 1400px;
        margin: 50px auto;
    }
</style>