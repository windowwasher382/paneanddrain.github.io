<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pane and Drain Bros - Window & Gutter Cleaning</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts - Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f9fafb; /* Very light gray for a clean base */
        }
        .hero-section {
            /* Updated hero image to reflect cleaning services, using emerald tones */
            background-image: url('https://placehold.co/1920x600/10b981/ffffff?text=Sparkling+Clean+Home');
            background-size: cover;
            background-position: center;
            position: relative;
            color: white;
            padding: 8rem 0;
        }
        .hero-overlay {
            background-color: rgba(0, 0, 0, 0.5); /* Dark overlay for text readability */
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
        }
        /* Custom styles for the logo */
        .logo-container {
            display: flex;
            align-items: center;
            gap: 8px; /* Space between icon and text */
            color: #1a202c; /* Dark gray for text */
            font-weight: 700; /* Bold font */
            font-size: 1.5rem; /* Equivalent to text-2xl */
        }
        .logo-icon {
            width: 32px; /* Size of the SVG icon */
            height: 32px;
            color: #059669; /* Emerald color for the icon */
        }

        /* Star Rating CSS */
        .star-rating {
            display: inline-block;
            direction: rtl; /* Right-to-left for star order */
        }
        .star-rating input {
            display: none; /* Hide radio buttons */
        }
        .star-rating label {
            font-size: 2rem; /* Size of the stars */
            color: #ccc; /* Default star color */
            cursor: pointer;
            padding: 0 5px;
            transition: color 0.2s ease-in-out;
        }
        .star-rating input:checked ~ label {
            color: #facc15; /* Gold color for checked stars */
        }
        .star-rating label:hover,
        .star-rating label:hover ~ label {
            color: #facc15; /* Gold color on hover */
        }
    </style>
