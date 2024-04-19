<script setup>

</script>

<template>
    <footer class="footer">
        <div class="footer-wrap container">
            <div class="footer-logo">
                <div class="footer-logo-img"><img alt="a-consult logo" src="@/assets/img/logo.png" /></div>
                <div class="footer-logo-text">
                    Empowering Businesses with 
                    <br>
                    Expert IT Consulting Solutions
                </div>
            </div>
            <div class="footer-contact">
                <div class="footer-contact-title">Contact</div>
                <div class="footer-contact-item">Email: sales@a-consult.com</div>
                <div class="footer-contact-item">Phone: (381) 290-4567</div>
                <div class="footer-soc">
                    <div class="footer-soc-item">
                        <svg width="9" height="16" viewBox="0 0 9 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M2.69904 15.3466L2.67857 9.04968H0V6.35099H2.67857V4.55187C2.67857 2.12377 4.17099 0.953613 6.32088 0.953613C7.35069 0.953613 8.23577 1.03086 8.4937 1.06538V3.60289L7.00264 3.60357C5.83342 3.60357 5.60703 4.16334 5.60703 4.98477V6.35099H8.92857L8.03571 9.04968H5.60702V15.3466H2.69904Z" fill="#242F4B"/>
                        </svg>
                    </div>
                    <div class="footer-soc-item">
                        <svg width="18" height="19" viewBox="0 0 18 19" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <g clip-path="url(#clip0_24_3417)">
                                <path d="M12.75 2.45361H5.25C3.17893 2.45361 1.5 4.13255 1.5 6.20361V13.7036C1.5 15.7747 3.17893 17.4536 5.25 17.4536H12.75C14.8211 17.4536 16.5 15.7747 16.5 13.7036V6.20361C16.5 4.13255 14.8211 2.45361 12.75 2.45361Z" stroke="#2B3651" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                                <path d="M11.9998 9.48134C12.0923 10.1055 11.9857 10.743 11.6951 11.3031C11.4045 11.8632 10.9446 12.3174 10.381 12.6011C9.81736 12.8848 9.17862 12.9835 8.55562 12.8833C7.93262 12.783 7.3571 12.4889 6.91091 12.0427C6.46472 11.5965 6.17058 11.021 6.07033 10.398C5.97008 9.775 6.06883 9.13626 6.35253 8.57262C6.63622 8.00898 7.09042 7.54915 7.65052 7.25852C8.21062 6.9679 8.8481 6.86128 9.47228 6.95384C10.109 7.04825 10.6984 7.34494 11.1536 7.80007C11.6087 8.2552 11.9054 8.84465 11.9998 9.48134Z" stroke="#2B3651" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                                <ellipse cx="13.125" cy="5.82861" rx="1.125" ry="1.125" fill="#EBEDF0"/>
                            </g>
                            <defs>
                                <clipPath id="clip0_24_3417">
                                    <rect width="18" height="18" fill="white" transform="translate(0 0.953613)"/>
                                </clipPath>
                            </defs>
                        </svg>
                    </div>
                    <div class="footer-soc-item">
                        <svg width="15" height="13" viewBox="0 0 15 13" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M14.2857 2.30296C13.75 2.57283 13.2143 2.66278 12.5893 2.75274C13.2143 2.39291 13.6607 1.85318 13.8393 1.13353C13.3036 1.49335 12.6786 1.67326 11.9643 1.85318C11.4286 1.31344 10.625 0.953613 9.82143 0.953613C8.30357 0.953613 6.96429 2.30296 6.96429 3.92217C6.96429 4.19204 6.96429 4.37195 7.05357 4.55187C4.64286 4.46191 2.41071 3.29248 0.982143 1.49335C0.714286 1.94313 0.625 2.39291 0.625 3.02261C0.625 4.01213 1.16071 4.91169 1.96429 5.45143C1.51786 5.45143 1.07143 5.27152 0.625 5.0916C0.625 6.53091 1.60714 7.70034 2.94643 7.97021C2.67857 8.06016 2.41071 8.06016 2.14286 8.06016C1.96429 8.06016 1.78571 8.06016 1.60714 7.97021C1.96429 9.13964 3.03571 10.0392 4.375 10.0392C3.39286 10.8488 2.14286 11.2986 0.714286 11.2986C0.446429 11.2986 0.267857 11.2986 0 11.2986C1.33929 12.1082 2.85714 12.6479 4.46429 12.6479C9.82143 12.6479 12.7679 8.15012 12.7679 4.282C12.7679 4.19204 12.7679 4.01213 12.7679 3.92217C13.3929 3.47239 13.9286 2.93265 14.2857 2.30296Z" fill="#242F4B"/>
                        </svg>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-copyrights">
            <div class="container">© All rights reserved. A-CONSULT.</div>
        </div>
    </footer>
</template>


<style scoped>
.footer {
    padding-top: 62px;
    background-color: var(--gray-10);
}
.footer-wrap {
    display: flex;
    justify-content: space-between;
    width: 80%;
}
.footer-logo {
    width: 280px;
}
.footer-logo-img {
    margin: 20px 0;
}
.footer-logo-text {
    /* margin-top: 42px; */
    color: var(--blue-400);
    font-size: 14px;
    line-height: 1.7;
    font-weight: 400;
}
.footer-contact {

}
.footer-contact-title {
    color: var(--blue-700);
}
.footer-contact-item {
    margin-top: 22px;
    color: var(--blue-400);
    font-size: 14px;
    font-weight: 400;
}
.footer-soc {
    display: flex;
    justify-content: space-between;
    width: 170px;
    margin-top: 15px;
}
.footer-soc-item {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: var(--gray-30);
}
.footer-copyrights {
    margin-top: 45px;
    padding: 16px 0;
    background-color: var(--gray-30);
    color: var(--blue-300);
    font-size: 14px;
    text-align: center;
    border-top: 1px solid var(--gray-40);
}
</style>