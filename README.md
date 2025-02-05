<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Personal Resume - Sui Qian</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet" />
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet" />
  <script src="https://cdnjs.cloudflare.com/ajax/libs/echarts/5.5.0/echarts.min.js"></script>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#2563eb',
            secondary: '#3b82f6'
          },
          borderRadius: {
            'none': '0px',
            'sm': '2px',
            DEFAULT: '4px',
            'md': '8px',
            'lg': '12px',
            'xl': '16px',
            '2xl': '20px',
            '3xl': '24px',
            'full': '9999px',
            'button': '4px'
          }
        }
      }
    }
  </script>
  <style>
    html {
      scroll-behavior: smooth;
    }
    body {
      min-height: 1024px;
    }
    .nav-link {
      position: relative;
    }
    .nav-link::after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: -2px;
      left: 0;
      background-color: #2563eb;
      transition: width 0.3s;
    }
    .nav-link:hover::after {
      width: 100%;
    }
    .fade-in {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.6s ease-out, transform 0.6s ease-out;
    }
    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }
    .timeline-item {
      position: relative;
      padding-left: 30px;
    }
    .timeline-item::before {
      content: '';
      position: absolute;
      left: 0;
      top: 0;
      width: 2px;
      height: 100%;
      background: #2563eb;
    }
    .timeline-item::after {
      content: '';
      position: absolute;
      left: -4px;
      top: 0;
      width: 10px;
      height: 10px;
      border-radius: 50%;
      background: #2563eb;
    }
  </style>