</head>
<body class="antialiased">

    <!-- Header/Navigation -->
    <header class="bg-white shadow-md py-4">
        <nav class="container mx-auto px-4 flex justify-between items-center">
            <a href="#" class="logo-container rounded-md p-2 hover:bg-gray-100">
                <!-- SVG Logo Icon: Represents a clean window and a drop/drain -->
                <svg class="logo-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect>
                    <line x1="12" y1="3" x2="12" y2="21"></line>
                    <line x1="3" y1="12" x2="21" y2="12"></line>
                    <path d="M9 18l3 3 3-3"></path>
                </svg>
                <span>Pane and Drain Bros</span>
            </a>
            <div class="space-x-4 hidden md:block">
                <a href="#services" class="text-gray-600 hover:text-emerald-600 px-3 py-2 rounded-md transition duration-300">Services</a>
                <a href="#reviews" class="text-gray-600 hover:text-emerald-600 px-3 py-2 rounded-md transition duration-300">Reviews</a>
                <a href="#about" class="text-gray-600 hover:text-emerald-600 px-3 py-2 rounded-md transition duration-300">About Us</a>
                <a href="#contact" class="text-gray-600 hover:text-emerald-600 px-3 py-2 rounded-md transition duration-300">Contact</a>
            </div>
            <!-- Mobile Menu Button -->
            <button id="mobile-menu-button" class="md:hidden text-gray-600 hover:text-emerald-600 focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path></svg>
            </button>
        </nav>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-lg py-2 mt-2">
            <a href="#services" class="block px-4 py-2 text-gray-800 hover:bg-gray-100 rounded-md">Services</a>
            <a href="#reviews" class="block px-4 py-2 text-gray-800 hover:bg-gray-100 rounded-md">Reviews</a>
            <a href="#about" class="block px-4 py-2 text-gray-800 hover:bg-gray-100 rounded-md">About Us</a>
            <a href="#contact" class="block px-4 py-2 text-gray-800 hover:bg-gray-100 rounded-md">Contact</a>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero-section text-center">
        <div class="hero-overlay"></div>
        <div class="relative z-10 container mx-auto px-4">
            <h1 class="text-5xl md:text-6xl font-extrabold mb-4 leading-tight">Sparkling Clean Windows & Clog-Free Gutters</h1>
            <p class="text-xl md:text-2xl mb-8">Your trusted local experts in New Concord & Zanesville, Ohio.</p>
            <a href="#contact" class="bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-3 px-8 rounded-full text-lg shadow-lg transition duration-300 transform hover:scale-105">Get a Free Estimate</a>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-4xl font-bold text-gray-800 mb-12">Our Services</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-3xl mx-auto">
                <!-- Service Card 1: Window Cleaning -->
                <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-xl transition duration-300 transform hover:-translate-y-1">
                    <!-- Placeholder icon for window cleaning with emerald background -->
                    <img src="https://placehold.co/80x80/059669/ffffff?text=Window" alt="Window Cleaning Icon" class="mx-auto mb-6 rounded-full p-3 bg-emerald-100">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-4">Professional Window Cleaning</h3>
                    <p class="text-gray-600">Achieve streak-free, crystal-clear windows for your home or business. We handle all types of windows, ensuring a spotless shine every time.</p>
                </div>
                <!-- Service Card 2: Gutter Cleaning -->
                <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-xl transition duration-300 transform hover:-translate-y-1">
                    <!-- Placeholder icon for gutter cleaning with emerald background -->
                    <img src="https://placehold.co/80x80/059669/ffffff?text=Gutter" alt="Gutter Cleaning Icon" class="mx-auto mb-6 rounded-full p-3 bg-emerald-100">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-4">Thorough Gutter Cleaning</h3>
                    <p class="text-gray-600">Protect your property from water damage with our comprehensive gutter cleaning services. We remove leaves, debris, and blockages to ensure proper drainage.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Customer Reviews Section -->
    <section id="reviews" class="py-16 bg-white">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-4xl font-bold text-gray-800 mb-12">What Our Customers Say</h2>

            <!-- Existing Reviews Display Area - Now empty, ready for dynamic content -->
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-4xl mx-auto mb-12">
                <p class="text-gray-600 col-span-full">Be the first to leave a review!</p>
            </div>

            <h3 class="text-3xl font-bold text-gray-800 mb-8 mt-12">Leave Us a Review!</h3>
            <div class="max-w-xl mx-auto bg-gray-50 p-8 rounded-xl shadow-lg">
                <form class="space-y-6">
                    <div>
                        <label for="reviewer-name" class="block text-left text-gray-700 text-sm font-semibold mb-2">Your Name</label>
                        <input type="text" id="reviewer-name" name="reviewer-name" class="w-full px-4 py-3 rounded-md border border-gray-300 focus:outline-none focus:ring-2 focus:ring-emerald-500" placeholder="Enter your name" required>
                    </div>
                    <div>
                        <label class="block text-left text-gray-700 text-sm font-semibold mb-2">Your Rating</label>
                        <div class="star-rating flex justify-center md:justify-start">
                            <input type="radio" id="star5" name="rating" value="5" /><label for="star5" title="5 stars">&#9733;</label>
                            <input type="radio" id="star4" name="rating" value="4" /><label for="star4" title="4 stars">&#9733;</label>
                            <input type="radio" id="star3" name="rating" value="3" /><label for="star3" title="3 stars">&#9733;</label>
                            <input type="radio" id="star2" name="rating" value="2" /><label for="star2" title="2 stars">&#9733;</label>
                            <input type="radio" id="star1" name="rating" value="1" /><label for="star1" title="1 star">&#9733;</label>
                        </div>
                    </div>
                    <div>
                        <label for="review-text" class="block text-left text-gray-700 text-sm font-semibold mb-2">Your Review</label>
                        <textarea id="review-text" name="review-text" rows="5" class="w-full px-4 py-3 rounded-md border border-gray-300 focus:outline-none focus:ring-2 focus:ring-emerald-500" placeholder="Share your experience with us..." required></textarea>
                    </div>
                    <div>
                        <label for="review-photo" class="block text-left text-gray-700 text-sm font-semibold mb-2">Upload Photo (Optional)</label>
                        <input type="file" id="review-photo" name="review-photo" accept="image/*" class="w-full px-4 py-3 rounded-md border border-gray-300 focus:outline-none focus:ring-2 focus:ring-emerald-500">
                        <p class="text-xs text-gray-500 mt-1 text-left">Note: Photo upload is for demonstration. Actual functionality requires server-side processing.</p>
                    </div>
                    <button type="submit" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-3 px-6 rounded-md text-lg shadow-md transition duration-300 transform hover:scale-105">Submit Review</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Call to Action Section -->
    <section class="py-16 bg-emerald-600 text-white text-center">
        <div class="container mx-auto px-4">
            <h2 class="text-4xl font-bold mb-4">Ready for a Brighter, Cleaner Property?</h2>
            <p class="text-xl mb-8">Get in touch with Pane and Drain Bros today for a free, no-obligation estimate!</p>
            <a href="#contact" class="bg-white text-emerald-600 hover:bg-emerald-100 font-bold py-3 px-8 rounded-full text-lg shadow-lg transition duration-300 transform hover:scale-105">Request Your Free Estimate</a>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-4xl font-bold text-gray-800 mb-12">Contact Us</h2>
            <div class="max-w-xl mx-auto bg-white p-8 rounded-xl shadow-lg">
                <form class="space-y-6">
                    <div>
                        <label for="name" class="block text-left text-gray-700 text-sm font-semibold mb-2">Name</label>
                        <input type="text" id="name" name="name" class="w-full px-4 py-3 rounded-md border border-gray-300 focus:outline-none focus:ring-2 focus:ring-emerald-500" placeholder="Your Name" required>
                    </div>
                    <div>
                        <label for="email" class="block text-left text-gray-700 text-sm font-semibold mb-2">Email</label>
                        <input type="email" id="email" name="email" class="w-full px-4 py-3 rounded-md border border-gray-300 focus:outline-none focus:ring-2 focus:ring-emerald-500" placeholder="your.email@example.com" required>
                    </div>
                    <div>
                        <label for="message" class="block text-left text-gray-700 text-sm font-semibold mb-2">Message</label>
                        <textarea id="message" name="message" rows="5" class="w-full px-4 py-3 rounded-md border border-gray-300 focus:outline-none focus:ring-2 focus:ring-emerald-500" placeholder="Tell us about your window or gutter cleaning needs..." required></textarea>
                    </div>
                    <button type="submit" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-3 px-6 rounded-md text-lg shadow-md transition duration-300 transform hover:scale-105">Send Message</button>
                </form>
            </div>
            <div class="mt-12 text-gray-700">
                <p class="mb-2"><strong class="text-gray-800">Service Area:</strong> New Concord & Zanesville, OH and surrounding areas</p>
                <p class="mb-2"><strong class="text-gray-800">Phone:</strong> 740-624-8940</p>
                <p><strong class="text-gray-800">Email:</strong> painanddrainbros@gmail.com</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-8">
        <div class="container mx-auto px-4 text-center">
            <p>&copy; 2025 Pane and Drain Bros. All rights reserved.</p>
            <div class="flex justify-center space-x-6 mt-4">
                <a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a>
                <a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
                // Close mobile menu if open
                if (mobileMenu.classList.contains('block')) {
                    mobileMenu.classList.remove('block');
                    mobileMenu.classList.add('hidden');
                }
            });
        });

        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            mobileMenu.classList.toggle('block');
        });
    </script>
</body>
</html>
