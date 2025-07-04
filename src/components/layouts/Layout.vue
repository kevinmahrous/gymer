<template>
    <header>
        <div>
            <img src="../../assets/favicon.svg">
            <h1 class="text-gradient">Gymer</h1>
        </div>
    </header>
    <main>
        <slot />
    </main>
    <footer>
        <small>Created by</small>
        <a href="https://github.com/kevinmahrous" target="_blank">
            <i class="fa-brands fa-github"></i>
            <p>kevinmahrous</p>
        </a>
    </footer>
</template>

<style scoped>
header,
main,
footer {
    align-items: center;
    padding: 1rem;
    width: 100%;
    max-width: 600px;
    margin: 0 auto;
}

main {
    flex: 1;
}


header div {
    display: flex;
    align-items: center;
    gap: 1rem;
}

header img {
    width: 2rem;
    height: 2rem;
}

footer {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    align-items: center;
    padding: 2rem 0;
    padding-bottom: 3rem;
}

footer a {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.5rem;
    padding-right: 0.5rem;
    background: var(--background-muted);
    border-radius: 4rem;
    border: 1px solid transparent;
    transition-duration: 200ms;
    text-decoration: none;
}

footer a:hover {
    border-color: var(--color-link);
}
</style>