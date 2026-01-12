<script>
    import wicsLogo from '../assets/wics_logo.png'
    
    let menuOpen = false;
    
    function toggleMenu() {
        menuOpen = !menuOpen;
    }
</script>

<nav>
    <div class="navbar">
        <a href="/">
            <img src={wicsLogo} class="logo" alt="WiCS Logo" />
        </a>
        <button class="hamburger" on:click={toggleMenu} aria-label="Toggle menu">
            <span class={menuOpen ? 'open' : ''}></span>
            <span class={menuOpen ? 'open' : ''}></span>
            <span class={menuOpen ? 'open' : ''}></span>
        </button>
        <div class="pages" class:menu-open={menuOpen}>
            <a href="/about" class="about">
                About
            </a>
            <a href="/events" class ="events">
                Events
            </a>
            <a href="/resources" class ="resources">
                Resources
            </a>
            <button class="join-mobile">
                Join Us
            </button>
        </div>
        <button class="join">
            Join Us
        </button>
    </div>
</nav>
<style>
    nav {
        position: relative;
        top: 0;
        left: 0;
        width: 100vw;
        margin-left: calc(-50vw + 50%);
        z-index: 1000;
        background-color: #FDF7FA;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }
    .navbar {
        display: flex;
        align-items: center;
        align-content: center;
        padding: 0.5rem;
        max-width: 100%;
    }
    .hamburger {
        display: none;
        flex-direction: column;
        background: none;
        border: none;
        cursor: pointer;
        gap: 5px;
        padding: 8px;
        z-index: 1001;
    }
    
    .hamburger span {
        width: 25px;
        height: 3px;
        background-color: rgb(61, 60, 60);
        border-radius: 2px;
        transition: all 0.3s ease;
    }
    
    .hamburger span.open:nth-child(1) {
        transform: rotate(45deg) translate(8px, 8px);
    }
    
    .hamburger span.open:nth-child(2) {
        opacity: 0;
    }
    
    .hamburger span.open:nth-child(3) {
        transform: rotate(-45deg) translate(7px, -7px);
    }
    
    .pages {
        font-size: 16px;
        display: flex;
        gap: 2rem;
        padding-left: 30px;
        padding-bottom: 7px;
    }
    
    .pages a {
        text-decoration: none;
        color: rgb(61, 60, 60);
    }
    
    .join-mobile {
        display: none;
    }
    
    .join {
        background-color: #F6A9CB;
        width: 125px;
        border: 1px solid #FF79B4;
        border-radius: 5px;
        color: white;
        font-weight: 600;
        padding: 0.5rem 1rem;
        font-size: 16px;
        border-radius: 10px;
        margin-left: auto;
        cursor: pointer;
    }
    .join:hover {
        transform: translateY(-2px);
        background-color: #FDF7FA;
        border: 1px solid #FF79B4;
        color: #F6A9CB;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }
    .logo {
        height: 40px;
        width: auto;
        padding-left: 20px;
    }
    
    @media (max-width: 767px) {
        .hamburger {
            display: flex;
            margin-left: auto;
            margin-right: 1rem;
        }
        
        .pages {
            position: fixed;
            top: 60px;
            left: 0;
            width: 100%;
            background-color: #FDF7FA;
            flex-direction: column;
            padding: 2rem;
            gap: 1.5rem;
            border-top: 1px solid rgba(61, 60, 60, 0.1);
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transform: translateX(-100%);
            transition: transform 0.3s ease;
            z-index: 999;
        }
        
        .pages.menu-open {
            transform: translateX(0);
        }
        
        .pages a {
            padding: 0.5rem 0;
            width: 90%;
            border-bottom: 1px solid rgba(61, 60, 60, 0.1);
        }
        
        .join {
            display: none;
        }
        
        .join-mobile {
            display: block;
            background-color: #F6A9CB;
            width: 70%;
            border: 1px solid #FF79B4;
            border-radius: 10px;
            margin-left: 1rem;
            margin-right: 1rem;
            font-size: 16px;
            font-weight: bold;
            color: white;
            cursor: pointer;
            margin-top: 1rem;
            box-shadow: 0 2px 4px rgba(246, 169, 203, 0.3);
        }
        
        .join-mobile:hover {
            transform: translateY(-2px);
            background-color: #FDF7FA;
            border: 1px solid #FF79B4;
            color: #F6A9CB;
            box-shadow: 0 4px 8px rgba(246, 169, 203, 0.4);
        }
    }
</style>