# haaayyy selamat datang!!!

-------------------------------
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Enhanced GitHub Profile - Redmoi</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #d90429;
            --secondary: #ef233c;
            --dark: #2b2d42;
            --light: #edf2f4;
            --accent: #8d99ae;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f8f9fa;
        }
        
        .profile-card {
            box-shadow: 0 10px 30px rgba(217, 4, 41, 0.1);
            transition: transform 0.3s;
        }
        
        .profile-card:hover {
            transform: translateY(-5px);
        }
        
        .stats-card {
            transition: all 0.3s ease;
        }
        
        .stats-card:hover {
            transform: scale(1.03);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .repo-card {
            transition: all 0.3s ease;
        }
        
        .repo-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 7px 20px rgba(217, 4, 41, 0.1);
        }
        
        .language-bar {
            height: 8px;
            border-radius: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .animate-fade-in {
            animation: fadeIn 0.6s ease forwards;
        }
        
        .delay-1 { animation-delay: 0.2s; }
        .delay-2 { animation-delay: 0.4s; }
        .delay-3 { animation-delay: 0.6s; }
    </style>
</head>
<body class="bg-gradient-to-b from-gray-50 to-gray-100 min-h-screen py-12 px-4 sm:px-6 lg:px-8">
    <div class="max-w-6xl mx-auto">
        <!-- Header -->
        <div class="text-center mb-12">
            <h1 class="text-4xl font-bold text-gray-900 mb-2">
                <span class="bg-gradient-to-r from-red-600 to-red-400 bg-clip-text text-transparent">Redmoi</span> GitHub Profile
            </h1>
            <p class="text-lg text-gray-600">Enhanced with beautiful UI and interactive elements</p>
        </div>
        
        <!-- Profile Section -->
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 mb-12">
            <!-- Left Column - Profile -->
            <div class="profile-card bg-white rounded-2xl p-6 shadow-md animate-fade-in">
                <div class="flex flex-col items-center">
                    <div class="relative mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/467812c4-3076-4402-9d01-1efdbf53e675.png" alt="Profile picture of Redmoi showing a stylized avatar with red accents and modern design" class="w-40 h-40 rounded-full border-4 border-white shadow-lg" onerror="this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/10158a21-9af0-4266-bd60-22c3c6b7d994.png'">
                        <div class="absolute bottom-0 right-0 bg-red-500 text-white rounded-full p-1">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                        </div>
                    </div>
                    <h2 class="text-2xl font-bold text-gray-800">Redmoi</h2>
                    <p class="text-gray-600 mb-4">Full Stack Developer | UI/UX Enthusiast</p>
                    <div class="flex space-x-2 mb-6">
                        <span class="bg-red-100 text-red-800 text-xs px-2 py-1 rounded">JavaScript</span>
                        <span class="bg-blue-100 text-blue-800 text-xs px-2 py-1 rounded">React</span>
                        <span class="bg-purple-100 text-purple-800 text-xs px-2 py-1 rounded">Node.js</span>
                    </div>
                    <div class="w-full border-t border-gray-200 pt-4">
                        <div class="flex justify-between text-sm text-gray-500 mb-2">
                            <span>Location</span>
                            <span class="text-gray-700 font-medium">Indonesia</span>
                        </div>
                        <div class="flex justify-between text-sm text-gray-500 mb-2">
                            <span>Followers</span>
                            <span class="text-gray-700 font-medium">1.2k</span>
                        </div>
                        <div class="flex justify-between text-sm text-gray-500">
                            <span>Following</span>
                            <span class="text-gray-700 font-medium">45</span>
                        </div>
                    </div>
                    <button class="mt-6 px-6 py-2 bg-gradient-to-r from-red-500 to-red-600 text-white rounded-full font-medium hover:from-red-600 hover:to-red-700 transition-all duration-300 shadow-lg flex items-center">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M12.586 4.586a2 2 0 112.828 2.828l-3 3a2 2 0 01-2.828 0 1 1 0 00-1.414 1.414 4 4 0 005.656 0l3-3a4 4 0 00-5.656-5.656l-1.5 1.5a1 1 0 101.414 1.414l1.5-1.5zm-5 5a2 2 0 012.828 0 1 1 0 101.414-1.414 4 4 0 00-5.656 0l-3 3a4 4 0 105.656 5.656l1.5-1.5a1 1 0 10-1.414-1.414l-1.5 1.5a2 2 0 11-2.828-2.828l3-3z" clip-rule="evenodd" />
                        </svg>
                        View Profile
                    </button>
                </div>
            </div>
            
            <!-- Middle Column - Stats -->
            <div class="lg:col-span-2 space-y-4 animate-fade-in delay-1">
                <!-- Activity Stats -->
                <div class="stats-card bg-white rounded-2xl p-6 shadow-md">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-red-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
                        </svg>
                        Activity Statistics
                    </h3>
                    <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                        <div class="text-center">
                            <div class="text-3xl font-bold text-red-500 mb-1">287</div>
                            <div class="text-sm text-gray-500">Contributions</div>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl font-bold text-red-500 mb-1">58</div>
                            <div class="text-sm text-gray-500">Repositories</div>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl font-bold text-red-500 mb-1">24</div>
                            <div class="text-sm text-gray-500">Stars</div>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl font-bold text-red-500 mb-1">16</div>
                            <div class="text-sm text-gray-500">Pull Requests</div>
                        </div>
                    </div>
                    
                    <div class="mt-6">
                        <h4 class="text-sm font-medium text-gray-700 mb-2">Contribution Graph</h4>
                        <div class="flex items-center justify-center">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/80638790-0de9-4f3e-8411-ed64c49cd8d5.png" alt="GitHub contribution graph showing daily activity with red squares indicating high activity on recent days" class="rounded-lg shadow-inner w-full max-w-md" onerror="this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/6bf7bf6e-6ecf-49aa-bac7-ae7d5d2421c0.png'">
                        </div>
                    </div>
                </div>
                
                <!-- Languages -->
                <div class="stats-card bg-white rounded-2xl p-6 shadow-md">
                    <h3 class="text-xl font-semibold text-gray-800 mb-6 flex items-center">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-red-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                        </svg>
                        Top Languages
                    </h3>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between text-sm text-gray-600 mb-1">
                                <span>JavaScript</span>
                                <span>42%</span>
                            </div>
                            <div class="language-bar bg-gray-200 h-2 rounded-full">
                                <div class="bg-red-500 h-full rounded-full" style="width: 42%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-sm text-gray-600 mb-1">
                                <span>HTML</span>
                                <span>28%</span>
                            </div>
                            <div class="language-bar bg-gray-200 h-2 rounded-full">
                                <div class="bg-orange-500 h-full rounded-full" style="width: 28%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-sm text-gray-600 mb-1">
                                <span>CSS</span>
                                <span>18%</span>
                            </div>
                            <div class="language-bar bg-gray-200 h-2 rounded-full">
                                <div class="bg-blue-500 h-full rounded-full" style="width: 18%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-sm text-gray-600 mb-1">
                                <span>Python</span>
                                <span>12%</span>
                            </div>
                            <div class="language-bar bg-gray-200 h-2 rounded-full">
                                <div class="bg-yellow-500 h-full rounded-full" style="width: 12%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Repositories Section -->
        <div class="animate-fade-in delay-2">
            <div class="flex justify-between items-center mb-6">
                <h2 class="text-2xl font-bold text-gray-900">Popular Repositories</h2>
                <button class="text-sm text-red-500 hover:text-red-600 font-medium">View All</button>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Repo 1 -->
                <div class="repo-card bg-white rounded-xl p-6 shadow-md cursor-pointer transition-all duration-300 hover:border-red-500 border border-transparent">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-lg font-semibold text-gray-800">awesome-web-dev</h3>
                        <span class="flex items-center text-sm text-gray-500">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z" />
                            </svg>
                            34
                        </span>
                    </div>
                    <p class="text-sm text-gray-600 mb-4">Collection of awesome web development resources, tools and libraries</p>
                    <div class="flex justify-between items-center text-xs text-gray-500">
                        <div class="flex items-center">
                            <span class="w-3 h-3 rounded-full bg-red-500 mr-2"></span>
                            <span>JavaScript</span>
                        </div>
                        <span>Updated 3 days ago</span>
                    </div>
                </div>
                
                <!-- Repo 2 -->
                <div class="repo-card bg-white rounded-xl p-6 shadow-md cursor-pointer transition-all duration-300 hover:border-red-500 border border-transparent">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-lg font-semibold text-gray-800">ui-components</h3>
                        <span class="flex items-center text-sm text-gray-500">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z" />
                            </svg>
                            27
                        </span>
                    </div>
                    <p class="text-sm text-gray-600 mb-4">Reusable UI components library with React and Tailwind CSS</p>
                    <div class="flex justify-between items-center text-xs text-gray-500">
                        <div class="flex items-center">
                            <span class="w-3 h-3 rounded-full bg-blue-500 mr-2"></span>
                            <span>TypeScript</span>
                        </div>
                        <span>Updated 1 week ago</span>
                    </div>
                </div>
                
                <!-- Repo 3 -->
                <div class="repo-card bg-white rounded-xl p-6 shadow-md cursor-pointer transition-all duration-300 hover:border-red-500 border border-transparent">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-lg font-semibold text-gray-800">portfolio-v2</h3>
                        <span class="flex items-center text-sm text-gray-500">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z" />
                            </svg>
                            18
                        </span>
                    </div>
                    <p class="text-sm text-gray-600 mb-4">My personal portfolio website built with Next.js and Framer Motion</p>
                    <div class="flex justify-between items-center text-xs text-gray-500">
                        <div class="flex items-center">
                            <span class="w-3 h-3 rounded-full bg-purple-500 mr-2"></span>
                            <span>CSS</span>
                        </div>
                        <span>Updated 2 weeks ago</span>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Footer -->
        <div class="mt-16 text-center text-gray-500 text-sm animate-fade-in delay-3">
            <p>© 2023 Redmoi. All rights reserved. Inspired by GitHub profile.</p>
            <div class="flex justify-center space-x-6 mt-4">
                <a href="#" class="text-gray-400 hover:text-red-500">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                    </svg>
                </a>
                <a href="#" class="text-gray-400 hover:text-red-500">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
                    </svg>
                </a>
                <a href="#" class="text-gray-400 hover:text-red-500">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"/>
                    </svg>
                </a>
            </div>
        </div>
    </div>

    <script>
        // Animation trigger with Intersection Observer
        document.addEventListener('DOMContentLoaded', function() {
            const animateElements = document.querySelectorAll('.animate-fade-in');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
            animateElements.forEach(el => {
                el.style.opacity = 0;
                el.style.transform = 'translateY(20px)';
                el.style.transition = 'all 0.6s ease';
                observer.observe(el);
            });
            
            // Add hover effect to repo cards
            const repoCards = document.querySelectorAll('.repo-card');
            repoCards.forEach(card => {
                card.addEventListener('mouseenter', () => {
                    card.style.boxShadow = '0 10px 25px rgba(217, 4, 41, 0.15)';
                });
                
                card.addEventListener('mouseleave', () => {
                    card.style.boxShadow = '0 4px 6px rgba(0, 0, 0, 0.1)';
                });
            });
        });
    </script>
</body>
</html>

