<template>
    <footer id="Contacto" class="footer">
        <div class="titulo">Contacto</div>
        <ul class="foot-links">
            <li>
                <a title="Los Tejos" href="https://github.com/Diego090200" target="_blank">
                    <img src="/img/redes/Github.png" alt="Link a Github" class="redes">
                </a>
            </li>
            <li>
                <a title="Los Tejos" href="https://www.instagram.com/pic_alej/" target="_blank">
                    <img src="/img/redes/Instagram.png" alt="Link a Instagram" class="redes">
                </a>
            </li>
            <li>
                <a title="Los Tejos" href="https://www.facebook.com/profile.php?id=100001564866961" target="_blank">
                    <img src="/img/redes/Facebook.png" alt="Link a Instagram" class="redes">
                </a>
            </li>
            <li>
                <a title="Los Tejos" href="https://www.linkedin.com/in/diego-hernandez-661418248/" target="_blank">
                    <img src="/img/redes/Linkedin.png" alt="Link a Instagram" class="redes">
                </a>
            </li>
            <li>
                <a title="Los Tejos" href="mailto:alehernandezhernandez09@gmail.com" target="_blank">
                    <img src="/img/redes/Google.png" alt="Link a Instagram" class="redes">
                </a>
            </li>
        </ul>
    </footer>
</template>
<style scoped>
    .footer{
        align-items: center;
        display: flex;
        flex-direction: column;
        gap: 50px;
        justify-content: center;
        padding: 40px 24px 30px;
    }

    .foot-links{
        align-items: center;
        display: flex;
        flex-direction: row;
        gap: 100px;
        justify-content: center;
        list-style: none;
        padding: 0px;
    }

    .redes{
        width: 48px;
        height: 48px;
    }

    .titulo{
        color: #FFFFFF;
        font-family: 'Nunito', sans-serif;
        font-size: 40px;
        font-style: normal;
        line-height: 23px;
        margin-top: 100px;
    }

    @media only screen and (max-width: 768px) {
    .foot-links {
        flex-direction: column;
        flex-wrap: wrap;
        gap: 20px;
    }
    .titulo {
        font-size: 30px;
        margin-top: 50px;
    }
}
</style>