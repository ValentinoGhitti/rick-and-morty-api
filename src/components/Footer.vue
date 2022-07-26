<template>
<div class="footer text-center text-white mt-5" id="footer">
    <div class="bubbles container">
        <div class="bubble" style="--size:3.3909991037595413rem; --distance:8.564411425917513rem; --position:-3.3532309343188405%; --time:3.337641675397866s; --delay:-3.8598811310658885s;"></div>
        <div class="bubble" style="--size:5.6696180078573795rem; --distance:8.237386989233332rem; --position:53.83419782426631%; --time:3.9822421087458917s; --delay:-3.89753449421937s;"></div>
        <div class="bubble" style="--size:4.583421366775942rem; --distance:9.38128061429176rem; --position:54.60126619661698%; --time:2.517052007029066s; --delay:-3.78693802909404s;"></div>
        <div class="bubble" style="--size:5.257650665640758rem; --distance:7.436513802589119rem; --position:58.07638903927696%; --time:3.5787606993702172s; --delay:-3.727907387715606s;"></div>
        <div class="bubble" style="--size:5.229508255244221rem; --distance:9.9519353103117rem; --position:74.21436924845615%; --time:3.028254580955734s; --delay:-3.2558799292110705s;"></div>
        <div class="bubble" style="--size:5.675200319744859rem; --distance:6.150496605028215rem; --position:16.40803187630667%; --time:2.095930094316172s; --delay:-2.012984983796527s;"></div>
        <div class="bubble" style="--size:4.3761417212986435rem; --distance:6.8733372826509695rem; --position:67.33293542719909%; --time:3.488941974619582s; --delay:-2.334601722943579s;"></div>
        <div class="bubble" style="--size:2.950301563617759rem; --distance:8.773235974561047rem; --position:72.33514453946891%; --time:2.52996034300591s; --delay:-3.093155150723837s;"></div>
        <div class="bubble" style="--size:3.7962980861050566rem; --distance:9.376934017605382rem; --position:0.9284191465863394%; --time:3.2726752420410317s; --delay:-3.2746503820920023s;"></div>
        <div class="bubble" style="--size:3.721084395955664rem; --distance:9.160889629565318rem; --position:17.773927915690802%; --time:3.288341342360385s; --delay:-2.714601022186284s;"></div>
        <div class="bubble" style="--size:2.235707949222566rem; --distance:7.440804351858876rem; --position:43.28529568082537%; --time:2.1995706778064124s; --delay:-3.680528188133694s;"></div>
        <div class="bubble" style="--size:5.158862079420235rem; --distance:9.533854451886327rem; --position:71.026240990692%; --time:2.8692037773746577s; --delay:-3.5557770672814346s;"></div>
        <div class="bubble" style="--size:2.839296642714123rem; --distance:6.182489448536465rem; --position:14.53940914818159%; --time:2.938568419305686s; --delay:-3.81476405451273s;"></div>
        <div class="bubble" style="--size:5.831089849696752rem; --distance:6.720856255476927rem; --position:-0.2918262612150073%; --time:3.6110339045076714s; --delay:-3.6108734761894308s;"></div>
        <div class="bubble" style="--size:3.7691993127248082rem; --distance:8.913331548077153rem; --position:64.18486372751045%; --time:2.19108565704424s; --delay:-2.3850044581272285s;"></div>
        <div class="bubble" style="--size:5.068613811981525rem; --distance:7.16414069186144rem; --position:2.613045732629777%; --time:3.8833174303115174s; --delay:-2.574991188736209s;"></div>
        <div class="bubble" style="--size:3.2798633470639915rem; --distance:7.299445260082528rem; --position:48.02708581947619%; --time:3.7242961387855673s; --delay:-2.4734505003243488s;"></div>
        <div class="bubble" style="--size:5.521576158610709rem; --distance:8.795523625782202rem; --position:23.798667098738793%; --time:2.0159378222175746s; --delay:-2.981385535625563s;"></div>
        <div class="bubble" style="--size:4.590771748441718rem; --distance:8.671193839332254rem; --position:59.88587536871286%; --time:3.3701772130578806s; --delay:-3.022271750369279s;"></div>
        <div class="bubble" style="--size:2.5809954125751933rem; --distance:9.753267128984376rem; --position:50.85335330973102%; --time:2.3057178413458725s; --delay:-3.020899022389121s;"></div>
        <div class="bubble" style="--size:4.0815595676298715rem; --distance:7.588289558521317rem; --position:85.59643940178883%; --time:3.060048727833308s; --delay:-2.756730474390774s;"></div>
    </div>
    <div class="content">
        <div class="col-auto" id="contact">
            <p class="pt-2 text-dark">
                <strong>Be sure to follow me on social media</strong><br>
                <strong> and visit my website to see more projects</strong>
            </p>
        </div>
        <div>
            <section class="mb-4">
                <a class="btn btn-outline-dark btn-floating m-1" href="https://www.linkedin.com/in/valentino-ghitti-b6042120a/" role="button"
                    ><i class="fa-brands fa-linkedin"></i></a>
                <a class="btn btn-outline-dark btn-floating m-1" href="https://github.com/ValentinoGhitti" role="button"
                    ><i class="fa-brands fa-github-square"></i>
                </a>
            </section>
            <section class="mb-2">
                <img class="logo" src="../../public/img/logo.png" alt="">
            </section>
        </div>
        <div class="text-center p-3 text-dark">
            <strong>© 2022 Copyright: Valentino Ghitti</strong>
        </div>
    </div>
</div>
<svg style="position:fixed; top:100vh;">
    <defs>
        <filter id="blob">
            <feGaussianBlur in="SourceGraphic" stdDeviation="10" result="blur"></feGaussianBlur>
            <feColorMatrix in="blur" mode="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 19 -9" result="blob"></feColorMatrix>
            <feComposite in="SourceGraphic" in2="blob" operator="atop"></feComposite>
        </filter>
    </defs>
</svg>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style scoped>
body {
    display: grid;
    grid-template-rows: 1fr auto;
    grid-template-areas: "main" "footer";
    overflow-x: hidden;
    min-height: 100vh;
    font-family: 'Open Sans', sans-serif;
}

.logo {
    height: 80px;
}
body .footer {
    z-index: 1;
    --footer-background:#57ba30;
    display: grid;
    position: relative;
    grid-area: footer;
    min-height: 12rem;
}   
body .footer .bubbles {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 1rem;
    background: var(--footer-background);
    -webkit-filter: url("#blob");
    filter: url("#blob");
}
body .footer .bubbles .bubble {
    position: absolute;
    left:var(--position, 2);
    background: linear-gradient(to right, #dce35b, #45b649);
    border-radius:100%;
    animation:bubble-size var(--time, 2s) ease-in infinite var(--delay, 0s),
    bubble-move var(--time, 2s) ease-in infinite var(--delay, 0s);
    transform:translate(-50%, 100%);
}
body .footer .content {
    z-index: 2;
    background: linear-gradient(to right, #dce35b, #45b649);
}

@keyframes bubble-size {
    0%, 75% {
        width:var(--size, 4rem);
        height:var(--size, 4rem);
    }
    100% {
        width:0rem;
        height:0rem;
    }
}
@keyframes bubble-move {
    0% {
        bottom:-4rem;
    }
    100% {
        bottom:var(--distance, 10rem);
    }
}
</style>