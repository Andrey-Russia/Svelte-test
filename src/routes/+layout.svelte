<script>
    const nav = [
        {
            title: "Обо мне",
            href: "/about",
            isShow: true,
        },
        {
            title: "Блог",
            href: "/blog",
            isShow: true,
        },
        {
            title: "Портфолио",
            href: "/project",
            isShow: true,
        },
        {
            title: "Контакты",
            href: "/contact",
            isShow: true,
        },
        {
            title: "temp",
            href: "/temp",
            isShow: false,
        },
    ];
</script>

<nav>
    <div class="nav-container">
        <!-- svelte-ignore missing-declaration -->
        {#each nav as link}
            {#if link.isShow}
                <a href={link.href} class="link">{link.title}</a>
            {/if}
        {/each}
    </div>
</nav>
<div class="container">
    <!-- Pages will be injected below -->
    <slot />
</div>

<style>
    .container {
        max-width: 1400px;
        margin: 50px auto;
    }
</style>
