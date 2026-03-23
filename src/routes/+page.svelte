<script>
    let downloadsShowMore = $state(false)
</script>

<main>
    <h1>sysfind.app</h1>

    <h2 id="download">Download</h2>
    <ul>
        <li>
            <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_x64-setup.exe">
                <img src="windows.png" width="48px" height="48px" alt="Windows">
            </a>
        </li>
        <li>
            <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_x64.dmg">
                <img src="apple.png" width="48px" height="48px" alt="MacOS">
            </a>
        </li>
        <li>
            <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_amd64.AppImage">
                <img src="tux.svg" width="48px" height="48px" alt="Linux">
            </a>
        </li>
    </ul>
    <button onclick={()=> downloadsShowMore = !downloadsShowMore}>More</button>
    {#if downloadsShowMore}
        <ul>
            <li>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_x64_en-US.msi">
                    <img src="windows.png" width="32px" height="32px"  alt="Windows MSI">
                    Windows MSI
                </a>
            </li>
            <li>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_aarch64.dmg">
                    <img src="apple.png" width="32px" height="32px" alt="MacOS Apple Silicon">
                    Apple Silicon
                </a>
            </li>
            <li>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_amd64.deb">
                    <img src="debian.svg" width="32px" height="32px" alt="Debian">
                    Debian/Ubuntu
                </a>
            </li>
            <li>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application-0.1.0-1.x86_64.rpm">
                    <img src="fedora.png" width="32px" height="32px" alt="Fedora">
                    Fedora
                </a>
            </li>
            <li>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_aarch64.AppImage">
                    <img src="tux.svg" width="32px" height="32px" alt="Linux ARM">
                    Linux ARM
                </a>
            </li>
            <li>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application_0.1.0_arm64.deb">
                    <img src="debian.svg" width="32px" height="32px" alt="Debian ARM">
                    Debian/Ubuntu ARM
                </a>
            </li>
            <li>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest/download/sysfind-application-0.1.0-1.aarch64.rpm">
                    <img src="fedora.png" width="32px" height="32px" alt="Fedora ARM">
                    Fedora ARM
                </a>
            </li>
            <li>
                <a href="https://github.com/Delfi-CH/sysfind-application/releases/latest">
                    <img src="github.png" width="32px" height="32px" alt="GitHub">
                    All Downloads
                </a>
            </li>
        </ul>
    {/if}

    <div>
        <p>© 2026-{new Date().getFullYear()} Delfi-CH (<a href="https://delfi.dev/">https://delfi.dev/</a>)</p>
        <a href="https://github.com/Delfi-CH/sysfind-application"><img src="github.png" width="32px" alt="GitHub">Source code</a>
    </div>
</main>

<style>

</style>