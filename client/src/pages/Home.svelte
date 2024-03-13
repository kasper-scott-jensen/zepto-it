<script>
    import SidePole from '../components/sidebar/SidePole.svelte'
    import TopPanel from '../components/header/TopPanel.svelte'
    import SideBar from '../components/sidebar/SideBar.svelte'
    import Slide from '../components/layouts/Slide.svelte'
    import CTA from '../components/buttons/CTA.svelte'
    import BottomPanel from '../components/footer/BottomPanel.svelte'
    import Trigger from '../components/buttons/Trigger.svelte'
    import Video from '../components/modals/Video.svelte'

    const slide1 = 'src/assets/bg/img-10.jpg'
    const slide2 = 'src/assets/bg/img-09.jpg'
    const slide3 = 'src/assets/bg/img-14.jpg'
    const slide4 = 'src/assets/bg/img-04.jpg'
    const slide5 = ''
    const slide6 = 'src/assets/bg/img-03.jpg'

    const vid1 = 'src/assets/vid/ricketyroll.mp4'

    function handleContactSubmit(event) {
        event.preventDefault()
        // handle email functionality
    }
</script>

<SidePole />
<TopPanel />
<SideBar />

<Slide bg={slide1} slideDir={null} anchor={'home'}>
    <div class="fix-12-12">
        <div class="fix-3-12 ae-2 margin-bottom-6">
            <img src="src/assets/svg/icon_white.svg" alt="icon" width="80px" />
        </div>
        <p class="ae-3 thin margin-bottom-6">
            <span
                >We provide <b>reliable</b> IT solutions and <b>peace</b> of mind.
                <br />Help is <b>one</b> click away.</span
            >
        </p>
        <CTA
            slideDir={'fromCenter'}
            animation={'ae-4'}
            text={'Get Started'}
            target={'#contact'}
        />
    </div>
</Slide>

<Slide bg={slide2} slideDir={'fromLeft'} anchor={'services'}>
    <div class="fix-12-12">
        <div class="fix-7-12 left toRight">
            <p class="opacity-6 margin-bottom-2 ae-1">
                Services
            </p>
            <h1 class="ae-1">
                Dont worry - we got you covered
            </h1>
            <p class="ae-2">
                <span class="opacity-8"
                    >Never hesitate to call us. Our expertise covers a large area, and we are always ready to find the exact solution suited for you.</span
                >
            </p>
            <ul class="flex">
                <li class="col-6-12 ae-3">
                    <h3 class="margin-top-3"><i class="fa-solid fa-circle-question padding-right-1"></i>IT Support</h3>
                    <p class="tiny opacity-6">
                        General support with any issues you might have. Have you tried turning it off and on again?
                    </p>
                </li>
                <li class="col-6-12 ae-4">
                    <h3 class="margin-top-3"><i class="fa-solid fa-users padding-right-1"></i>Consulting</h3>
                    <p class="tiny opacity-6">
                        Looking to digitalize your company? We can help you get a great start.
                    </p>
                </li>
                <li class="col-6-12 ae-5">
                    <h3 class="margin-top-3"><i class="fa-solid fa-code padding-right-1"></i>Software Development</h3>
                    <p class="tiny opacity-6">
                        In need of custom code? We house talented programmers, ready to go.
                    </p>
                </li>
                <li class="col-6-12 ae-6">
                    <h3 class="margin-top-3"><i class="fa-solid fa-globe padding-right-1"></i>Website</h3>
                    <p class="tiny opacity-6">
                        We do website development, optimization and templating. And everything in between.
                    </p>
                </li>
            </ul>
        </div>
    </div>
</Slide>

<Slide bg={slide4} slideDir={'fromRight'} anchor={'portfolio'}>
    <div class="fix-12-12">
        <ul class="flex left">
            <li class="col-6-12 fromBottomLeft">
                <p class="opacity-6 margin-bottom-2 ae-1">
                    Portfolio
                </p>
                <h1 class="ae-2">Our amazing customers</h1>
                <div class="ae-3">
                    <p class="opacity-8 margin-bottom-6">
                        We have had the pleasure of working with many valued customers.
                        Each one has added a unique perspective and set of challenges, driving us to innovate and improve our services.
                    </p>
                </div>
                <ul class="flex">
                    <li class="col-6-12 ae-3 margin-bottom-6">
                        <a href="https://www.aim-robotics.com" target="_blank"><img src="src/assets/img/aim-robotics-logo.png" alt="icon" width="200px" /></a>
                    </li>
                    <li class="col-6-12 ae-4 margin-bottom-6">
                        <a href="https://www.ungkrisecenter.dk" target="_blank"><img src="src/assets/img/ung-krisecenter-logo.png" alt="icon" width="200px" /></a>
                    </li>
                </ul>
            </li>
            <li class="col-1-12">&nbsp;</li>
            <li class="col-5-12 bottom">
                <!-- svelte-ignore a11y-img-redundant-alt -->
                <img
                    src="src/assets/img/partnership.jpg"
                    data-action="zoom"
                    class="shadow rounded ae-5 margin-bottom-6 margin-top-6"
                    alt="image"
                />
            </li>
        </ul>
    </div>
</Slide>

<Slide bg={slide3} slideDir={null} anchor={'about'}>
    <div class="fix-12-12">
        <div class="fix-6-12 left toLeft">
            <p class="opacity-6 margin-bottom-2 ae-1">
                About
            </p>
            <h1 class="ae-1">
                Nerds with a capital N
            </h1>
            <p class="ae-2 margin-bottom-6">
                <span class="opacity-8"
                    >
                    Code monkeys, problem solvers and coffee addicts.
                    A small company with large ambitions based in Copenhagen.
                    We're not just here to meet expectations; we're here to exceed them.
                    </span
                >
            </p>
            <Trigger 
                slideDir={null}
                animation={'ae-3'}
                text={'Read More'}
                target={null}
                id={9}
            />
        </div>
    </div>
</Slide>

<!-- <Video id={9} source={vid1} /> -->

<Slide bg={slide6} slideDir={null} anchor={'contact'}>
    <div class="fix-6-12">
        <p class="opacity-6 margin-bottom-2 ae-1">
            Contact
        </p>
        <img src="src/assets/svg/combo_white.svg" alt="icon" width="200px" class="ae-2 margin-bottom-4" />
        <ul class="flex margin-bottom-4">
            <li class="col-4-12 ae-3">
                <h3><i class="fa-solid fa-phone padding-right-1"></i></h3><p class="tiny">+45 91 74 36 42</p>
            </li>
            <li class="col-4-12 ae-4">
                <h3><i class="fa-solid fa-envelope padding-right-1"></i></h3><p class="tiny">contact@zeptoit.dk</p>
            </li>
            <li class="col-4-12 ae-5">
                <h3><i class="fa-solid fa-building padding-right-1"></i></h3><p class="tiny">Copenhagen</p>
            </li>
        </ul>
        <p class="hero ae-6 margin-bottom-3">
            <span class="opacity-8"
                >Let's have a conversation.</span
            >
        </p>
        <form
            autocomplete="off"
            class="slides-form"
            id="contact-form"
            on:submit={handleContactSubmit}
        >
            <input
                type="text"
                class="ae-7 margin-right-3 margin-bottom-3"
                name="name"
                placeholder="E-mail address"
                required
            />
            <CTA
                slideDir={null}
                animation={'ae-8'}
                text={'Send'}
                target={null}
            />
        </form>
    </div>
</Slide>

<BottomPanel />
