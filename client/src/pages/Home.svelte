<script>
    import SidePole from '../components/sidebar/SidePole.svelte'
    import TopPanel from '../components/header/TopPanel.svelte'
    import SideBar from '../components/sidebar/SideBar.svelte'
    import Slide from '../components/layouts/Slide.svelte'
    import BottomPanel from '../components/footer/BottomPanel.svelte'
    import CTA from '../components/buttons/CTA.svelte'

    const slide1 = 'src/assets/bg/img-10.jpg'
    const slide2 = 'src/assets/bg/img-15.jpg'
    const slide3 = 'src/assets/bg/img-14.jpg'
    const slide4 = 'src/assets/bg/img-89.jpg'
    const slide5 = ''
    const slide6 = 'src/assets/bg/img-95.jpg'
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
                    <h3 class="margin-top-3">IT Support</h3>
                    <p class="tiny opacity-6">
                        General support with any issues you might have. Have you tried turning it off and on again?
                    </p>
                </li>
                <li class="col-6-12 ae-4">
                    <h3 class="margin-top-3">Consulting</h3>
                    <p class="tiny opacity-6">
                        Looking to digitalize your company? We can help you get a great start.
                    </p>
                </li>
                <li class="col-6-12 ae-5">
                    <h3 class="margin-top-3">Software Development</h3>
                    <p class="tiny opacity-6">
                        In need of custom code? We house talented programmers, ready to go.
                    </p>
                </li>
                <li class="col-6-12 ae-6">
                    <h3 class="margin-top-3">Website</h3>
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
                <h1 class="ae-2">The Secret of Success</h1>
                <div class="ae-3">
                    <p class="opacity-8">
                        No matter how many times your amazing,
                        absolutely brilliant work is rejected by the
                        client, for whatever dopey, arbitrary
                        reason, there is often another amazing,
                        absolutely brilliant solution possible.
                    </p>
                </div>
                <ul class="flex">
                    <li class="col-6-12 ae-3">
                        <h3 class="margin-top-3">Camera</h3>
                    </li>
                    <li class="col-6-12 ae-4">
                        <h3 class="margin-top-3">Messages</h3>
                    </li>
                    <li class="col-6-12 ae-5">
                        <h3 class="margin-top-3">Music Center</h3>
                    </li>
                    <li class="col-6-12 ae-6">
                        <h3 class="margin-top-3">Channels</h3>
                    </li>
                </ul>
            </li>
            <li class="col-1-12">&nbsp;</li>
            <li class="col-5-12 bottom">
                <img
                    src="src/assets/img/image-89-2.jpg"
                    data-action="zoom"
                    class="shadow rounded ae-8 margin-bottom-6"
                    alt="Image"
                />
                <img
                    src="src/assets/img/image-89-2.jpg"
                    data-action="zoom"
                    class="shadow rounded ae-8"
                    alt="Image"
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
                Designers are meant to be loved, not to be
                understood.
            </h1>
            <p class="ae-2 margin-bottom-6">
                <span class="opacity-8"
                    >You must forget all your theories, all your
                    ideas before the subject. What part of these is
                    really your own will be expressed in
                    your&nbsp;expression.</span
                >
            </p>
            <CTA
            slideDir={null}
            animation={'ae-3'}
            text={'Read More'}
            target={''}
        />
        </div>
    </div>
</Slide>

<Slide bg={slide6} slideDir={null} anchor={'contact'}>
    <div class="fix-6-12">
        <p class="opacity-6 margin-bottom-2 ae-1">
            Contact
        </p>
        <h1 class="huge ae-1 margin-bottom-2">
            Download Mobile App
        </h1>
        <p class="hero ae-2 margin-bottom-3">
            <span class="opacity-8"
                >Learning never exhausts the mind.</span
            >
        </p>

        <form
            action="#"
            autocomplete="off"
            class="slides-form margin-bottom-3"
        >
            <input
                type="email"
                class="ae-3"
                name="email"
                placeholder="E-mail address"
            />
            <button
                type="submit"
                class="button blue gradient ae-4"
                name="submit">Try it free</button
            >
        </form>

        <a href="#" class="button hollow ae-5"
            ><img
                src="src/assets/img/appstore.jpg"
                height="63"
            /></a
        ><a href="#" class="button hollow ae-6"
            ><img
                src="src/assets/img/googleplay.jpg"
                height="63"
            /></a
        >
    </div>
</Slide>

<BottomPanel />
