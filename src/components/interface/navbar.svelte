<script>
    import PapillonLogo from '$lib/assets/logo.svg';
    import { page } from '$app/stores';

    import DownloadCta from './download_cta.svelte';
    import Error from '../../routes/+error.svelte';

    let path;
    $: path = $page.url.pathname;

    const paths = [
        {
            name: 'L\'application',
            path: '/'
        },
        {
            name: 'Documentation',
            path: 'https://docs.getpapillon.xyz'
        },
        {
            name: 'Blog',
            path: 'https://blog.getpapillon.xyz/'
        },
    ];
</script>

<div class="navbar width">
    <div class="navbar-left">
        <a href="/" style="opacity: 1;">
            <img src={PapillonLogo} alt="Papillon" />
        </a>

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
        <div>
            <DownloadCta />
        </div>
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
        height: 22px;
        margin-top: 2px;
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
        .navbar {
            padding: 24px 0;
        }
    }
</style>
