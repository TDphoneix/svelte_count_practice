<div class="header">
    <nav>
        <a href="/">home</a>
        <a href="/about">about</a>
        <a href="https://github.com" target="_blank">github</a>
    </nav>
</div>
<slot></slot>

<style>
    .header {
        width: calc(100% - 1rem);
        margin: 0.5rem;
        border:1px solid rgb(235, 235, 235);
        border-radius: 8px;
    }

    nav {
        display: flex;
        flex-flow: row nowrap;
        align-items: center;
        padding: 1rem 0.5rem;
    }

    a {
        font-size: 1rem;
        text-decoration: none;
        color: rgb(85, 85, 85);
        padding:0 1rem;
        
    }
</style>