</head>
<body class="bg-white">
  <!-- Navigation -->
  <nav class="fixed top-0 w-full bg-white bg-opacity-95 shadow-sm z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center h-16">
        <div class="flex-shrink-0">
          <span class="text-2xl font-['Pacifico'] text-primary">Sui Qian</span>
        </div>
        <div class="hidden md:block">
          <div class="ml-10 flex items-baseline space-x-8">
            <a href="#home" class="nav-link text-gray-700 hover:text-primary px-3 py-2 text-sm font-medium">Home</a>
            <a href="#about" class="nav-link text-gray-700 hover:text-primary px-3 py-2 text-sm font-medium">About Me</a>
            <a href="#experience" class="nav-link text-gray-700 hover:text-primary px-3 py-2 text-sm font-medium">Experience</a>
            <a href="#projects" class="nav-link text-gray-700 hover:text-primary px-3 py-2 text-sm font-medium">Projects</a>
            <a href="#achievements" class="nav-link text-gray-700 hover:text-primary px-3 py-2 text-sm font-medium">Achievements &amp; Patents</a>
            <a href="#education" class="nav-link text-gray-700 hover:text-primary px-3 py-2 text-sm font-medium">Education</a>
            <a href="#contact" class="nav-link text-gray-700 hover:text-primary px-3 py-2 text-sm font-medium">Contact</a>
          </div>
        </div>
      </div>
    </div>
  </nav>

  <!-- Home / Hero Section -->
  <section id="home" class="relative h-screen flex items-center justify-center bg-cover bg-center" style="background-image: url('https://ai-public.mastergo.com/ai/img_res/b50f713be9a71e5e8e928bf2c3f62f5c.jpg');">
    <div class="absolute inset-0 bg-gradient-to-r from-white/90 to-transparent"></div>
    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-left">
        <h1 class="text-5xl font-bold text-gray-900 mb-4">Sui Qian</h1>
        <h2 class="text-3xl font-semibold text-gray-800 mb-6">Senior Internet Product Manager / Technical Product Leader</h2>
        <p class="text-xl text-gray-700 mb-8">9 years of product experience | AI &amp; IoT Expert</p>
        <a href="#about" class="inline-flex items-center px-6 py-3 !rounded-button bg-primary text-white font-medium hover:bg-primary/90 transition-colors whitespace-nowrap">
          Learn More
          <i class="fas fa-arrow-down ml-2"></i>
        </a>
      </div>
    </div>
  </section>

  <!-- About Me Section -->
  <section id="about" class="py-20 bg-gray-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="fade-in">
        <h2 class="text-3xl font-bold text-center text-gray-900 mb-16">About Me</h2>
        <div class="flex flex-wrap items-center">
          <div class="w-full lg:w-3/5 pr-8">
            <p class="text-lg text-gray-700 mb-6">
              I am a technical product leader with 9 years of experience in internet product management, specializing in AI and IoT solutions. I have led key projects at top-tier companies such as Alibaba, overseeing the entire process from concept to implementation for products like smart cockpits, hybrid AI service desks, and warehouse video intelligent inspection systems, while also promoting technological innovation and social inclusion.
            </p>
            <div class="grid grid-cols-3 gap-6 mb-8">
              <div class="p-4 bg-white rounded-lg shadow-sm">
                <h3 class="font-semibold text-gray-900 mb-2">Product Planning</h3>
                <p class="text-gray-600">Led key projects from concept to launch</p>
              </div>
              <div class="p-4 bg-white rounded-lg shadow-sm">
                <h3 class="font-semibold text-gray-900 mb-2">Team Management</h3>
                <p class="text-gray-600">Coordinated cross-functional teams for efficient delivery</p>
              </div>
              <div class="p-4 bg-white rounded-lg shadow-sm">
                <h3 class="font-semibold text-gray-900 mb-2">Patent Achievement</h3>
                <p class="text-gray-600">1 Patent Application (Pending)</p>
              </div>
            </div>
            <div class="flex space-x-4">
              <a href="#contact" class="inline-flex items-center px-6 py-3 !rounded-button bg-primary text-white font-medium hover:bg-primary/90 transition-colors whitespace-nowrap">
                Contact Me
                <i class="fas fa-arrow-right ml-2"></i>
              </a>
              <a href="#" class="inline-flex items-center px-6 py-3 !rounded-button border-2 border-primary text-primary font-medium hover:bg-primary/10 transition-colors whitespace-nowrap">
                Download Resume
                <i class="fas fa-download ml-2"></i>
              </a>
            </div>
          </div>
          <div class="w-full lg:w-2/5 mt-8 lg:mt-0">
            <img src="https://ai-public.mastergo.com/ai/img_res/54dc21182561c81cd129221642b12548.jpg" alt="Profile Photo" class="w-full h-auto rounded-lg shadow-lg">
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Experience Section -->
  <section id="experience" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="fade-in">
        <h2 class="text-3xl font-bold text-center text-gray-900 mb-16">Experience</h2>
        <div class="space-y-12">
          <!-- Alibaba Cloud - Banma Smart Cockpit Solutions Product Department -->
          <div class="timeline-item">
            <div class="bg-white p-6 rounded-lg shadow-sm">
              <h3 class="text-xl font-bold text-gray-900">Alibaba Cloud - Banma Smart Cockpit Solutions Product Department</h3>
              <p class="text-gray-600 mt-1">May 2021 - Oct 2023 | Shanghai</p>
              <div class="mt-4">
                <p class="text-gray-700 mb-4">Product Leader: Responsible for the planning and implementation of the in-vehicle interactive cloud application and intelligent voice assistant.</p>
                <ul class="list-disc list-inside text-gray-700 space-y-2">
                  <li><strong>In-Vehicle Citylife Service Cloud Application:</strong> Deployed on 200,000 in-vehicle devices with an average weekly active rate of 10%.</li>
                  <li><strong>In-Vehicle AI Voice Assistant:</strong> Developed for LS6 engineering vehicles and showcased at the Chengdu International Auto Show, supporting office assistance and traffic violation recognition.</li>
                </ul>
              </div>
            </div>
          </div>

          <!-- Alibaba Group - Taobao Consulting Product Department -->
          <div class="timeline-item">
            <div class="bg-white p-6 rounded-lg shadow-sm">
              <h3 class="text-xl font-bold text-gray-900">Alibaba Group - Taobao Consulting Product Department</h3>
              <p class="text-gray-600 mt-1">Sept 2018 - May 2021 | Hangzhou</p>
              <div class="mt-4">
                <p class="text-gray-700 mb-4">Product Leader: Oversaw the design and implementation of Taobao platform consulting services.</p>
                <ul class="list-disc list-inside text-gray-700 space-y-2">
                  <li><strong>Merchant Support Chatbot:</strong> Supported 20,000 daily conversations, with 80% resolved by AI.</li>
                  <li><strong>AI-Hybrid Service Desk:</strong> Served over 50 international enterprises, achieving product sales of over 21,000,000 RMB.</li>
                  <li><strong>Inclusive Product For Disabled:</strong> Created 110,000 job opportunities for disabled individuals, saving $2M per month.</li>
                </ul>
              </div>
            </div>
          </div>

          <!-- Alibaba Group - Logistics & After-Sales Product Department -->
          <div class="timeline-item">
            <div class="bg-white p-6 rounded-lg shadow-sm">
              <h3 class="text-xl font-bold text-gray-900">Alibaba Group - Logistics &amp; After-Sales Product Department</h3>
              <p class="text-gray-600 mt-1">Mar 2016 - Sept 2018 | Hangzhou</p>
              <div class="mt-4">
                <p class="text-gray-700 mb-4">Product Expert: Provided logistics and after-sales solutions for platform merchants.</p>
                <ul class="list-disc list-inside text-gray-700 space-y-2">
                  <li><strong>Warehouse Video Intelligent Inspection Solution:</strong> Sold 50,000 units, saving $24M annually, and filed a technology patent.</li>
                  <li><strong>Logistics Service AI Plugin:</strong> Integrated with ERP systems to send over 60,000 abnormal logistics alerts daily, reducing refund rates by 30%.</li>
                </ul>
              </div>
            </div>
          </div>

          <!-- Alibaba Group - Transaction Security Product Department -->
          <div class="timeline-item">
            <div class="bg-white p-6 rounded-lg shadow-sm">
              <h3 class="text-xl font-bold text-gray-900">Alibaba Group - Transaction Security Product Department</h3>
              <p class="text-gray-600 mt-1">Nov 2014 - Mar 2016 | Hangzhou</p>
              <div class="mt-4">
                <p class="text-gray-700 mb-4">Product Manager: Responsible for identifying high-risk transactions and providing VIP services.</p>
                <ul class="list-disc list-inside text-gray-700 space-y-2">
                  <li><strong>Risk Transaction Prevention Product:</strong> Detected an average of 1 million high-risk orders per month with a 20% automated processing rate.</li>
                  <li><strong>VIP Service Product:</strong> Provided dedicated account managers for the top 200 core merchants on the Alibaba platform.</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="py-20 bg-gray-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="fade-in">
        <h2 class="text-3xl font-bold text-center text-gray-900 mb-16">Projects</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- Smart Cockpit Solution -->
          <div class="bg-white rounded-lg shadow-sm overflow-hidden">
            <img src="https://ai-public.mastergo.com/ai/img_res/085b278baa197b2b4a14cc877a00327a.jpg" alt="Smart Cockpit Solution" class="w-full h-48 object-cover">
            <div class="p-6">
              <h3 class="text-xl font-bold text-gray-900 mb-2">Smart Cockpit Solution</h3>
              <p class="text-gray-700 mb-4">Combines visual perception and intelligent voice technology to automatically detect traffic violations and enable an in-vehicle office experience.</p>
              <button class="inline-flex items-center px-4 py-2 !rounded-button bg-primary text-white font-medium hover:bg-primary/90 transition-colors whitespace-nowrap">
                Learn More
                <i class="fas fa-arrow-right ml-2"></i>
              </button>
            </div>
          </div>

          <!-- Hybrid AI Service Desk -->
          <div class="bg-white rounded-lg shadow-sm overflow-hidden">
            <img src="https://ai-public.mastergo.com/ai/img_res/aa39b8747a86d2700c954da5a8db10c9.jpg" alt="Hybrid AI Service Desk" class="w-full h-48 object-cover">
            <div class="p-6">
              <h3 class="text-xl font-bold text-gray-900 mb-2">Hybrid AI Service Desk</h3>
              <p class="text-gray-700 mb-4">Utilizes a crowdsourcing model and RNN intent recognition algorithm to support 20,000 daily consultations, serving over 50 international enterprises and creating 110,000 job opportunities.</p>
              <button class="inline-flex items-center px-4 py-2 !rounded-button bg-primary text-white font-medium hover:bg-primary/90 transition-colors whitespace-nowrap">
                Learn More
                <i class="fas fa-arrow-right ml-2"></i>
              </button>
            </div>
          </div>

          <!-- Warehouse Video Intelligent Inspection -->
          <div class="bg-white rounded-lg shadow-sm overflow-hidden">
            <img src="https://ai-public.mastergo.com/ai/img_res/fefa8afbe8f1e4b2862e422a3d535d60.jpg" alt="Warehouse Video Intelligent Inspection" class="w-full h-48 object-cover">
            <div class="p-6">
              <h3 class="text-xl font-bold text-gray-900 mb-2">Warehouse Video Intelligent Inspection</h3>
              <p class="text-gray-700 mb-4">A computer vision-based intelligent inspection system for warehouses, successfully sold 50,000 units while saving $24M annually.</p>
              <button class="inline-flex items-center px-4 py-2 !rounded-button bg-primary text-white font-medium hover:bg-primary/90 transition-colors whitespace-nowrap">
                Learn More
                <i class="fas fa-arrow-right ml-2"></i>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Achievements & Patents Section -->
  <section id="achievements" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="fade-in">
        <h2 class="text-3xl font-bold text-center text-gray-900 mb-16">Achievements &amp; Patents</h2>
        <!-- Core Numbers -->
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 mb-16">
          <div class="text-center">
            <div class="text-4xl font-bold text-primary mb-2" data-count="21000000">0</div>
            <p class="text-gray-700">Product Sales (RMB)</p>
          </div>
          <div class="text-center">
            <div class="text-4xl font-bold text-primary mb-2" data-count="200000">0</div>
            <p class="text-gray-700">In-Vehicle Device Coverage</p>
          </div>
          <div class="text-center">
            <div class="text-4xl font-bold text-primary mb-2" data-count="110000">0</div>
            <p class="text-gray-700">Job Opportunities</p>
          </div>
          <div class="text-center">
            <div class="text-4xl font-bold text-primary mb-2" data-count="50000">0</div>
            <p class="text-gray-700">Warehouse Units Sold</p>
          </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
          <!-- Technical Patents -->
          <div class="bg-white p-6 rounded-lg shadow-sm">
            <h3 class="text-xl font-bold text-gray-900 mb-4">Technical Patents</h3>
            <ul class="space-y-4">
              <li class="flex items-start">
                <i class="fas fa-certificate text-primary mt-1 mr-3"></i>
                <div>
                  <h4 class="font-medium text-gray-900">Information Processing Method and Device &amp; Electronic Device</h4>
                  <p class="text-gray-600 text-sm">Patent No.: CN113327114A (Pending)</p>
                </div>
              </li>
            </ul>
          </div>
          <!-- Industry Impact -->
          <div class="bg-white p-6 rounded-lg shadow-sm">
            <h3 class="text-xl font-bold text-gray-900 mb-4">Industry Impact</h3>
            <ul class="space-y-4">
              <li class="flex items-start">
                <i class="fas fa-trophy text-primary mt-1 mr-3"></i>
                <div>
                  <h4 class="font-medium text-gray-900">200,000 In-Vehicle Device Coverage</h4>
                  <p class="text-gray-600">Smart cockpit cloud application deployed on 200,000 devices.</p>
                </div>
              </li>
              <li class="flex items-start">
                <i class="fas fa-trophy text-primary mt-1 mr-3"></i>
                <div>
                  <h4 class="font-medium text-gray-900">50+ International Enterprises Served</h4>
                  <p class="text-gray-600">Hybrid AI service desk efficiently supports over 50 international enterprises.</p>
                </div>
              </li>
              <li class="flex items-start">
                <i class="fas fa-trophy text-primary mt-1 mr-3"></i>
                <div>
                  <h4 class="font-medium text-gray-900">110,000 Job Opportunities</h4>
                  <p class="text-gray-600">Inclusive product created 110,000 employment opportunities for the disabled.</p>
                </div>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Education Section -->
  <section id="education" class="py-20 bg-gray-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="fade-in">
        <h2 class="text-3xl font-bold text-center text-gray-900 mb-16">Education</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
          <div class="bg-white p-6 rounded-lg shadow-sm">
            <div class="flex items-center mb-4">
              <i class="fas fa-graduation-cap text-3xl text-primary mr-4"></i>
              <div>
                <h3 class="text-xl font-bold text-gray-900">Zhejiang University of Technology</h3>
                <p class="text-gray-600">Master of Applied Economics</p>
                <p class="text-gray-500">Sep 2012 - Apr 2015</p>
              </div>
            </div>
          </div>
          <div class="bg-white p-6 rounded-lg shadow-sm">
            <div class="flex items-center mb-4">
              <i class="fas fa-graduation-cap text-3xl text-primary mr-4"></i>
              <div>
                <h3 class="text-xl font-bold text-gray-900">Zhejiang University of Technology Zhijiang College</h3>
                <p class="text-gray-600">Bachelor’s Degree in International Economics and Trade</p>
                <p class="text-gray-500">Sep 2008 - Sep 2012</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="fade-in">
        <h2 class="text-3xl font-bold text-center text-gray-900 mb-16">Contact</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div class="text-center">
            <div class="w-16 h-16 mx-auto bg-primary/10 rounded-full flex items-center justify-center mb-4">
              <i class="fas fa-envelope text-2xl text-primary"></i>
            </div>
            <h3 class="text-lg font-medium text-gray-900 mb-2">Email</h3>
            <p class="text-gray-700">jaysean.qian@gmail.com</p>
          </div>
          <div class="text-center">
            <div class="w-16 h-16 mx-auto bg-primary/10 rounded-full flex items-center justify-center mb-4">
              <i class="fas fa-phone text-2xl text-primary"></i>
            </div>
            <h3 class="text-lg font-medium text-gray-900 mb-2">Phone</h3>
            <p class="text-gray-700">+86-159-8817-1024</p>
          </div>
          <div class="text-center">
            <div class="w-16 h-16 mx-auto bg-primary/10 rounded-full flex items-center justify-center mb-4">
              <i class="fab fa-linkedin text-2xl text-primary"></i>
            </div>
            <h3 class="text-lg font-medium text-gray-900 mb-2">LinkedIn</h3>
            <a href="#" class="text-primary hover:text-primary/90">View Profile</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-900 text-white py-12">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div>
          <span class="text-2xl font-['Pacifico'] text-white mb-4 block">Sui Qian</span>
          <p class="text-gray-400">Senior Internet Product Manager | AI &amp; IoT Expert</p>
        </div>
        <div class="text-center">
          <h3 class="text-lg font-medium mb-4">Quick Links</h3>
          <ul class="space-y-2">
            <li><a href="#about" class="text-gray-400 hover:text-white">About Me</a></li>
            <li><a href="#experience" class="text-gray-400 hover:text-white">Experience</a></li>
            <li><a href="#projects" class="text-gray-400 hover:text-white">Projects</a></li>
          </ul>
        </div>
        <div class="text-right">
          <h3 class="text-lg font-medium mb-4">Contact</h3>
          <ul class="space-y-2">
            <li class="text-gray-400">Email: jaysean.qian@gmail.com</li>
            <li class="text-gray-400">Phone: +86-159-8817-1024</li>
            <li class="text-gray-400">Address: Chaoyang District, Beijing</li>
          </ul>
        </div>
      </div>
      <div class="mt-8 pt-8 border-t border-gray-800 text-center">
        <p class="text-gray-400">&copy; 2024 Personal Resume Website. All rights reserved.</p>
      </div>
    </div>
  </footer>

  <script>
    document.addEventListener('DOMContentLoaded', function() {
      const fadeElements = document.querySelectorAll('.fade-in');
      const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.classList.add('visible');
          }
        });
      });

      fadeElements.forEach(element => {
        observer.observe(element);
      });

      const countElements = document.querySelectorAll('[data-count]');
      countElements.forEach(element => {
        const target = parseInt(element.getAttribute('data-count'));
        const duration = 2000;
        const step = target / (duration / 16);
        let current = 0;

        const updateCount = () => {
          current += step;
          if (current < target) {
            element.textContent = Math.floor(current).toLocaleString();
            requestAnimationFrame(updateCount);
          } else {
            element.textContent = target.toLocaleString();
          }
        };

        const countObserver = new IntersectionObserver((entries) => {
          entries.forEach(entry => {
            if (entry.isIntersecting) {
              updateCount();
              countObserver.unobserve(entry.target);
            }
          });
        });

        countObserver.observe(element);
      });
    });
  </script>
</body>
</html>

