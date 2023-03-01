<script>

    import Footer from '../lib/components/Footer.svelte';
    import AiIndustries from '../lib/components/AIIndustries.svelte';
    import OurPartners from '../lib/components/OurPartners.svelte';
</script>

<div>
    <img src="tensax/bg.png" class="absolute -z-10 w-[40rem]" alt="" />
    <nav class="flex p-8 z-10 justify-between px-20">
        <ul class="flex space-x-14 text-xl font-semibold mt-5 ml-5">
            <li class="hover:underline underline-offset-8 cursor-pointer"><a href="/#home"> Home </a></li>
            <li class="hover:underline underline-offset-8 cursor-pointer"><a href="/#products"> Products </a></li>
            <li class="hover:underline underline-offset-8 cursor-pointer"><a href="/#industries"> Industries </a></li>
            <li class="hover:underline underline-offset-8 cursor-pointer">Technologies</li>
            <li class="hover:underline underline-offset-8 cursor-pointer">Partner with us</li>
            <li class="hover:underline underline-offset-8 cursor-pointer"> <a href="/#footer"> About Us </a></li>
            <li class="hover:underline underline-offset-8 cursor-pointer"><a href="/#footer"> Contact Us </a></li>
        </ul> 
        <img src="tensax/logo.jpg" class="absolute right-28 w-52" alt="" />
    </nav> 
</div>

<div id="home" class="flex justify-between mt-20 ml-20">
    <div >
        <p class="text-5xl text-gray-700 w-[rem] leading-tight font-bold">Build AI & <br> Emerging Technologies</p>
        <p class="text-xl mt-8 font-semibold text-gray-500">Revolutionizing the AI & Emerging Technology development process</p>
        <div class="mt-20  space-x-10">
            <a href="/#products" class="bg-orange-500 hover:shadow hover:bg-orange-600 p-6 rounded-2xl text-xl text-white font-semibold">Explore our products</a>
            <button class="relative after:absolute after:bg-orange-500 after:bottom-0 after:left-0 after:h-[3px] after:w-full after:origin-bottom-right after:scale-x-0 hover:after:origin-bottom-left hover:after:scale-x-100 after:transition-transform after:ease-in-out after:duration-300">
                <p class=" p-4 rounded-2xl text-xl text-orange-600 font-bold">View our Industries</p> 
            </button>
        </div>
    </div>
    <div class="">
        <img src="tensax/build_ai.jpg" class="w-96 h-80 mr-10" alt="" />
    </div>
</div>


<div id="Industries" class="ml-20 mt-32">
    <AiIndustries/>
</div>

<OurPartners/>

<div id="footer">
    <Footer/>
</div>