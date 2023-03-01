<script>
    import Carousel from 'svelte-carousel';
    import { browser } from '$app/environment';
    import Industry from '../lib/components/Industry.svelte';
    import Footer from '../lib/components/Footer.svelte';
    import Technologies from '../lib/components/Technologies.svelte';
    let carousel;

    var industries=[
        {
            img:"/tensax/photo 1.png",
            title: "AI in Healthcare",
            content:"AI for Diagnosis | Personalised | Medicine | Drug Discovery | Patient Apps"
        },
        {
            img:"/tensax/photo 2.png",
            title: "Office AI",
            content:"Document Intelligence | Personal Assistants | AI Avatars | AI Works OS | Process AI Automation | AI Insights"
        },
        {
            img:"/tensax/photo 3.png",
            title: "Household AI",
            content:"AI Avatars | RLSE | Inventory Management | Domestic Helps | Smart Home | AI Companions"
        },
        {
            img:"/tensax/photo 4.png",
            title: "Fintech & Banking AI",
            content:"AI Investment Algorithum | Anomaly Detection | Document Intelligence | AI Due Diligence"
        },
        {
            img:"/tensax/photo 5.png",
            title: "Education AI",
            content:"AI Tutor | Personalized Education | AI Assessment Intelligence | AI Student Attention Intelligence"
        },
        {
            img:"/tensax/photo 6.png",
            title: "Human Emotion AI",
            content:"Attention | Facial Expression |Speech intelligence | Body language | Emotion AI"
        },
        {
            img:"/tensax/photo 7.png",
            title: "Fashion AI",
            content:"Clothing Try-On | Computer Vision | Body language-Ppse Tracking | 3D Superimposing | AI transfer | AI Recommendtions"
        },
        {
            img:"/tensax/photo 8.png",
            title: "Social Intalligence AI",
            content:"Conversational AI | AI Avatars | Natural Language | Swarm Intelligence | Feedback AI | Emotion AI | Attention AI"
        },
        {
            img:"/tensax/photo 9.png",
            title: "Smart Governance AI ",
            content:"Document intelligence | AI Assistants | AI Avatars | AI Works OS | AI Work Monitoring"
        },
        {
            img:"/tensax/photo 10.png",
            title: "Transpotation AI",
            content:"Self Driving AI | Traffic Grid AI | AI Avatars | Road Safety Camera Vision AI | In-Vehicle AI "
        },
        {
            img:"/tensax/photo 11.png",
            title: "Real Estate AI ",
            content:"Automated Valuation Models (AMVs) | Conversational AI | AI Agents | AI Chatbots"
        },
        {
            img:"/tensax/photo 12.png",
            title: "Factoy AI & RPA",
            content:"Machine intelligence | Reinforcement Learning | Computer Vision | Custom AI"
        },
        {
            img:"/tensax/photo 13.png",
            title: "Energy & Power AI",
            content:"Sun Harvasting | Computer Vision | Concentrated Solar Mirror Control AI | Power Grid AI"
        },
        {
            img:"/tensax/photo 14.png",
            title: "Agriculture AI ",
            content:"Computer Vision Segmentation | Customer Insights+BlockChain | AI Vision Applications"
        },
        {
            img:"/tensax/photo 15.png",
            title: "FoodTech AI",
            content:"Food recomandations |RPA | Customer Feedback | Emotinal AI | Supply Chain AI"
        },
        {
            img:"/tensax/photo 16.png",
            title: "Security & Defence AI ",
            content:"Real Life Search Engine(RLSE) | AI instant Camouflafe | Intruder Detection | AI Object Tracking"
        },
        {
            img:"/tensax/photo 17.png",
            title: "BlockChain",
            content:"Intellectual Property | Security Tokens | Data Integrity | Immutable Data Chain"
        },
        {
            img:"/tensax/photo 18.png",
            title: "Space AI",
            content:"AI Powered Ephemeris | Ai Exoplanet Descovery | AI Vision"
        },
        {
            img:"/tensax/photo 19.png",
            title: "AI for Good-Humanitarian",
            content:"AI in Remote Areas | Embendded AI | CSR REdistribution Management AI"
        },
    ]
 
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
        <img src="tensax/build_ai.jpg" class="w-96 h-80 mr-10" alt="">
    </div>
</div>


<div id="products" class="ml-20 mt-32">
    <p class="text-3xl font-bold text-gray-700 ">Our Products</p>
    {#if browser}
      <Carousel
        bind:this={carousel}
      >
        <div class="p-8 grid grid-cols-2">
            <div class="bg-slate-200 ">
                <img src="/tensax/aihub.jpg" alt="" />
            </div>
            <div>
                <p class="text-center text-3xl font-semibold text-gray-600">tensaX AI Hub</p>
                <ul class="mt-10 list-disc space-y-4">
                    <li>
                        Discover & Test Pilot Pre-Built AI Models, Explore from our range of ready-to-deploy AI Models and see the power of AI with our AI models
                    </li>
                    <li>
                        Establish your AI Data Lake for the development of your customized AI & prepare yourself or your team for the future development of customized AI On-premises or Cloud.
                    </li>
                    <li>
                        Our Team of AI Expefis from TensaX Innovation Lab pefiorm Feature Engineering and present Insights, presented to you in intelligence insights.
                    </li>
                    <li>
                        Manage your deployed AIs with TensaX AI Hub.
                    </li>
                    <li>
                        Our Team of AI Expefis from TensaX Innovation Lab build custom AI for your case and view live updates and results in AI control Rooms.
                    </li>
                </ul>
            </div>
        </div>
        <div>2</div>
        <div>3</div>
      </Carousel>
    {/if}
</div>

<div id="industries" class="mx-20 mb-10  bg-orange-100 p-4 rounded-2xl drop-shadow-2xl">
    <p class="text-3xl font-bold text-gray-700 mt-40 ">Explore Tensax AI Industries</p>
    <div class="grid grid-cols-4 gap-8 pt-10">
        {#each industries.slice(0, 7) as ind}
            <Industry img={ind.img} title={ind.title} content = {ind.content}/>

        {/each}
        <div class="flex justify-center items-center bg-gray-100 rounded-lg ">view more
        </div>
    </div>
</div>

<div id="technologies">
    <Technologies/>
</div>

<div id="footer">
    <Footer/>
    </div>