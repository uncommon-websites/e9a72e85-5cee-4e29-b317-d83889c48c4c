<script lang="ts">
	import { onMount } from 'svelte';

	let scrollY = 0;
</script>

<svelte:window bind:scrollY />

<div class="font-sans text-gray-900 antialiased selection:bg-primary-200 selection:text-primary-900">
	<!-- Hero Section -->
	<section class="relative min-h-screen w-full bg-gradient-to-b from-gray-900 via-gray-800 to-gray-50 text-white px-6 md:px-12 lg:px-24 pt-32 pb-24 flex flex-col justify-between">
		<div class="max-w-5xl">
			<h1 class="font-serif text-5xl md:text-7xl lg:text-8xl leading-[1.1] md:leading-[1.1] tracking-tight">
				Premium websites for South African businesses at prices you can afford.
			</h1>
			<p class="mt-8 text-xl md:text-2xl text-gray-300 max-w-3xl">
				From Cape Town to the world, we transform your business vision into stunning websites through collaborative design and custom development.
			</p>
		</div>

		<div class="mt-24 flex flex-col sm:flex-row gap-4">
			<a href="https://wa.me/27832540891" target="_blank" class="inline-flex items-center justify-center px-8 py-4 bg-primary-500 text-white rounded-full text-sm font-medium hover:bg-primary-600 transition-colors duration-300">
				WhatsApp Us
			</a>
			<a href="#work" class="inline-flex items-center justify-center px-8 py-4 border border-white/30 rounded-full text-sm font-medium hover:bg-white hover:text-gray-900 transition-colors duration-300 backdrop-blur-sm">
				View Our Work
			</a>
		</div>
	</section>

	<!-- Trusted Clients -->
	<section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-16 md:py-24">
		<p class="text-lg md:text-xl text-gray-600 mb-12">Trusted by South African businesses and international clients</p>
		
		<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-4 md:gap-8">
			{#each ["Jane's Edibles", "CA-PETAL Studio", "Veteranson", "Tech Hub", "Sainsbury Exotics", "The Clutter Fairy"] as client}
				<div class="h-20 bg-white rounded-lg flex items-center justify-center shadow-sm hover:shadow-md transition-all duration-300 px-4">
					<span class="font-semibold text-gray-800 text-center text-sm">{client}</span>
				</div>
			{/each}
		</div>
	</section>

    <!-- Work Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24" id="work">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 md:mb-24">
            <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900">Our portfolio, from Cape Town to the world</h2>
        </div>

        <div class="space-y-24 md:space-y-32">
            <!-- Project 1: Jane's Edibles -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Jane's Edibles</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Custom e-commerce solution built entirely from scratch with membership passcodes, age verification, order management, and shipment tracking. A complete platform for a business that couldn't use traditional e-commerce solutions.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Custom E-commerce</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Web Development</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-a-beautiful-artisan-bakery-display-with--1765525447576-0.webp" alt="Jane's Edibles" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 2: CA-PETAL Studio -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">CA-PETAL Studio</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        A stunning creative portfolio website that showcases the studio's work with commitment to quality and understanding of their vision.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Portfolio Website</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Brand Design</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-creative-studio-workspace-with-design-ma-1765525612746-0.webp" alt="CA-PETAL Studio" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 3: Veteranson -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Veteranson</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Professional corporate website for an Illinois-based security services company, demonstrating our international reach and ability to deliver premium websites for global clients.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Corporate Website</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">International Client</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-200 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-modern-office-building-with-glass-window-1765525777716-0.webp" alt="Veteranson" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 4: Tech Hub -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Tech Hub</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Modern e-commerce platform for South African tech products, featuring seamless shopping experience, product management, and secure payment integration.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">E-commerce</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Web Development</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-900 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out border border-gray-700">
                        <div class="absolute inset-0 flex items-center justify-center">
                            <div class="text-white text-4xl font-bold">Tech Hub</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Process Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-16 max-w-3xl">Our seamless process, from concept to completion</h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Consult -->
            <div class="bg-gray-50 p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[350px]">
                <div class="w-12 h-12 bg-primary-500 rounded-lg flex items-center justify-center mb-6">
                    <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z"></path>
                    </svg>
                </div>
                <h3 class="text-xl font-semibold mb-4">Consult & Understand</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We start by understanding your business vision and needs. Through collaborative consultation, we capture your ideas and provide creative direction on UX, design, and brand building.
                </p>
            </div>

            <!-- Design -->
            <div class="bg-gray-50 p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[350px]">
                <div class="w-12 h-12 bg-primary-500 rounded-lg flex items-center justify-center mb-6">
                    <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 21a4 4 0 01-4-4V5a2 2 0 012-2h4a2 2 0 012 2v12a4 4 0 01-4 4zm0 0h12a2 2 0 002-2v-4a2 2 0 00-2-2h-2.343M11 7.343l1.657-1.657a2 2 0 012.828 0l2.829 2.829a2 2 0 010 2.828l-8.486 8.485M7 17h.01"></path>
                    </svg>
                </div>
                <h3 class="text-xl font-semibold mb-4">Design & Create</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    With your vision in mind, we craft beautiful, mobile-responsive designs that reflect your brand. We remain flexible throughout, incorporating your feedback with free revisions during development.
                </p>
            </div>

            <!-- Develop -->
            <div class="bg-gray-50 p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[350px]">
                <div class="w-12 h-12 bg-primary-500 rounded-lg flex items-center justify-center mb-6">
                    <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"></path>
                    </svg>
                </div>
                <h3 class="text-xl font-semibold mb-4">Develop & Launch</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We build your website with custom development, including hosting, analytics, and all technical setup. Fast delivery with priority support ensures your business gets online quickly and smoothly.
                </p>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-16 text-center">What our clients say</h2>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-7xl mx-auto">
            <!-- Testimonial 1 -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
                <div class="mb-6">
                    <svg class="w-8 h-8 text-primary-500" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M14.017 21v-7.391c0-5.704 3.731-9.57 8.983-10.609l.995 2.151c-2.432.917-3.995 3.638-3.995 5.849h4v10h-9.983zm-14.017 0v-7.391c0-5.704 3.748-9.57 9-10.609l.996 2.151c-2.433.917-3.996 3.638-3.996 5.849h3.983v10h-9.983z"/>
                    </svg>
                </div>
                <p class="text-gray-700 mb-6 leading-relaxed">
                    "Jared's dedication and creativity truly went above and beyond. No one could have pulled this off as perfectly."
                </p>
                <div class="border-t border-gray-100 pt-4">
                    <p class="font-semibold text-gray-900">Jane's Edibles</p>
                    <p class="text-sm text-gray-500">E-commerce Platform</p>
                </div>
            </div>

            <!-- Testimonial 2 -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
                <div class="mb-6">
                    <svg class="w-8 h-8 text-primary-500" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M14.017 21v-7.391c0-5.704 3.731-9.57 8.983-10.609l.995 2.151c-2.432.917-3.995 3.638-3.995 5.849h4v10h-9.983zm-14.017 0v-7.391c0-5.704 3.748-9.57 9-10.609l.996 2.151c-2.433.917-3.996 3.638-3.996 5.849h3.983v10h-9.983z"/>
                    </svg>
                </div>
                <p class="text-gray-700 mb-6 leading-relaxed">
                    "Working with Jared was seamless. His commitment to quality and understanding what we needed made all the difference."
                </p>
                <div class="border-t border-gray-100 pt-4">
                    <p class="font-semibold text-gray-900">Daiyaan Patel</p>
                    <p class="text-sm text-gray-500">CEO, CA-PETAL Studio</p>
                </div>
            </div>

            <!-- Testimonial 3 -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
                <div class="mb-6">
                    <svg class="w-8 h-8 text-primary-500" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M14.017 21v-7.391c0-5.704 3.731-9.57 8.983-10.609l.995 2.151c-2.432.917-3.995 3.638-3.995 5.849h4v10h-9.983zm-14.017 0v-7.391c0-5.704 3.748-9.57 9-10.609l.996 2.151c-2.433.917-3.996 3.638-3.996 5.849h3.983v10h-9.983z"/>
                    </svg>
                </div>
                <p class="text-gray-700 mb-6 leading-relaxed">
                    "The attention to detail was incredible. Jared brought our vision to life after briefing with just basic concepts."
                </p>
                <div class="border-t border-gray-100 pt-4">
                    <p class="font-semibold text-gray-900">The Clutter Fairy</p>
                    <p class="text-sm text-gray-500">Founder</p>
                </div>
            </div>

            <!-- Testimonial 4 -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
                <div class="mb-6">
                    <svg class="w-8 h-8 text-primary-500" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M14.017 21v-7.391c0-5.704 3.731-9.57 8.983-10.609l.995 2.151c-2.432.917-3.995 3.638-3.995 5.849h4v10h-9.983zm-14.017 0v-7.391c0-5.704 3.748-9.57 9-10.609l.996 2.151c-2.433.917-3.996 3.638-3.996 5.849h3.983v10h-9.983z"/>
                    </svg>
                </div>
                <p class="text-gray-700 mb-6 leading-relaxed">
                    "Fast delivery, creative input, and fair pricing for the quality delivered. The process was smooth from start to finish."
                </p>
                <div class="border-t border-gray-100 pt-4">
                    <p class="font-semibold text-gray-900">Ziyaad Hanware</p>
                    <p class="text-sm text-gray-500">Finance Manager, Sainsbury Exotics</p>
                </div>
            </div>

            <!-- Testimonial 5 -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
                <div class="mb-6">
                    <svg class="w-8 h-8 text-primary-500" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M14.017 21v-7.391c0-5.704 3.731-9.57 8.983-10.609l.995 2.151c-2.432.917-3.995 3.638-3.995 5.849h4v10h-9.983zm-14.017 0v-7.391c0-5.704 3.748-9.57 9-10.609l.996 2.151c-2.433.917-3.996 3.638-3.996 5.849h3.983v10h-9.983z"/>
                    </svg>
                </div>
                <p class="text-gray-700 mb-6 leading-relaxed">
                    "Jared's expertise in UX and design, combined with his passion for our business, made him the perfect partner."
                </p>
                <div class="border-t border-gray-100 pt-4">
                    <p class="font-semibold text-gray-900">Olivia Ngei</p>
                    <p class="text-sm text-gray-500">Founder, LiveWell by Olivia</p>
                </div>
            </div>

            <!-- Testimonial 6 -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
                <div class="mb-6">
                    <svg class="w-8 h-8 text-primary-500" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M14.017 21v-7.391c0-5.704 3.731-9.57 8.983-10.609l.995 2.151c-2.432.917-3.995 3.638-3.995 5.849h4v10h-9.983zm-14.017 0v-7.391c0-5.704 3.748-9.57 9-10.609l.996 2.151c-2.433.917-3.996 3.638-3.996 5.849h3.983v10h-9.983z"/>
                    </svg>
                </div>
                <p class="text-gray-700 mb-6 leading-relaxed">
                    "Going above and beyond with creative input. Jared remained flexible and considered all my ideas throughout the project."
                </p>
                <div class="border-t border-gray-100 pt-4">
                    <p class="font-semibold text-gray-900">Veteranson</p>
                    <p class="text-sm text-gray-500">Security Services, Illinois</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <div class="text-center mb-16">
            <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-4">Transparent, affordable pricing</h2>
            <p class="text-xl text-gray-600 max-w-2xl mx-auto">No hidden fees. One-off payment. Premium quality.</p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-4xl mx-auto">
            <!-- Starter Package -->
            <div class="bg-gray-50 p-8 md:p-10 rounded-2xl shadow-sm hover:shadow-lg transition-all duration-300 border-2 border-gray-200">
                <h3 class="text-2xl font-bold text-gray-900 mb-2">Starter</h3>
                <div class="mb-6">
                    <span class="text-5xl font-bold text-gray-900">R5,000</span>
                    <span class="text-gray-600 ml-2">once-off</span>
                </div>
                <ul class="space-y-4 mb-8">
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-primary-500 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-gray-700">1 page website</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-primary-500 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-gray-700">Mobile responsive design</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-primary-500 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-gray-700">Contact form</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-primary-500 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-gray-700">Hosting included</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-primary-500 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-gray-700">Analytics integration</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-primary-500 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-gray-700">Free revisions during development</span>
                    </li>
                </ul>
                <a href="https://wa.me/27832540891?text=Hi%2C%20I'm%20interested%20in%20the%20Starter%20package" target="_blank" class="block w-full text-center bg-gray-900 text-white px-6 py-4 rounded-lg font-medium hover:bg-gray-800 transition-colors">
                    Get Started
                </a>
            </div>

            <!-- Professional Package -->
            <div class="bg-primary-500 p-8 md:p-10 rounded-2xl shadow-lg hover:shadow-xl transition-all duration-300 border-2 border-primary-600 relative">
                <div class="absolute -top-4 left-1/2 transform -translate-x-1/2 bg-gray-900 text-white px-4 py-1 rounded-full text-sm font-medium">
                    Most Popular
                </div>
                <h3 class="text-2xl font-bold text-white mb-2">Professional</h3>
                <div class="mb-6">
                    <span class="text-5xl font-bold text-white">R10,000</span>
                    <span class="text-primary-100 ml-2">once-off</span>
                </div>
                <ul class="space-y-4 mb-8">
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-white mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-white">Up to 5 pages</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-white mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-white">Mobile responsive design</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-white mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-white">Contact form</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-white mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-white">Hosting included</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-white mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-white">Analytics integration</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-white mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-white">Free revisions during development</span>
                    </li>
                    <li class="flex items-start">
                        <svg class="w-6 h-6 text-white mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-white">Priority support</span>
                    </li>
                </ul>
                <a href="https://wa.me/27832540891?text=Hi%2C%20I'm%20interested%20in%20the%20Professional%20package" target="_blank" class="block w-full text-center bg-white text-primary-600 px-6 py-4 rounded-lg font-medium hover:bg-gray-100 transition-colors">
                    Get Started
                </a>
            </div>
        </div>

        <p class="text-center text-gray-600 mt-12 max-w-2xl mx-auto">
            Need custom e-commerce or advanced features? <a href="https://wa.me/27832540891" target="_blank" class="text-primary-600 hover:text-primary-700 font-medium">Contact us</a> for a custom quote.
        </p>
    </section>

    <!-- About Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center max-w-6xl mx-auto">
            <div>
                <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-6">Meet Jared, your web designer</h2>
                <p class="text-lg text-gray-600 mb-6 leading-relaxed">
                    As the founder of Web500ZA, I've experienced firsthand how South African businesses struggle with expensive web solutions. My hands-on design expertise and deep understanding of local market needs position me to deliver quality websites at accessible prices.
                </p>
                <p class="text-lg text-gray-600 mb-8 leading-relaxed">
                    Based in Cape Town, I work with businesses across South Africa and internationally, transforming visions into premium websites through collaborative design and custom development.
                </p>
                <a href="https://wa.me/27832540891" target="_blank" class="inline-flex items-center justify-center px-8 py-4 bg-primary-500 text-white rounded-full text-sm font-medium hover:bg-primary-600 transition-colors duration-300">
                    Let's Work Together
                </a>
            </div>
            <div class="relative">
                <div class="aspect-[3/4] bg-gray-200 rounded-2xl overflow-hidden shadow-xl">
                    <img src="/generated/image-young-professional-at-desk-with-computer-1765525780208-2.webp" alt="Jared - Web Designer" class="w-full h-full object-cover" />
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Hero Section -->
    <section class="relative bg-gradient-to-b from-gray-900 via-gray-800 to-gray-900 pt-32 pb-32 px-6 md:px-12 lg:px-24 overflow-hidden">
        <div class="max-w-4xl mx-auto text-center relative z-10">
            <h2 class="font-serif text-4xl md:text-5xl lg:text-6xl text-white leading-tight mb-8">
                Ready to transform your business vision into a stunning website?
            </h2>
            <p class="text-xl text-gray-300 mb-12 max-w-2xl mx-auto">
                Join South African businesses who chose quality web design at affordable prices. Let's bring your vision to life.
            </p>
            
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <a href="https://wa.me/27832540891" target="_blank" class="inline-flex items-center justify-center px-8 py-4 bg-primary-500 text-white rounded-full text-lg font-medium hover:bg-primary-600 transition-colors duration-300">
                    <svg class="w-6 h-6 mr-2" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413Z"/>
                    </svg>
                    WhatsApp Us
                </a>
                <a href="mailto:agency@web500za.dev" class="inline-flex items-center justify-center px-8 py-4 border border-white/30 rounded-full text-lg font-medium text-white hover:bg-white hover:text-gray-900 transition-colors duration-300 backdrop-blur-sm">
                    Email Us
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 px-6 md:px-12 lg:px-24 pt-24 pb-12 relative overflow-hidden">

        <div class="relative z-10">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mb-24">
                <div class="col-span-1 md:col-span-1">
                    <h3 class="text-2xl font-bold text-white mb-4">Web500ZA</h3>
                    <p class="text-gray-400 mb-6">Premium websites for South African businesses at prices you can afford.</p>
                </div>
                
                <div class="space-y-4">
                    <h4 class="font-medium text-white">Contact</h4>
                    <div class="text-sm space-y-2">
                        <p><a href="mailto:agency@web500za.dev" class="hover:text-primary-400 transition-colors">agency@web500za.dev</a></p>
                        <p><a href="https://wa.me/27832540891" target="_blank" class="hover:text-primary-400 transition-colors">+27 83 254 0891</a></p>
                    </div>
                </div>

                <div class="space-y-4">
                    <h4 class="font-medium text-white">Location</h4>
                    <div class="text-sm space-y-1">
                        <p class="text-gray-400">Cape Town, South Africa</p>
                        <p class="text-gray-400 mt-4">Serving South African and<br>international clients</p>
                    </div>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between items-center border-t border-gray-800 pt-8">
                <div class="mb-4 md:mb-0">
                    <!-- Logo Icon -->
                    <svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-primary-500">
                        <path
                            fill-rule="evenodd"
                            clip-rule="evenodd"
                            d="M12 2.85795C11.7768 2.81204 11.5465 2.81204 11.3233 2.85795C11.0652 2.91103 10.8346 3.04023 10.6512 3.14294L10.6012 3.17086L4.38615 6.62366C4.36897 6.63319 4.35127 6.64294 4.33313 6.65293C4.13901 6.75988 3.89493 6.89432 3.70749 7.09769C3.54543 7.27357 3.4228 7.482 3.34778 7.70903C3.261 7.97166 3.26202 8.25029 3.26283 8.47194C3.2629 8.49264 3.26297 8.51284 3.26297 8.53253V15.3498C3.26297 15.3695 3.2629 15.3897 3.26283 15.4104C3.26202 15.632 3.261 15.9107 3.34778 16.1733C3.4228 16.4004 3.54543 16.6088 3.70749 16.7846C3.89493 16.988 4.13901 17.1224 4.33313 17.2294C4.35127 17.2394 4.36897 17.2491 4.38615 17.2587L10.6012 20.7115L10.6512 20.7394C10.8346 20.8421 11.0652 20.9713 11.3233 21.0244C11.5465 21.0703 11.7768 21.0703 12 21.0244C12.2581 20.9713 12.4888 20.8421 12.6721 20.7394L12.7221 20.7115L18.9371 17.2587C18.9448 17.2545 18.9525 17.2502 18.9603 17.2459C18.9701 17.2405 18.9801 17.235 18.9902 17.2294C19.1843 17.1224 19.4284 16.988 19.6158 16.7846C19.7779 16.6088 19.9005 16.4004 19.9756 16.1733C20.0623 15.9107 20.0613 15.632 20.0605 15.4104C20.0604 15.3897 20.0603 15.3695 20.0603 15.3498V8.53253C20.0603 8.51284 20.0604 8.49264 20.0605 8.47194C20.0613 8.25029 20.0623 7.97166 19.9756 7.70903C19.9005 7.482 19.7779 7.27357 19.6158 7.09769C19.4284 6.89432 19.1843 6.75988 18.9902 6.65293L18.9895 6.65256C18.9716 6.64272 18.9541 6.6331 18.9371 6.62366L12.7221 3.17086L12.6721 3.14294C12.4888 3.04023 12.2581 2.91103 12 2.85795ZM11.417 4.63921C11.5442 4.56851 11.6092 4.53278 11.6577 4.5094L11.6617 4.50748L11.6657 4.5094C11.7141 4.53278 11.7791 4.5685 11.9064 4.63921L17.491 7.7418L11.6616 10.9803L5.83225 7.7418L11.417 4.63921ZM4.94271 9.16917L10.8218 12.4353L10.8218 18.9125L5.20191 15.7903C5.06757 15.7157 4.99898 15.6772 4.95086 15.6465L4.94679 15.6439L4.94649 15.6391C4.94306 15.5822 4.94271 15.5035 4.94271 15.3498V9.16917Z"
                            fill="currentColor"
                        />
                    </svg>
                </div>
                
                <div class="flex gap-6 text-sm">
                    <a href="https://wa.me/27832540891" target="_blank" class="hover:text-primary-400 transition-colors">WhatsApp</a>
                    <a href="mailto:agency@web500za.dev" class="hover:text-primary-400 transition-colors">Email</a>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between items-center text-sm text-gray-500 mt-12 gap-4">
                <p>© 2025 Web500ZA. All rights reserved.</p>
                <p>Crafted with passion in Cape Town, South Africa</p>
            </div>
        </div>
    </footer>
</div>

<style>
    /* Custom utility for vertical writing mode */
    .writing-vertical-rl {
        writing-mode: vertical-rl;
    }
</style>

