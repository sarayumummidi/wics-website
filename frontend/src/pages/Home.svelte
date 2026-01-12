<script>
    import wicsWebsiteDesign from '../assets/wicswebsite.png'
</script>

<div class="home">
    <img src={wicsWebsiteDesign} class="webDesign" alt="WiCS Website Design" />
    <div class="homeText">
        <div class="text-container">
            <p class="wics-welcome">Welcome! We are </p>
            <p class="wics-name">Davis Women in Computer Science</p>
        </div>
        <div class="wics-description-container">
            <p class="wics-description">
                <span class="wics-bold-text">Women in Computer Science (WiCS)</span> 
                supports, empowers and motivates the growing community of women in computer science. 
                <br />
                <br />
                We aim to prepare women for tech industry, in addition to inspiring women to explore educational and professional opportunities in computing through creating a powerful community, providing mentorship and helping them to succeed. We aim to grow, learn and spread the joy of computer science together!
            </p>
            <a href="/about" class="about-button"> About Us <span class="arrow">→</span> </a>
        </div>
    </div>
</div>

<style>
    .home {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        background-color: #FDF7FA;
    }
    .webDesign {
        width: 120%;
        height: 120%;
    }
    .text-container {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
    }
    .wics-welcome {
        font-size: 48px;
        font-weight: 300;
        color: #666666;
        margin: 0;
    }
    .wics-name {
        font-size: 48px;
        color: #666666;
        font-weight: 600;
        margin: 0;
    }
    .homeText {
        display: flex;
        flex-direction: column;
        margin-top: 5%;
        margin-left: 5%;
        margin-right: 10%;
        margin-bottom: 5%;
    }
    .wics-description-container {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        gap: 10px;
    }
    .wics-description {
        font-size: 20px;
        color: #666666;
        font-weight: 400;
        margin: 0;
    }
    .wics-bold-text {
        font-weight: 600;
    }
    .about-button {
        font-size: 20px;
        color: #FF79B4;
        font-weight: 500;
        margin: 0;
    }
</style>