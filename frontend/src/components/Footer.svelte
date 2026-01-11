<script>
    import emailIcon from '../assets/email.png'
    import instagramIcon from '../assets/insta.png'
    import facebookIcon from '../assets/facebook.png'
    import linkedinIcon from '../assets/linkedin.png'
    import discordIcon from '../assets/discord.png'
    import wicsLogo from '../assets/wics_logo.png'
</script>

<footer>
    <div class="footer-content">
        <div class="left-footer">
            <div class="logo-container">
                <a href="/">
                    <img src={wicsLogo} class="logo" alt="WiCS Logo" />
                </a>
                <h1 class="logo-text">Women in Computer Science</h1>
            </div>
            <div class="social-links">
                <a href="mailto:wicsdavis@gmail.com" aria-label="Email">
                    <img src={emailIcon} alt="Email" class="social-icon" />
                </a>
                <a href="https://instagram.com/wicsdavis" target="_blank" rel="noopener noreferrer" aria-label="Instagram">
                    <img src={instagramIcon} alt="Instagram" class="social-icon" />
                </a>
                <a href="https://discord.gg/BvDEaQgQQC" target="_blank" rel="noopener noreferrer" aria-label="Discord">
                    <img src={discordIcon} alt="Discord" class="social-icon" />
                </a>
                <a href="https://www.facebook.com/DavisWICS/" target="_blank" rel="noopener noreferrer" aria-label="Facebook">
                    <img src={facebookIcon} alt="Facebook" class="social-icon" />
                </a>
                <a href="https://www.linkedin.com/company/women-in-computer-science-at-ucd/" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn">
                    <img src={linkedinIcon} alt="LinkedIn" class="social-icon" />
                </a>
            </div>
        </div>
        <div class="right-footer">
            <div class="newsletter-container">
                <h1 class="newsletter-title">Join Our Newsletter</h1>
                <p class="newsletter-text">Receive weekly emails about our upcoming 
                    <br>events and opportunities!</p>
                <button class="newsletter-button">Sign Up</button>
            </div>
        </div>
    </div>
    <div class="footer-divider"></div>
    <div class="copyright-text">
        <p class="footer-text">© 2026 Women in Computer Science at UC Davis</p>
    </div>
</footer>

<style>
    footer {
        background-color: #FDF7FA;
        margin-top: auto;
        padding-top: 1rem;
        padding-bottom: 1rem;
        box-shadow: 0 -2px 4px rgba(0, 0, 0, 0.1);
        width: 100%;
        position: fixed;
        bottom: 0;
        left: 0;
        right: 0;
        z-index: 1000;
    }
    
    .footer-content {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1.3rem;
        max-width: 1200px;
        margin: 0 auto;
        padding-bottom: 1.5rem;
    }
    .logo-container {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 1rem;
        justify-content: center;
    }
    .logo-text {
        font-size: 20px;
        font-family: 'Montserrat', sans-serif;
        color: #5D5D5F;
        margin: 0;
        font-weight: 600;
        text-align: center;
    }

    .logo {
        width: auto;
        height: 30px;
    }

    .footer-text {
        color: #5D5D5F;
        font-size: 14px;
        margin: 0;
    }
    .left-footer {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 100%;
    }
    
    .right-footer {
        display: flex;
        align-items: flex-start;
        width: 100%;
        justify-content: center;
    }
    
    .newsletter-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        width: 100%;
    }
    
    .newsletter-title {
        color: #5D5D5F;
        font-family: 'Montserrat', sans-serif;
        font-size: 18px;
        font-weight: bold;
        margin: 0;
    }
    
    .newsletter-text {
        color: rgb(100, 100, 100);
        font-size: 14px;
        font-weight: normal;
        text-align: left;
        margin: 0;
        line-height: 1.5;
    }
    
    
    .newsletter-button {
        margin-top: 0.5rem;
        background-color: #F6A9CB;
        border: 1px solid #FF79B4;
        border-radius: 10px;
        padding: 0.75rem 1.5rem;
        font-size: 16px;
        font-weight: bold;
        color: white;
        cursor: pointer;
        box-shadow: 0 2px 4px rgba(246, 169, 203, 0.3);
        transition: transform 0.2s, box-shadow 0.2s;
    }
    
    .newsletter-button:hover {
        transform: translateY(-2px);
        background-color: #FDF7FA;
        border: 1px solid #FF79B4;
        color: #F6A9CB;
        box-shadow: 0 4px 8px rgba(246, 169, 203, 0.4);
    }
     
    .social-links {
        display: flex;
        gap: 0.75rem;
        align-items: center;
        justify-content: center;
    }
    
    .social-links a {
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 50%;
        transition: transform 0.2s;
        padding: 8px;
    }
    
    .social-icon {
        width: 35px;
        height: 35px;
    }
    
    .social-links a:hover {
        transform: scale(1.1);
    }
    
    a {
        display: inline-block;
    }
    
    .footer-divider {
        width: 90%;
        max-width: 1000px;
        margin: 0 auto;
        padding-top: 0.5rem;
        border-top: 1px solid rgba(93, 93, 95, 0.2);
    }
    
    .copyright-text {
        text-align: center;
        max-width: 1200px;
        margin: 0 auto;
        padding-top: 0.5rem;
    }
    
    @media (min-width: 768px) {
        .footer-content {
            flex-direction: row;
            padding-left: 2.5%;
            padding-right: 2.5%;
            justify-content: center;
            align-items: center;
            gap: 10rem;
            padding-top: 1rem;
            padding-bottom: 2rem;
        }
        
        .left-footer {
            align-items: flex-start;
            width: auto;
        }
        
        .right-footer {
            justify-content: flex-end;
            width: auto;
        }
        
        .newsletter-container {
            align-items: flex-start;
            text-align: left;
        }
        
        .newsletter-title {
            font-size: 20px;
        }
        
        .logo-container {
            justify-content: flex-start;
        }
        
        .logo-text {
            font-size: 24px;
            text-align: left;
        }
        
        .social-links {
            justify-content: flex-start;
        }
        
        .footer-text {
            font-size: 16px;
        }
        
        .social-icon {
            width: 35px;
            height: 35px;
        }
        
        .footer-divider {
            width: 95%;
            max-width: 1500px;
            margin: 1rem auto;
        }
        
        .copyright-text {
            text-align: left;
            margin-left: 3rem;
        }
    }

</style>