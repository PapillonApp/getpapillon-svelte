<script>
    import PapillonLogo from '$lib/assets/logo.svg';
    import { page } from '$app/stores';

    import DownloadCta from './download_cta.svelte';

    let path;
    $: path = $page.url.pathname;

    const paths = [
        {
            name: 'L\'application',
            path: '/'
        },
        {
            name: 'L\'équipe Papillon',
            path: '/team'
        },
        {
            name: 'Documentation',
            path: 'https://docs.getpapillon.xyz'
        },
    ];
</script>

<div class="navbar width">
    <div class="navbar-left">
        <img src={PapillonLogo} alt="Papillon" />

        <div class="nav-separator no-mobile"></div>

        <ul class="no-mobile">
            {#each paths as { name, path }}
                <li class="no-mobile">
                    <a href={path} class:active={path === $page.url.pathname}>{name}</a>
                </li>
            {/each}
        </ul>
    </div>

    <div class="navbar-right">
        <DownloadCta />
    </div>
</div>

<style>
    .navbar {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 16px 0;
    }

    .navbar-left {
        display: flex;
        align-items: center;
        gap: 24px;
    }

    .navbar-right {
        display: flex;
        align-items: center;
        gap: 24px;
    }

    .navbar img {
        height: 20px;
    }

    .nav-separator {
        width: 1px;
        height: 28px;
        background-color: #ffffff55;
    }

    .navbar ul {
        display: flex;
        gap: 24px;
    }

    .navbar li {
        list-style: none;
    }

    .navbar a {
        text-decoration: none;
        color: #ffffff;
        opacity: 0.5;
    }

    .navbar a:hover {
        opacity: 1;
    }

    .navbar a.active {
        opacity: 1;
        font-weight: 500;
    }

    @media (max-width: 768px) {
        .no-mobile {
            display: none;
        }
    }
</style>