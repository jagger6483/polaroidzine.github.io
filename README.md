<!DOCTYPE html>
<html lang="en">
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Polaroid Zine (Dark Grid)</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Load Playfair Display (Titles) and Kalam (Handwritten/Body) -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&family=Kalam:wght@300;400;700&display=swap" rel="stylesheet">
    
<script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'soft-pink': '#FFC0CB', /* Brighter, classic pink for pop */
                        'accent-pink': '#F872A1', /* Rose pink for highlights */
                        'text-light': '#f0f0f0',
                        'bg-dark': '#111111',
                        'grid-line': '#333333',
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        title: ['"Playfair Display"', 'serif'],
                        handwritten: ['Kalam', 'cursive'],
                    },
                    boxShadow: {
                        'soft': '0 4px 10px rgba(255, 255, 255, 0.08)',
                        'clipping': '3px 3px 0px 0px #F872A1',
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #111111;
            color: #f0f0f0; /* Default light text */
            /* Black Grid Paper Effect */
            background-image: 
                linear-gradient(to right, #333333 1px, transparent 1px),
                linear-gradient(to bottom, #333333 1px, transparent 1px);
            background-size: 20px 20px;
        }
        /* Clipping elements are white paper on the dark background */
        .article-card {
            background-color: white; 
            color: #333333; /* Dark text on white card */
            transition: all 0.2s ease-in-out;
            border: 1px solid #ddd;
            border-radius: 8px;
        }
        .article-card:hover {
            transform: translateY(-2px); 
            box-shadow: 0 6px 15px rgba(255, 255, 255, 0.15); /* Light shadow on dark mode hover */
        }
        .clipping {
            border: 2px solid #F872A1;
            box-shadow: 3px 3px 0px 0px #F872A1;
        }
    .text.accent-pink {
}
    .font-title {
}
    .text.accent-pink {
}
    .text-accent-pink {
}
    </style>
</head>
<body class="text-text-light">

    <!-- Header & Navigation -->
    <header class="bg-bg-dark sticky top-0 z-50 border-b border-gray-800 shadow-lg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <!-- Logo/Title -->
            <div class="text-4xl font-title font-light italic tracking-tight">
                <a href="#" class="text-text-light hover:text-accent-pink transition duration-300">
                    Polaroid <span class="text-soft-pink font-semibold">Zine</span>
                </a>
            </div>

            <!-- Desktop Navigation -->
            <nav class="hidden md:flex space-x-8 text-lg font-title font-medium">
                <a href="#about-us-section" class="text-text-light hover:text-accent-pink transition duration-300">About</a>
                <a href="#features" class="text-text-light hover:text-accent-pink transition duration-300">Features</a>
                <a href="#photo-essays" class="text-text-light hover:text-accent-pink transition duration-300">Photo Essays</a>
                <a href="#about-us-section" class="text-text-light hover:text-accent-pink transition duration-300">Contact</a>
            </nav>

            <!-- Menu/Search Icon -->
            <button class="text-text-light hover:text-accent-pink p-2 rounded-full transition duration-300">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6"><line x1="4" y1="12" x2="20" y2="12"></line><line x1="4" y1="6" x2="20" y2="6"></line><line x1="4" y1="18" x2="20" y2="18"></line></svg>
            </button>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10 md:py-16">
        
        <!-- Hero Featured Article (Updated to 'Coming Soon' status) -->
        <section class="mb-16">
            <div class="block group bg-white article-card shadow-soft hover:shadow-xl">
                <div class="md:flex overflow-hidden rounded-lg">
                    
                    <!-- Text Content -->
                    <div class="md:w-1/2 p-6 sm:p-10 flex flex-col justify-center order-2 text-text-dark">
                        <p class="text-sm uppercase font-handwritten text-accent-pink mb-2 tracking-wider">Debut Issue</p>
                        <h2 class="text-5xl sm:text-6xl font-title font-light leading-tight mb-4">
                        Issue No. 1: ...&nbsp; <span class="text-accent-pink">&nbsp;</span> </h2>
                        <p class="text-gray-700 mb-6 text-xl font-title italic">
                            Our debut issue is currently being developed! Check back soon for our first featured photo essay.
                        </p>
                        <div class="text-sm font-title text-gray-500">
                            Coming Soon &middot; Fall 2025
                        </div>
                    </div>

                    <!-- Image -->
                    <div class="md:w-1/2 h-80 md:h-96 overflow-hidden order-1 border-r border-gray-200">
                        <img src="https://placehold.co/800x600/333/FFC0CB?text=ISSUE+1+COMING+SOON" 
                             alt="Placeholder image for the coming soon featured article" 
                             class="w-full h-full object-cover">
                    </div>
                </div>
            </div>
        </section>

        <!-- New About Us Section -->
        <section id="about-us-section" class="mb-16">
            <div class="bg-white p-6 sm:p-10 rounded-lg article-card clipping text-text-dark max-w-4xl mx-auto">
                <h3 class="text-4xl font-title font-medium italic mb-4 border-b-2 border-accent-pink pb-2">
                    About <span class="text-accent-pink">Polaroid Zine</span>
                </h3>
                <p class="text-lg font-title leading-relaxed text-gray-700">
                    Polaroid Zine is a creative space where pop culture, memory, media, and fashion intersect. Through both print and digital formats, we explore the small, vivid moments that shape how we see the world, from nostalgic snapshots to contemporary trends. Each issue features photography, illustration, essays, reflections, and fashion perspectives that celebrate individuality and creativity. We invite readers to pause, reflect, and engage with the cultural moments that linger—whether it’s the thrill of a new release, the charm of a vintage outfit, or the everyday details that make life unique. Polaroid Zine is a lens on life, framed in pixels, print, and perspective.
                </p>
            </div>
        </section>

        <!-- Main Grid & Sidebar -->
        <div class="grid grid-cols-1 lg:grid-cols-4 gap-8 md:gap-10">

            <!-- Article Grid (3 columns on large screens) -->
            <div class="lg:col-span-3">
                <h3 class="text-4xl font-title font-medium italic mb-8 pb-3 border-b-2 border-accent-pink">
                    Upcoming <span class="text-soft-pink">Features</span>
                </h3>
                
                <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-8">
                    <!-- Article 1: Pending -->
                    <a href="#" class="block group bg-white p-5 article-card shadow-soft">
                        <div class="h-48 overflow-hidden mb-4 border border-gray-200">
                            <img src="https://placehold.co/600x400/333/FFC0CB?text=PENDING+ARTICLE+1" alt="Placeholder image for pending content" class="w-full h-full object-cover">
                        </div>
                        <p class="text-sm uppercase font-handwritten text-accent-pink mb-1">Coming Soon</p>
                        <h4 class="text-xl font-title font-medium italic mb-2 text-accent-pink">The Comfort of     Film</h4>
                    <p class="text-base text-gray-700 font-handwritten line-clamp-3">
                            This article will be available when our first issue drops. Check back soon for our debut content!
                        </p>
                    </a>
                    
                    <!-- Article 2: Pending -->
                    <a href="#" class="block group bg-white p-5 clipping">
                        <div class="h-48 overflow-hidden mb-4 border border-gray-300">
                            <img src="https://placehold.co/600x400/333/F872A1?text=PENDING+ARTICLE+2" alt="Placeholder image for pending content" class="w-full h-full object-cover">
                        </div>
                        <p class="text-sm uppercase font-handwritten mb-1 text-accent-pink">Coming Soon</p>
                        <h4 class="text-xl font-title font-medium italic mb-2 text-accent-pink">&nbsp;Halloween Media</h4>
<p class="text-base text-gray-700 font-handwritten line-clamp-3">
                            This article will be available when our first issue drops. Check back soon for our debut content!
                        </p>
                    </a>

                    <!-- Article 3: Pending -->
                    <a href="#" class="block group bg-white p-5 article-card shadow-soft">
                        <div class="h-48 overflow-hidden mb-4 border border-gray-200">
                            <img src="https://placehold.co/600x400/333/F872A1?text=PENDING+ARTICLE+3" alt="Placeholder image for pending content" class="w-full h-full object-cover">
                        </div>
                        <p class="text-sm uppercase font-handwritten text-accent-pink mb-1">Coming Soon</p>
                        <h4 class="text-xl font-title font-medium italic mb-2 text-accent-pink">The Revival Horror   in Film</h4>
                        <p class="text-base text-gray-700 font-handwritten line-clamp-3">
                            This article will be available when our first issue drops. Check back soon for our debut content!
                        </p>
                    </a>

                    <!-- Article 4: Pending -->
                    <a href="#" class="block group bg-white p-5 article-card shadow-soft">
                        <div class="h-48 overflow-hidden mb-4 border border-gray-200">
                            <img src="https://placehold.co/600x400/333/FFC0CB?text=PENDING+ARTICLE+4" alt="Placeholder image for pending content" class="w-full h-full object-cover">
                        </div>
                        <p class="text-sm uppercase font-handwritten text-text-dark mb-1 text-accent-pink">Coming Soon</p>
                        <h4 class="text-xl font-title font-medium italic mb-2">Halloween Trends&nbsp;</h4>
                        <p class="text-base text-gray-700 font-handwritten line-clamp-3">
                            This article will be available when our first issue drops. Check back soon for our debut content!
                        </p>
                    </a>
                    
                    <!-- Article 5: Pending -->
                    <a href="#" class="block group bg-white p-5 article-card clipping">
                        <div class="h-48 overflow-hidden mb-4 border border-gray-300">
                            <img src="https://placehold.co/600x400/333/F872A1?text=PENDING+ARTICLE+5" alt="Placeholder image for pending content" class="w-full h-full object-cover">
                        </div>
                        <p class="text-sm uppercase font-handwritten text-accent-pink mb-1">Coming Soon</p>
                        <h4 class="text-xl font-title font-medium italic mb-2">&nbsp;Sustainable Costumes</h4>
                        <p class="text-base text-gray-700 font-handwritten line-clamp-3">
                            This article will be available when our first issue drops. Check back soon for our debut content!
                        </p>
                    </a>

                    <!-- Article 6: Pending -->
                    <a href="#" class="block group bg-white p-5 article-card shadow-soft">
                        <div class="h-48 overflow-hidden mb-4 border border-gray-200">
                            <img src="https://placehold.co/600x400/333/FFC0CB?text=PENDING+ARTICLE+6" alt="Placeholder image for pending content" class="w-full h-full object-cover">
                        </div>
                        <p class="text-sm uppercase font-handwritten text-text-dark mb-1 text-accent-pink">Coming Soon</p>
                        <h4 class="text-xl font-title font-medium italic mb-2">&nbsp;The Final Girl</h4>
                        <p class="text-base text-gray-700 font-handwritten line-clamp-3">
                            This article will be available when our first issue drops. Check back soon for our debut content!
                        </p>
                    </a>
                </div>
            </div>

            <!-- Sidebar (1 column on large screens) -->
            <aside class="lg:col-span-1 space-y-8">
                
                <!-- Submission Guide (White Card) -->
                <div class="bg-white p-6 rounded-lg article-card clipping text-text-dark">
                    <h4 class="text-2xl font-title font-medium italic mb-4 border-b border-accent-pink pb-2">Submissions <span class="text-accent-pink">Paused</span></h4>
                    <p class="text-sm font-title text-gray-600 mb-4">
                        We are currently focused on finalizing our debut issue. Submission guidelines will be posted here once the first issue launches!
                    </p>
                    <button class="w-full bg-accent-pink text-white font-title font-semibold py-3 rounded-lg hover:bg-soft-pink hover:text-bg-dark transition duration-300 shadow-clipping" style="box-shadow: 2px 2px 0px 0px #333333;">
                        Check Back Soon
                    </button>
                </div>

                <!-- Print Zine Placeholder (Soft Pink background to pop against black) -->
                <div class="bg-soft-pink p-6 rounded-lg article-card shadow-soft text-center text-text-dark">
                    <h4 class="text-xl font-title italic mb-2">Print Issue: Fading Light</h4>
                    <img src="https://placehold.co/300x200/fff/F872A1?text=ZINE+COMING+SOON" 
                         alt="Mockup of the zine cover" 
                         class="w-2/3 mx-auto my-4 border-2 border-accent-pink">
                    <p class="text-sm font-handwritten text-gray-700 mb-3">Pre-orders opening soon!</p>
                    <button class="bg-white border border-accent-pink text-accent-pink font-handwritten py-2 px-6 rounded-full opacity-50 cursor-not-allowed">
                        Order Physical Zine
                    </button>
                </div>
            </aside>
        </div>

    </main>

    <!-- Footer -->
    <footer class="bg-bg-dark border-t border-gray-800 mt-20 text-text-light">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10">
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 mb-8">
                <!-- Col 1: Polaroid Zine Links -->
                <div>
                    <h5 class="text-xl font-title italic mb-3 text-soft-pink">Polaroid Zine</h5>
                    <ul class="space-y-1 text-sm text-gray-400 font-title">
                        <li><a href="#about-us-section" class="hover:text-soft-pink transition">Our Story</a></li>
                        <li><a href="#" class="hover:text-soft-pink transition">Archives</a></li>
                    </ul>
                </div>
                <!-- Col 2: Content Links -->
                <div>
                    <h5 class="text-xl font-title italic mb-3 text-text-light">Content</h5>
                    <ul class="space-y-1 text-sm text-gray-400 font-title">
                        <li><a href="#" class="hover:text-soft-pink transition">Photo Essays (Pending)</a></li>
                        <li><a href="#" class="hover:text-soft-pink transition">Style Clips (Pending)</a></li>
                    </ul>
                </div>
                
                <!-- Col 3: Connect & Apply (NEW SOCIAL SECTION) -->
                <div>
                    <h5 class="text-xl font-title italic mb-3 text-text-light">Connect & Apply</h5>
                    <ul class="space-y-1 text-sm text-gray-400 font-title">
                        <li><a href="https://www.instagram.com/polaroidzine/" target="_blank" rel="noopener noreferrer" class="hover:text-soft-pink transition">Instagram (@polaroidzine)</a></li>
                        <li><a href="https://docs.google.com/forms/d/e/1FAIpQLScIqGjqLJ7JiGgShbmwnt30qJIoXHml3fvHh6rC9rA9CB3Zkw/viewform?usp=dialog" target="_blank" rel="noopener noreferrer" class="hover:text-soft-pink transition">Contributor Application</a></li>
                    </ul>
                </div>

                <!-- Col 4: Newsletter Signup (Now only 1 column on large screens) -->
                <div class="md:col-span-1">
                    <h5 class="text-xl font-title italic mb-3">Soft <span class="text-soft-pink">Notes</span></h5>
                    <p class="text-sm text-gray-400 font-title mb-3">Sign up for our quiet weekly update.</p>
                    <div class="flex space-x-2">
                        <input type="email" placeholder="Email address" class="p-3 w-full rounded-lg bg-gray-800 border border-accent-pink text-white font-title focus:outline-none focus:border-soft-pink" required>
                        <button class="bg-accent-pink text-white px-5 rounded-lg font-title font-semibold hover:bg-soft-pink hover:text-bg-dark transition">
                            Go
                        </button>
                    </div>
                </div>
            </div>

            <!-- Copyright -->
            <div class="text-center text-sm font-title text-gray-600 pt-4 border-t border-gray-800">
                &copy; 2025 Polaroid Zine. Keep it soft.
            </div>

        </div>
    </footer>

</body>
</html>
