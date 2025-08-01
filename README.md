<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Machel's - Family Blog</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .hero {
            background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1529333166437-7750a6dd5a70?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2069&q=80');
            background-size: cover;
            background-position: center;
        }
        
        .video-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .family-member:hover img {
            transform: scale(1.05);
        }
        
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: #888;
            border-radius: 10px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #555;
        }
    </style>
</head>
<body class="font-sans bg-gray-50 text-gray-800">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <i class="fas fa-home text-2xl text-indigo-600 mr-2"></i>
                        <span class="text-xl font-bold text-indigo-600">The Machel's</span>
                    </div>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="text-gray-900 hover:text-indigo-600 px-3 py-2 text-sm font-medium">Home</a>
                    <a href="#about" class="text-gray-900 hover:text-indigo-600 px-3 py-2 text-sm font-medium">About Us</a>
                    <a href="#videos" class="text-gray-900 hover:text-indigo-600 px-3 py-2 text-sm font-medium">Videos</a>
                    <a href="#blog" class="text-gray-900 hover:text-indigo-600 px-3 py-2 text-sm font-medium">Blog</a>
                    <a href="#contact" class="text-gray-900 hover:text-indigo-600 px-3 py-2 text-sm font-medium">Contact</a>
                </div>
                <div class="md:hidden flex items-center">
                    <button id="menu-btn" class="text-gray-900 hover:text-indigo-600">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile menu -->
        <div id="mobile-menu" class="md:hidden hidden bg-white border-t">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="block px-3 py-2 text-base font-medium text-gray-900 hover:text-indigo-600">Home</a>
                <a href="#about" class="block px-3 py-2 text-base font-medium text-gray-900 hover:text-indigo-600">About Us</a>
                <a href="#videos" class="block px-3 py-2 text-base font-medium text-gray-900 hover:text-indigo-600">Videos</a>
                <a href="#blog" class="block px-3 py-2 text-base font-medium text-gray-900 hover:text-indigo-600">Blog</a>
                <a href="#contact" class="block px-3 py-2 text-base font-medium text-gray-900 hover:text-indigo-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero h-screen flex items-center justify-center text-white">
        <div class="text-center px-4">
            <h1 class="text-4xl md:text-6xl font-bold mb-6">Welcome to The Machel's</h1>
            <p class="text-xl md:text-2xl mb-8 max-w-2xl mx-auto">Sharing our family adventures, memories, and everyday moments with you</p>
            <div class="flex justify-center space-x-4">
                <a href="#videos" class="bg-indigo-600 hover:bg-indigo-700 text-white px-6 py-3 rounded-full font-medium transition duration-300">Watch Videos</a>
                <a href="#blog" class="bg-white hover:bg-gray-100 text-indigo-600 px-6 py-3 rounded-full font-medium transition duration-300">Read Blog</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Our Family Story</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="flex flex-col md:flex-row items-center mb-16">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-10">
                    <h3 class="text-2xl font-bold mb-4">Who We Are</h3>
                    <p class="text-gray-600 mb-4">We're the Machel family - a loving bunch who enjoys sharing our life's journey with friends and family. Through this blog, we hope to document our adventures, milestones, and the little moments that make life special.</p>
                    <p class="text-gray-600">From family vacations to Sunday dinners, school events to holiday traditions, we're excited to have you along for the ride!</p>
                </div>
                <div class="md:w-1/2">
                    <img src="https://images.unsplash.com/photo-1518621736915-f3b1c41bfd00?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2073&q=80" alt="Family photo" class="rounded-lg shadow-xl w-full h-auto">
                </div>
            </div>
            
            <div class="text-center mt-20">
                <h3 class="text-2xl font-bold mb-8">Meet The Family</h3>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                    <!-- Family Member 1 -->
                    <div class="family-member bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                        <div class="w-32 h-32 mx-auto mb-4 overflow-hidden rounded-full border-4 border-indigo-100">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Dad" class="w-full h-full object-cover transition duration-300">
                        </div>
                        <h4 class="text-xl font-semibold mb-1">John</h4>
                        <p class="text-indigo-600 mb-2">Dad</p>
                        <p class="text-gray-600 text-sm">The rock of our family who loves telling dad jokes and grilling on weekends.</p>
                    </div>
                    
                    <!-- Family Member 2 -->
                    <div class="family-member bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                        <div class="w-32 h-32 mx-auto mb-4 overflow-hidden rounded-full border-4 border-indigo-100">
                            <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Mom" class="w-full h-full object-cover transition duration-300">
                        </div>
                        <h4 class="text-xl font-semibold mb-1">Sarah</h4>
                        <p class="text-indigo-600 mb-2">Mom</p>
                        <p class="text-gray-600 text-sm">The organizer who keeps us all on track and makes the best chocolate chip cookies.</p>
                    </div>
                    
                    <!-- Family Member 3 -->
                    <div class="family-member bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                        <div class="w-32 h-32 mx-auto mb-4 overflow-hidden rounded-full border-4 border-indigo-100">
                            <img src="https://randomuser.me/api/portraits/women/12.jpg" alt="Daughter" class="w-full h-full object-cover transition duration-300">
                        </div>
                        <h4 class="text-xl font-semibold mb-1">Emily</h4>
                        <p class="text-indigo-600 mb-2">Daughter</p>
                        <p class="text-gray-600 text-sm">Our creative soul who loves painting, dancing, and reading mystery novels.</p>
                    </div>
                    
                    <!-- Family Member 4 -->
                    <div class="family-member bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                        <div class="w-32 h-32 mx-auto mb-4 overflow-hidden rounded-full border-4 border-indigo-100">
                            <img src="https://randomuser.me/api/portraits/men/22.jpg" alt="Son" class="w-full h-full object-cover transition duration-300">
                        </div>
                        <h4 class="text-xl font-semibold mb-1">Michael</h4>
                        <p class="text-indigo-600 mb-2">Son</p>
                        <p class="text-gray-600 text-sm">The tech whiz who's always building something new and loves soccer.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Videos Section -->
    <section id="videos" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Our Family Videos</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">Watch our latest family adventures, celebrations, and everyday moments captured on video.</p>
            </div>
            
            <!-- Video Grid - You can add/edit your videos here -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Video 1 -->
                <div class="video-card bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="relative pb-[56.25%] bg-gray-200">
                        <!-- Replace with your actual video embed code -->
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Summer Vacation 2023</h3>
                        <p class="text-gray-600 text-sm mb-4">Our amazing family trip to the beach last summer with lots of fun activities.</p>
                        <div class="flex items-center text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> June 15, 2023</span>
                            <span class="ml-4"><i class="fas fa-clock mr-1"></i> 8:32</span>
                        </div>
                    </div>
                </div>
                
                <!-- Video 2 -->
                <div class="video-card bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="relative pb-[56.25%] bg-gray-200">
                        <!-- Replace with your actual video embed code -->
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Emily's Dance Recital</h3>
                        <p class="text-gray-600 text-sm mb-4">Watch Emily's beautiful ballet performance at her annual dance recital.</p>
                        <div class="flex items-center text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> May 5, 2023</span>
                            <span class="ml-4"><i class="fas fa-clock mr-1"></i> 5:15</span>
                        </div>
                    </div>
                </div>
                
                <!-- Video 3 -->
                <div class="video-card bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="relative pb-[56.25%] bg-gray-200">
                        <!-- Replace with your actual video embed code -->
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Sunday Brunch at Home</h3>
                        <p class="text-gray-600 text-sm mb-4">Our weekly family tradition of making pancakes and enjoying time together.</p>
                        <div class="flex items-center text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> April 2, 2023</span>
                            <span class="ml-4"><i class="fas fa-clock mr-1"></i> 12:45</span>
                        </div>
                    </div>
                </div>
                
                <!-- Video 4 -->
                <div class="video-card bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="relative pb-[56.25%] bg-gray-200">
                        <!-- Replace with your actual video embed code -->
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Michael's Science Project</h3>
                        <p class="text-gray-600 text-sm mb-4">Michael demonstrates his award-winning volcano science project.</p>
                        <div class="flex items-center text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> March 18, 2023</span>
                            <span class="ml-4"><i class="fas fa-clock mr-1"></i> 4:22</span>
                        </div>
                    </div>
                </div>
                
                <!-- Video 5 -->
                <div class="video-card bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="relative pb-[56.25%] bg-gray-200">
                        <!-- Replace with your actual video embed code -->
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Christmas Morning 2022</h3>
                        <p class="text-gray-600 text-sm mb-4">The kids opening presents on Christmas morning - so much excitement!</p>
                        <div class="flex items-center text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> December 25, 2022</span>
                            <span class="ml-4"><i class="fas fa-clock mr-1"></i> 15:08</span>
                        </div>
                    </div>
                </div>
                
                <!-- Video 6 -->
                <div class="video-card bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="relative pb-[56.25%] bg-gray-200">
                        <!-- Replace with your actual video embed code -->
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Family Game Night</h3>
                        <p class="text-gray-600 text-sm mb-4">We play board games every Friday night - this time it got very competitive!</p>
                        <div class="flex items-center text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> November 11, 2022</span>
                            <span class="ml-4"><i class="fas fa-clock mr-1"></i> 22:17</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <button class="bg-indigo-600 hover:bg-indigo-700 text-white px-6 py-3 rounded-full font-medium transition duration-300">
                    Load More Videos
                </button>
            </div>
        </div>
    </section>

    <!-- Blog Section -->
    <section id="blog" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Latest Blog Posts</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">Read about our family experiences, parenting tips, and life lessons we've learned along the way.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Blog Post 1 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="h-48 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1506126613408-eca07ce68773?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1999&q=80" alt="Vacation" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <div class="flex items-center text-sm text-gray-500 mb-2">
                            <span><i class="fas fa-calendar-alt mr-1"></i> July 10, 2023</span>
                            <span class="ml-4"><i class="fas fa-user mr-1"></i> Sarah</span>
                        </div>
                        <h3 class="text-xl font-semibold mb-3">Our Summer Vacation Highlights</h3>
                        <p class="text-gray-600 mb-4">This year's family vacation was one for the books! From beach days to exploring local attractions, we made so many wonderful memories...</p>
                        <a href="#" class="text-indigo-600 font-medium hover:text-indigo-800 transition duration-300">Read More <i class="fas fa-arrow-right ml-1"></i></a>
                    </div>
                </div>
                
                <!-- Blog Post 2 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="h-48 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1541178735493-479c1a27ed24?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2071&q=80" alt="School" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <div class="flex items-center text-sm text-gray-500 mb-2">
                            <span><i class="fas fa-calendar-alt mr-1"></i> June 2, 2023</span>
                            <span class="ml-4"><i class="fas fa-user mr-1"></i> John</span>
                        </div>
                        <h3 class="text-xl font-semibold mb-3">Balancing Work and Family Time</h3>
                        <p class="text-gray-600 mb-4">As a working parent, finding that perfect balance between career and family can be challenging. Here's what I've learned over the years...</p>
                        <a href="#" class="text-indigo-600 font-medium hover:text-indigo-800 transition duration-300">Read More <i class="fas fa-arrow-right ml-1"></i></a>
                    </div>
                </div>
                
                <!-- Blog Post 3 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300">
                    <div class="h-48 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1519208250240-2096f3a577b4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Dinner" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <div class="flex items-center text-sm text-gray-500 mb-2">
                            <span><i class="fas fa-calendar-alt mr-1"></i> May 15, 2023</span>
                            <span class="ml-4"><i class="fas fa-user mr-1"></i> Emily</span>
                        </div>
                        <h3 class="text-xl font-semibold mb-3">Our Favorite Family Recipes</h3>
                        <p class="text-gray-600 mb-4">Food brings our family together. Here are some of our favorite recipes that have been passed down through generations...</p>
                        <a href="#" class="text-indigo-600 font-medium hover:text-indigo-800 transition duration-300">Read More <i class="fas fa-arrow-right ml-1"></i></a>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <button class="bg-indigo-600 hover:bg-indigo-700 text-white px-6 py-3 rounded-full font-medium transition duration-300">
                    View All Blog Posts
                </button>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="py-16 bg-indigo-600 text-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-3xl font-bold mb-4">Stay Updated With Our Family</h2>
            <p class="text-indigo-100 mb-8 max-w-2xl mx-auto">Subscribe to our newsletter to get notified about new videos, blog posts, and family updates.</p>
            <form class="flex flex-col sm:flex-row justify-center max-w-md mx-auto">
                <input type="email" placeholder="Your email address" class="px-4 py-3 rounded-l-full sm:rounded-r-none rounded-r-full sm:w-2/3 focus:outline-none text-gray-900">
                <button type="submit" class="mt-2 sm:mt-0 sm:ml-2 bg-white text-indigo-600 px-6 py-3 rounded-r-full sm:rounded-l-none rounded-l-full font-medium hover:bg-gray-100 transition duration-300">Subscribe</button>
            </form>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Get In Touch</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">We'd love to hear from you! Send us a message or connect with us on social media.</p>
            </div>
            
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-10">
                    <form class="space-y-6">
                        <div>
                            <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Your Name</label>
                            <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-600 focus:border-indigo-600">
                        </div>
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email Address</label>
                            <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-600 focus:border-indigo-600">
                        </div>
                        <div>
                            <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Your Message</label>
                            <textarea id="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-600 focus:border-indigo-600"></textarea>
                        </div>
                        <button type="submit" class="bg-indigo-600 hover:bg-indigo-700 text-white px-6 py-3 rounded-full font-medium transition duration-300 w-full">Send Message</button>
                    </form>
                </div>
                
                <div class="md:w-1/2 md:pl-10">
                    <div class="bg-white p-8 rounded-lg shadow-md">
                        <h3 class="text-xl font-semibold mb-4">Contact Information</h3>
                        <div class="space-y-4">
                            <div class="flex items-start">
                                <i class="fas fa-map-marker-alt text-indigo-600 mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-medium">Address</h4>
                                    <p class="text-gray-600">123 Family Street, Hometown, USA</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-envelope text-indigo-600 mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-medium">Email</h4>
                                    <p class="text-gray-600">hello@themachels.com</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-phone-alt text-indigo-600 mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-medium">Phone</h4>
                                    <p class="text-gray-600">(123) 456-7890</p>
                                </div>
                            </div>
                        </div>
                        
                        <h3 class="text-xl font-semibold mt-8 mb-4">Follow Us</h3>
                        <div class="flex space-x-4">
                            <a href="#" class="w-10 h-10 rounded-full bg-indigo-100 text-indigo-600 flex items-center justify-center hover:bg-indigo-200 transition duration-300">
                                <i class="fab fa-facebook-f"></i>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-full bg-indigo-100 text-indigo-600 flex items-center justify-center hover:bg-indigo-200 transition duration-300">
                                <i class="fab fa-instagram"></i>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-full bg-indigo-100 text-indigo-600 flex items-center justify-center hover:bg-indigo-200 transition duration-300">
                                <i class="fab fa-youtube"></i>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-full bg-indigo-100 text-indigo-600 flex items-center justify-center hover:bg-indigo-200 transition duration-300">
                                <i class="fab fa-pinterest-p"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">The Machel's</h3>
                    <p class="text-gray-400">Sharing our family's journey, one memory at a time.</p>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#home" class="text-gray-400 hover:text-white transition duration-300">Home</a></li>
                        <li><a href="#about" class="text-gray-400 hover:text-white transition duration-300">About Us</a></li>
                        <li><a href="#videos" class="text-gray-400 hover:text-white transition duration-300">Videos</a></li>
                        <li><a href="#blog" class="text-gray-400 hover:text-white transition duration-300">Blog</a></li>
                        <li><a href="#contact" class="text-gray-400 hover:text-white transition duration-300">Contact</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Categories</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Family Adventures</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Parenting Tips</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Recipes</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Travel</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Holidays</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Newsletter</h4>
                    <p class="text-gray-400 mb-4">Subscribe to get updates on new content.</p>
                    <form class="flex">
                        <input type="email" placeholder="Your email" class="px-4 py-2 rounded-l text-gray-900 w-full focus:outline-none">
                        <button type="submit" class="bg-indigo-600 hover:bg-indigo-700 px-4 py-2 rounded-r">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </form>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 text-sm mb-4 md:mb-0">© 2023 The Machel's. All rights reserved.</p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300"><i class="fab fa-facebook-f"></i></a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300"><i class="fab fa-youtube"></i></a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300"><i class="fab fa-pinterest-p"></i></a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
                
                // Close mobile menu if open
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                }
            });
        });
    </script>
</body>
</html>
