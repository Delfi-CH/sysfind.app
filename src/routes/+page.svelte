<script>
    import {slide} from "svelte/transition";

    let downloadsShowMore = $state(false)
</script>

<main>
    <div class="header">
        <img src="favicon.svg" alt="logo" width="64px" class="headerItem">
        <h1 class="headerItem">sysfind.app</h1>
        <p class="headerItem">A <a href="https://delfi.dev/" target="_blank">Delfi-CH</a> project</p>
    </div>

    <h2>Manage your Operating Systems</h2>

    <p>Sysfind lets you explore and download installers for a multitude of operating systems</p>

    <p>The sysfind desktop app is available for Windows, MacOS and Linux under the GNU General Public License</p>

    <img src="screenshot1.png" width="70%" alt="screenshot">

    <img src="screenshot2.png" width="70%" alt="screenshot">

    <h2 id="download">Download</h2>
    <ul class="commonDownloads">
        <li class="commonDownloadItem">
            <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_x64-setup.exe">
                <img src="windows.png" width="48px" height="48px" alt="Windows">
            </a>
        </li>
        <li class="commonDownloadItem">
            <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_x64.dmg">
                <img src="apple.png" width="48px" height="48px" alt="MacOS">
            </a>
        </li>
        <li class="commonDownloadItem">
            <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_amd64.AppImage">
                <img src="tux.svg" width="48px" height="48px" alt="Linux">
            </a>
        </li>
    </ul>
    <button onclick={()=> downloadsShowMore = !downloadsShowMore} class="showMoreDownloads">More Downloads</button>
    {#if downloadsShowMore}
        <ul class="commonDownloads" transition:slide>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_x64_en-US.msi">
                    <img src="windows.png" width="32px" height="32px"  alt="Windows MSI">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_x64_en-US.msi"><span>Windows MSI</span></a>
            </li>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_aarch64.dmg">
                    <img src="apple.png" width="32px" height="32px" alt="MacOS Apple Silicon">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_aarch64.dmg"><span>Apple Silicon</span></a>
            </li>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_amd64.deb">
                    <img src="debian.svg" width="32px" height="32px" alt="Debian">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_amd64.deb"><span>Debian/Ubuntu</span></a>
            </li>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application-0.1.0-1.x86_64.rpm">
                    <img src="fedora.png" width="32px" height="32px" alt="Fedora">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application-0.1.0-1.x86_64.rpm"><span>Fedora</span></a>
            </li>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_aarch64.AppImage">
                    <img src="tux.svg" width="32px" height="32px" alt="Linux ARM">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_aarch64.AppImage"><span>Linux ARM</span></a>
            </li>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_arm64.deb">
                    <img src="debian.svg" width="32px" height="32px" alt="Debian ARM">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_arm64.deb"><span>Debian/Ubuntu ARM</span></a>
            </li>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application-0.1.0-1.aarch64.rpm">
                    <img src="fedora.png" width="32px" height="32px" alt="Fedora ARM">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application-0.1.0-1.aarch64.rpm"><span>Fedora ARM</span></a>
            </li>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/tree/main?tab=readme-ov-file#build-from-source" target="_blank">
                    <img src="github.png" width="32px" height="32px" alt="Build from Source">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/tree/main?tab=readme-ov-file#build-from-source"><span>Build from Source</span></a>
            </li>
            <li class="uncommonDownloadItem">
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest" target="_blank">
                    <img src="github.png" width="32px" height="32px" alt="GitHub">
                </a>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest" target="_blank"><span>All Downloads</span></a>
            </li>
        </ul>
    {/if}

    <p class="buffer"></p>

    <div class="footer">
        <p class="footerItem">© 2026-{new Date().getFullYear()} Delfi-CH (<a href="https://delfi.dev/" target="_blank">https://delfi.dev/</a>)</p>
        <a href="https://github.com/Delfi-CH/sysfind-application" target="_blank" class="footerItem"><img src="github.png" width="32px" alt="GitHub">Source code</a>
    </div>
</main>

<style>
    :root {
        background: #131416;
        color: white;
    }

    .header {
        border: 5px solid blue;
        background: rgb(0, 132, 255);
        border-radius: 2rem;
        display: flex;
        flex-direction: row;
        color: white;
    }
    .headerItem {
        align-self: end;
        margin: 0.5rem;
    }

    .headerItem a {
        color: darkblue;
    }

    .commonDownloads {
        border: 5px solid blue;
        background: lightgray;
        border-radius: 2rem;
        display: flex;
        flex-direction: row;
        margin: 1rem;
        padding: 0.5rem;
        width: fit-content;
    }
    .commonDownloadItem {
        list-style: none;
        padding: 0.5rem;
        transition: 0.2s;
    }
    .commonDownloadItem:hover {
        scale: 130%;
    }

    .showMoreDownloads {
        border: 5px solid blue;
        border-radius: 2rem;
        padding: 0.5rem;
        font-size: 100%;
        background: rgb(0, 132, 255);
        color: white;
        transition: 0.2s;
        margin-left: 1rem;
    }

    .showMoreDownloads:hover {
        background-color: rgb(0, 132, 255, 0.8);
        cursor: pointer;
    }

    .uncommonDownloadItem {
        text-align: center;
        list-style: none;
        padding: 0.7rem;
        transition: 0.2s;
        display: flex;
        flex-direction: column;
    }

    .uncommonDownloadItem:hover {
        scale: 120%;
    }

    .uncommonDownloadItem a {
        color: darkblue;
    }

    .uncommonDownloadItem a:visited {
        color: dodgerblue;
    }

    .footer {
        position: fixed;
        bottom: 0;
        left: 0;
        right: 0;
        background: rgb(0, 132, 255);
        display: flex;
        flex-direction: column;
        color: white;
        margin-top: 1rem;
    }

    .buffer {
        margin-bottom: 10rem;
    }

    .footerItem {
        margin: 0.2rem;
        padding: 0.3rem;
    }

    .footerItem a {
        color: darkblue;
    }

</style>