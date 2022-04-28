<script lang="ts">
    import { push } from "svelte-spa-router";

    import LogoSvelte from "../assets/svelte.svg";
    import LogoAppwrite from "../assets/appwrite.svg";
    import LogoGithub from "../assets/github.svg";
    import LogoTwitter from "../assets/twitter.svg";
</script>

<!-- Hero -->
<section class="container h-screen mx-auto flex">
    <div class="flex flex-col mx-auto justify-center p-6 text-center">
        <p class="my-8 text-xl md:text-2xl lg:text-3xl font-medium">
            Introducing
        </p>
        <h1 class="text-4xl md:text-7xl lg:text-9xl font-bold">toTooooDoooo</h1>
        <p class="my-8 text-xl md:text-2xl lg:text-3xl font-medium">
            A Costumized personal To-do App built with
            <a href="http://github.com/appwrite/appwrite"><img
                class="w-8 h-8 inline transition duration-200 ease-in-out transform hover:-translate-y-3 hover:scale-125 hover:shadow-2xl"
                src={LogoAppwrite}
                alt="Appwrite Logo"
            /></a>
            Appwrite and
            <a href="https://svelte.dev/">
                <img class="w-8 h-8 inline transition duration-200 ease-in-out transform hover:-translate-y-3 hover:scale-125 hover:shadow-2xl" src={LogoSvelte} alt="Svelte Logo" />
            </a> Svelte
        </p>
        <button
            on:click={() => push("/login")}
            class="mx-auto mt-4 py-3 lg:py-5 px-10 lg:px-24 text-lg md:text-2xl font-semibold  rounded-lg shadow-md bg-white text-gray-900 border border-gray-900 hover:border-transparent hover:text-white hover:bg-gray-900 focus:outline-none"
        >
            Get Started
        </button>
    </div>
</section>

