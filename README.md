<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Artisan's Meadow</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Klee+One:wght@400;600&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #FDF6E3; /* Warm Beige */
        }
        .font-ghibli {
            font-family: 'Klee One', cursive;
        }
        .bg-gradient-ghibli {
            background-image: linear-gradient(to bottom right, #FDF6E3, #E0E7FF, #D1FAE5); /* Warm Beige -> Sky Blue -> Moss Green */
        }
        .shadow-gentle {
            box-shadow: 0 4px S12px 0 rgba(0, 0, 0, 0.05);
        }
        .shadow-gentle-hover:hover {
            box-shadow: 0 8px 20px 0 rgba(0, 0, 0, 0.08);
            transform: translateY(-4px);
        }
        .tab-active {
            background-color: #FBCFE8; /* Blush Pink */
            color: #881337;
        }
        .icon-hand-drawn {
            stroke-width: 1.5;
            stroke-linecap: round;
            stroke-linejoin: round;
        }
    </style>
</head>
<body class="bg-gradient-ghibli text-gray-700">

    <div class="container mx-auto px-4 sm:px-6 lg:px-8 py-10">

        <!-- Header -->
        <header class="flex flex-col sm:flex-row justify-between items-center mb-12">
            <h1 class="font-ghibli text-5xl font-semibold text-green-800 mb-6 sm:mb-0">Artisan's Meadow</h1>
            <div class="flex items-center space-x-5">
                <a href="#" class="text-lg text-gray-600 hover:text-green-700 transition duration-300">Log In</a>
                <a href="#" class="bg-pink-200 text-pink-800 hover:bg-pink-300 font-semibold px-6 py-3 rounded-full transition duration-300 text-lg">Sign Up</a>
                <button class="p-3 rounded-full hover:bg-yellow-100 transition duration-300">
                    <!-- Hand-drawn style cart icon -->
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-7 icon-hand-drawn text-gray-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z" />
                    </svg>
                </button>
            </div>
        </header>

        <!-- Search Bar -->
        <div class="relative w-full max-w-3xl mx-auto mb-16">
            <input type="text" placeholder="Search for dreamy illustrations, cozy pottery..." class="w-full py-4 pl-14 pr-5 text-lg bg-white/70 backdrop-blur-sm border-2 border-transparent focus:border-yellow-400 rounded-full shadow-gentle transition duration-300 outline-none text-gray-700 placeholder-gray-500">
            <!-- Hand-drawn style search icon -->
            <svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-7 icon-hand-drawn absolute left-5 top-1/2 -translate-y-1/2 text-gray-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
            </svg>
        </div>

        <!-- Category Filters -->
        <div class="flex justify-center flex-wrap gap-4 mb-16">
            <button class="px-6 py-3 rounded-full font-medium transition duration-300 bg-green-100 text-green-800 hover:bg-green-200">All</button>
            <button class="px-6 py-3 rounded-full font-medium transition duration-300 tab-active">Illustration</button>
            <button class="px-6 py-3 rounded-full font-medium transition duration-300 bg-blue-100 text-blue-800 hover:bg-blue-200">Pottery</button>
            <button class="px-6 py-3 rounded-full font-medium transition duration-300 bg-yellow-100 text-yellow-800 hover:bg-yellow-200">Crafts</button>
            <button class="px-6 py-3 rounded-full font-medium transition duration-300 bg-purple-100 text-purple-800 hover:bg-purple-200">Animation</button>
            <button class="px-6 py-3 rounded-full font-medium transition duration-300 bg-red-100 text-red-800 hover:bg-red-200">Textiles</button>
        </div>

        <!-- Grid-based Project Cards -->
        <main class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-10">
            <!-- Card 1 -->
            <div class="bg-white rounded-2xl overflow-hidden shadow-gentle shadow-gentle-hover transition-all duration-300">
                <img src="https://placehold.co/400x300/A7D7C5/5E8B7E?text=Forest+Spirits" alt="Artwork of forest spirits" class="w-full h-56 object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x300/cccccc/ffffff?text=Image+Not+Found';">
                <div class="p-6">
                    <h3 class="font-semibold text-xl mb-2 text-gray-800">Whispers of the Woods</h3>
                    <div class="flex items-center text-gray-500">
                        <img src="https://placehold.co/40x40/F7F5E6/BFB0A3?text=A" alt="Creator Avatar" class="w-8 h-8 rounded-full mr-3 border-2 border-white">
                        <span>Anna Evergreen</span>
                    </div>
                </div>
            </div>
            <!-- Card 2 -->
            <div class="bg-white rounded-2xl overflow-hidden shadow-gentle shadow-gentle-hover transition-all duration-300">
                <img src="https://placehold.co/400x300/F7F5E6/BFB0A3?text=Cozy+Pottery" alt="Handmade cozy pottery" class="w-full h-56 object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x300/cccccc/ffffff?text=Image+Not+Found';">
                <div class="p-6">
                    <h3 class="font-semibold text-xl mb-2 text-gray-800">Morning Dew Mugs</h3>
                    <div class="flex items-center text-gray-500">
                        <img src="https://placehold.co/40x40/A7D7C5/5E8B7E?text=L" alt="Creator Avatar" class="w-8 h-8 rounded-full mr-3 border-2 border-white">
                        <span>Leo Clayfield</span>
                    </div>
                </div>
            </div>
            <!-- Card 3 -->
            <div class="bg-white rounded-2xl overflow-hidden shadow-gentle shadow-gentle-hover transition-all duration-300">
                <img src="https://placehold.co/400x300/FFD1BA/E86A33?text=Sky+Castle" alt="Artwork of a castle in the sky" class="w-full h-56 object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x300/cccccc/ffffff?text=Image+Not+Found';">
                <div class="p-6">
                    <h3 class="font-semibold text-xl mb-2 text-gray-800">Floating Citadel</h3>
                    <div class="flex items-center text-gray-500">
                        <img src="https://placehold.co/40x40/F7F5E6/BFB0A3?text=S" alt="Creator Avatar" class="w-8 h-8 rounded-full mr-3 border-2 border-white">
                        <span>Sophie Skies</span>
                    </div>
                </div>
            </div>
            <!-- Card 4 -->
            <div class="bg-white rounded-2xl overflow-hidden shadow-gentle shadow-gentle-hover transition-all duration-300">
                <img src="https://placehold.co/400x300/C8B6A6/8D7B68?text=Felted+Friend" alt="A small felted animal" class="w-full h-56 object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x300/cccccc/ffffff?text=Image+Not+Found';">
                <div class="p-6">
                    <h3 class="font-semibold text-xl mb-2 text-gray-800">Mossy Knoll Critter</h3>
                    <div class="flex items-center text-gray-500">
                        <img src="https://placehold.co/40x40/A7D7C5/5E8B7E?text=M" alt="Creator Avatar" class="w-8 h-8 rounded-full mr-3 border-2 border-white">
                        <span>Milo Needlefelt</span>
                    </div>
                </div>
            </div>
            <!-- Card 5 -->
            <div class="bg-white rounded-2xl overflow-hidden shadow-gentle shadow-gentle-hover transition-all duration-300">
                <img src="https://placehold.co/400x300/87CEEB/4682B4?text=Night+Train" alt="Animation of a train moving through the night" class="w-full h-56 object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x300/cccccc/ffffff?text=Image+Not+Found';">
                <div class="p-6">
                    <h3 class="font-semibold text-xl mb-2 text-gray-800">Starlight Express Loop</h3>
                    <div class="flex items-center text-gray-500">
                        <img src="https://placehold.co/40x40/F7F5E6/BFB0A3?text=C" alt="Creator Avatar" class="w-8 h-8 rounded-full mr-3 border-2 border-white">
                        <span>Celeste Animate</span>
                    </div>
                </div>
            </div>
            <!-- Card 6 -->
            <div class="bg-white rounded-2xl overflow-hidden shadow-gentle shadow-gentle-hover transition-all duration-300">
                <img src="https://placehold.co/400x300/FADADD/F472B6?text=Pink+Scarf" alt="A hand-knitted pink scarf" class="w-full h-56 object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x300/cccccc/ffffff?text=Image+Not+Found';">
                <div class="p-6">
                    <h3 class="font-semibold text-xl mb-2 text-gray-800">Blush Petal Scarf</h3>
                    <div class="flex items-center text-gray-500">
                        <img src="https://placehold.co/40x40/A7D7C5/5E8B7E?text=P" alt="Creator Avatar" class="w-8 h-8 rounded-full mr-3 border-2 border-white">
                        <span>Penelope Yarn</span>
                    </div>
                </div>
            </div>
            <!-- Card 7 -->
            <div class="bg-white rounded-2xl overflow-hidden shadow-gentle shadow-gentle-hover transition-all duration-300">
                <img src="https://placehold.co/400x300/D4AF37/B8860B?text=Gold+Leaf" alt="Golden leaf enamel pin" class="w-full h-56 object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x300/cccccc/ffffff?text=Image+Not+Found';">
                <div class="p-6">
                    <h3 class="font-semibold text-xl mb-2 text-gray-800">Faded Gold Leaf Pin</h3>
                    <div class="flex items-center text-gray-500">
                        <img src="https://placehold.co/40x40/F7F5E6/BFB0A3?text=G" alt="Creator Avatar" class="w-8 h-8 rounded-full mr-3 border-2 border-white">
                        <span>Gilda Forge</span>
                    </div>
                </div>
            </div>
            <!-- Card 8 -->
            <div class="bg-white rounded-2xl overflow-hidden shadow-gentle shadow-gentle-hover transition-all duration-300">
                <img src="https://placehold.co/400x300/B0E0E6/87CEEB?text=River+Scene" alt="Watercolor painting of a river" class="w-full h-56 object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x300/cccccc/ffffff?text=Image+Not+Found';">
                <div class="p-6">
                    <h3 class="font-semibold text-xl mb-2 text-gray-800">Lazy River Journey</h3>
                    <div class="flex items-center text-gray-500">
                        <img src="https://placehold.co/40x40/A7D7C5/5E8B7E?text=R" alt="Creator Avatar" class="w-8 h-8 rounded-full mr-3 border-2 border-white">
                        <span>River Painter</span>
                    </div>
                </div>
            </div>
        </main>

        <!-- Featured Creators -->
        <section class="mt-24">
            <h2 class="font-ghibli text-4xl text-center text-green-800 mb-12">Featured Creators</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-10">
                <div class="flex flex-col items-center text-center p-8 bg-white/50 rounded-2xl shadow-gentle">
                    <img src="https://placehold.co/100x100/A7D7C5/5E8B7E?text=A" alt="Creator Avatar" class="w-28 h-28 rounded-full mb-5 border-4 border-white">
                    <h4 class="font-semibold text-xl text-gray-800">Anna Evergreen</h4>
                    <p class="text-gray-500">Illustrator of magical worlds</p>
                </div>
                <div class="flex flex-col items-center text-center p-8 bg-white/50 rounded-2xl shadow-gentle">
                    <img src="https://placehold.co/100x100/F7F5E6/BFB0A3?text=L" alt="Creator Avatar" class="w-28 h-28 rounded-full mb-5 border-4 border-white">
                    <h4 class="font-semibold text-xl text-gray-800">Leo Clayfield</h4>
                    <p class="text-gray-500">Potter of cozy companions</p>
                </div>
                <div class="flex flex-col items-center text-center p-8 bg-white/50 rounded-2xl shadow-gentle">
                    <img src="https://placehold.co/100x100/FFD1BA/E86A33?text=S" alt="Creator Avatar" class="w-28 h-28 rounded-full mb-5 border-4 border-white">
                    <h4 class="font-semibold text-xl text-gray-800">Sophie Skies</h4>
                    <p class="text-gray-500">Dreamer of floating castles</p>
                </div>
                <div class="flex flex-col items-center text-center p-8 bg-white/50 rounded-2xl shadow-gentle">
                    <img src="https://placehold.co/100x100/C8B6A6/8D7B68?text=M" alt="Creator Avatar" class="w-28 h-28 rounded-full mb-5 border-4 border-white">
                    <h4 class="font-semibold text-xl text-gray-800">Milo Needlefelt</h4>
                    <p class="text-gray-500">Crafter of felted friends</p>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="text-center mt-24 pt-12 border-t border-white/30 text-gray-500">
            <p class="font-ghibli text-xl">Artisan's Meadow</p>
            <p class="mt-2">A place for creators to share their dreams.</p>
            <div class="flex justify-center space-x-8 mt-6 text-base">
                <a href="#" class="hover:text-green-700 transition duration-300">About</a>
                <a href="#" class="hover:text-green-700 transition duration-300">Careers</a>
                <a href="#" class="hover:text-green-700 transition duration-300">Press</a>
                <a href="#" class="hover:text-green-700 transition duration-300">Help</a>
            </div>
        </footer>

    </div>

</body>
</html>
