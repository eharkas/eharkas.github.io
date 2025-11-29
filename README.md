<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ZoomTutors Content</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    body {
      font-family: 'Inter', sans-serif;
      line-height: 1.6;
      scroll-behavior: smooth;
      background-color: #f8fafc;
      margin: 0;
      overflow-x: hidden;
    }

    /* --- Color Utilities --- */
    .bg-zt-orange { background-color: #F97316; }
    .text-zt-orange { color: #F97316; }

    /* --- Button Styles --- */
    .btn-enhanced-primary {
      display: inline-flex; align-items: center; justify-content: center;
      font-weight: 600; padding: 0.8rem 2rem; border-radius: 0.75rem;
      background: linear-gradient(135deg, #F97316, #fb923c); color: white;
      box-shadow: 0 8px 25px rgba(249, 115, 22, 0.4);
      transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1); cursor: pointer; text-decoration: none;
    }
    .btn-enhanced-primary:hover { 
      background: linear-gradient(135deg, #EA580C, #f97316); 
      transform: scale(1.02) translateY(-2px);
    }

    /* --- Cards --- */
    .card {
      border-radius: 1rem; background: white;
      box-shadow: 0 4px 20px rgba(0,0,0,0.06);
      transition: all 0.3s ease; border: 1px solid #f1f5f9;
    }
    .card:hover { transform: translateY(-8px); box-shadow: 0 15px 30px rgba(0,0,0,0.1); }

    /* --- Hero Background --- */
    .hero-bg-image {
      position: relative;
      background-image: url('https://images.unsplash.com/photo-1523240795612-9a054b0db644?q=80&w=2070&auto=format&fit=crop');
      background-size: cover; background-position: center;
    }
    .hero-overlay {
      position: absolute; inset: 0;
      background: linear-gradient(135deg, rgba(30, 41, 59, 0.8), rgba(249, 115, 22, 0.3));
      z-index: 0;
    }
    .hero-content { position: relative; z-index: 1; }
  </style>
</head>
<body>

  <section id="hero" class="hero-bg-image py-24 md:py-32 flex items-center justify-center">
    <div class="hero-overlay"></div>
    <div class="hero-content container mx-auto px-4 text-center">
      <div class="inline-block mb-6 px-4 py-1.5 rounded-full bg-orange-500/20 border border-orange-400/30 backdrop-blur-md">
        <span class="text-orange-100 font-bold text-sm tracking-wide uppercase">🚀 Non-Profit & 100% Free</span>
      </div>
      
      <h1 class="text-4xl sm:text-5xl md:text-6xl font-extrabold text-white mb-6 leading-tight drop-shadow-lg">
        Master Your Classes with <br />
        <span class="text-transparent bg-clip-text bg-gradient-to-r from-orange-200 to-orange-400">Expert Peer Tutors</span>
      </h1>
      
      <p class="text-lg sm:text-xl text-gray-100 mb-10 max-w-2xl mx-auto font-medium leading-relaxed">
        Connect with high-achieving students who aced the exact AP, IB, and Dual Enrollment courses you are taking now.
      </p>
      
      <div class="flex justify-center">
        <a href="https://docs.google.com/forms/d/e/1FAIpQLScie_Nlqbt3ldEomHnsrVzbJJ42-zYavDdfC9PO70ve80CRTQ/viewform"
           target="_blank" class="btn-enhanced-primary text-xl">
           Book a Free Session
        </a>
      </div>
    </div>
  </section>

  <div class="bg-white border-b border-gray-100 relative z-20 mx-auto max-w-5xl -mt-8 rounded-xl shadow-xl flex flex-col md:flex-row justify-around py-6 px-4 text-center">
    <div class="mb-4 md:mb-0">
      <div class="text-3xl font-bold text-gray-900">100%</div>
      <div class="text-sm text-gray-500 font-bold uppercase">Free</div>
    </div>
    <div class="hidden md:block w-px bg-gray-200"></div>
    <div class="mb-4 md:mb-0">
      <div class="text-3xl font-bold text-gray-900">Top 10%</div>
      <div class="text-sm text-gray-500 font-bold uppercase">Tutor Scores</div>
    </div>
    <div class="hidden md:block w-px bg-gray-200"></div>
    <div>
      <div class="text-3xl font-bold text-zt-orange" id="hours-counter-banner">...</div>
      <div class="text-sm text-gray-500 font-bold uppercase">Hours Tutored</div>
    </div>
  </div>

  <section class="py-20 container mx-auto px-6">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-extrabold text-gray-900 mb-4">Why ZoomTutors?</h2>
      <p class="text-gray-600 max-w-2xl mx-auto">We bridge the gap between struggling in class and excelling on exams.</p>
    </div>
    <div class="grid sm:grid-cols-3 gap-8">
      <div class="card p-8 text-center group border-t-4 border-zt-orange">
        <div class="text-4xl text-zt-orange mb-4 group-hover:scale-110 transition-transform"><i class="fas fa-wallet"></i></div>
        <h3 class="text-xl font-bold mb-2">Always Free</h3>
        <p class="text-gray-600 text-sm">Professional tutoring costs $50+/hr. We provide the same quality for $0.</p>
      </div>
      <div class="card p-8 text-center group border-t-4 border-blue-500">
        <div class="text-4xl text-blue-500 mb-4 group-hover:scale-110 transition-transform"><i class="fas fa-user-graduate"></i></div>
        <h3 class="text-xl font-bold mb-2">Relatable Peers</h3>
        <p class="text-gray-600 text-sm">Learn from students who just took the same class and understand the struggle.</p>
      </div>
      <div class="card p-8 text-center group border-t-4 border-zt-orange">
        <div class="text-4xl text-zt-orange mb-4 group-hover:scale-110 transition-transform"><i class="fas fa-medal"></i></div>
        <h3 class="text-xl font-bold mb-2">Top Talent</h3>
        <p class="text-gray-600 text-sm">Our tutors have above the 80th percentile in SAT/ACT or PSAT. With a average of 90th precentile  </p>
      </div>
    </div>
  </section>

  <section class="py-16 bg-slate-100">
    <div class="container mx-auto px-6 text-center">
      <h2 class="text-3xl font-bold mb-10">Courses We Cover</h2>
      <div class="grid grid-cols-2 md:grid-cols-4 gap-4 text-left">
        <div class="bg-white p-5 rounded-lg shadow-sm"><span class="font-bold text-zt-orange block mb-1">AP Math</span>Calculus AB/BC, Stats</div>
        <div class="bg-white p-5 rounded-lg shadow-sm"><span class="font-bold text-blue-600 block mb-1">AP Science</span>Bio, Chem, Envio</div>
        <div class="bg-white p-5 rounded-lg shadow-sm"><span class="font-bold text-zt-orange block mb-1">History</span>APUSH, World, Gov</div>
        <div class="bg-white p-5 rounded-lg shadow-sm"><span class="font-bold text-blue-600 block mb-1">College</span>SAT, ACT, Essays</div>
      </div>
      <div class="mt-10">
        <a href="https://docs.google.com/forms/d/e/1FAIpQLScie_Nlqbt3ldEomHnsrVzbJJ42-zYavDdfC9PO70ve80CRTQ/viewform" target="_blank" class="text-zt-orange font-bold hover:underline">
          See full course list in sign-up form &rarr;
        </a>
      </div>
    </div>
  </section>

  <section class="py-20 bg-white">
    <div class="container mx-auto px-6 text-center">
      <h2 class="text-3xl font-extrabold mb-12">Get Started in 3 Steps</h2>
      <div class="grid md:grid-cols-3 gap-8">
        <div>
          <div class="w-16 h-16 bg-orange-100 text-zt-orange rounded-full flex items-center justify-center text-2xl font-bold mx-auto mb-4">1</div>
          <h3 class="font-bold text-lg">Sign Up</h3>
          <p class="text-sm text-gray-600 mt-2">Fill out the Google Form.</p>
        </div>
        <div>
          <div class="w-16 h-16 bg-blue-100 text-blue-600 rounded-full flex items-center justify-center text-2xl font-bold mx-auto mb-4">2</div>
          <h3 class="font-bold text-lg">Get Matched</h3>
          <p class="text-sm text-gray-600 mt-2">We pair you with an expert.</p>
        </div>
        <div>
          <div class="w-16 h-16 bg-orange-100 text-zt-orange rounded-full flex items-center justify-center text-2xl font-bold mx-auto mb-4">3</div>
          <h3 class="font-bold text-lg">Zoom</h3>
          <p class="text-sm text-gray-600 mt-2">Join the link and learn!</p>
        </div>
      </div>
    </div>
  </section>

  <section id="connect" class="py-20 bg-gray-50">
    <div class="container mx-auto px-6">
      <h2 class="text-3xl md:text-4xl font-extrabold text-center text-gray-900 mb-4">Join The Community</h2>
      <p class="text-center text-gray-600 mb-12 max-w-2xl mx-auto">Click a box below to connect with us on your favorite platform.</p>
      
      <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
        
        <a href="https://teams.live.com/" target="_blank" class="group block bg-white border border-gray-200 p-8 rounded-2xl shadow-sm hover:shadow-xl hover:-translate-y-2 transition-all duration-300 text-center relative overflow-hidden">
          <div class="absolute inset-0 bg-blue-600 opacity-0 group-hover:opacity-5 transition-opacity duration-300"></div>
          <div class="text-5xl text-blue-600 mb-4 group-hover:scale-110 transition-transform duration-300"><i class="fab fa-microsoft"></i></div>
          <h3 class="text-xl font-bold text-gray-800 mb-1">Teams</h3>
          <span class="text-sm font-semibold text-blue-600 group-hover:underline">Join Meeting &rarr;</span>
        </a>

        <a href="https://chat.whatsapp.com/GPhe2MXL51xA37ARf0wiGB" target="_blank" class="group block bg-white border border-gray-200 p-8 rounded-2xl shadow-sm hover:shadow-xl hover:-translate-y-2 transition-all duration-300 text-center relative overflow-hidden">
          <div class="absolute inset-0 bg-green-500 opacity-0 group-hover:opacity-5 transition-opacity duration-300"></div>
          <div class="text-5xl text-green-500 mb-4 group-hover:scale-110 transition-transform duration-300"><i class="fab fa-whatsapp"></i></div>
          <h3 class="text-xl font-bold text-gray-800 mb-1">WhatsApp</h3>
          <span class="text-sm font-semibold text-green-600 group-hover:underline">Join Group &rarr;</span>
        </a>

        <a href="https://discord.gg/MMsmbGD4nG" target="_blank" class="group block bg-white border border-gray-200 p-8 rounded-2xl shadow-sm hover:shadow-xl hover:-translate-y-2 transition-all duration-300 text-center relative overflow-hidden">
          <div class="absolute inset-0 bg-indigo-500 opacity-0 group-hover:opacity-5 transition-opacity duration-300"></div>
          <div class="text-5xl text-indigo-500 mb-4 group-hover:scale-110 transition-transform duration-300"><i class="fab fa-discord"></i></div>
          <h3 class="text-xl font-bold text-gray-800 mb-1">Discord</h3>
          <span class="text-sm font-semibold text-indigo-600 group-hover:underline">Join Server &rarr;</span>
        </a>

        <a href="https://www.instagram.com/zoomtutors_broward" target="_blank" class="group block bg-white border border-gray-200 p-8 rounded-2xl shadow-sm hover:shadow-xl hover:-translate-y-2 transition-all duration-300 text-center relative overflow-hidden">
          <div class="absolute inset-0 bg-pink-500 opacity-0 group-hover:opacity-5 transition-opacity duration-300"></div>
          <div class="text-5xl text-pink-600 mb-4 group-hover:scale-110 transition-transform duration-300"><i class="fab fa-instagram"></i></div>
          <h3 class="text-xl font-bold text-gray-800 mb-1">Instagram</h3>
          <span class="text-sm font-semibold text-pink-600 group-hover:underline">Follow Us &rarr;</span>
        </a>

      </div>
      
      <div class="mt-6 text-center">
        <a href="https://docs.google.com/forms/d/e/1FAIpQLSd7gfbI8o0HqMoX3LZnlhaDu7W9eR9X4DM4A9fsA7JiAVj9rA/viewform" target="_blank" class="inline-block px-8 py-3 bg-white border border-gray-300 rounded-full font-semibold text-gray-600 hover:bg-gray-50 hover:text-zt-orange transition-colors shadow-sm">
          <i class="fas fa-comment-dots mr-2"></i> Give Feedback / Contact Us
        </a>
      </div>
    </div>
  </section>

  <footer class="bg-gray-900 text-white py-8 text-center">
    <p class="text-gray-500 text-sm">&copy; 2025 ZoomTutors. All rights reserved.</p>
  </footer>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    // Counter Logic
    const baseHours = 250; 
    const weeklyHours = 15; 
    const startDate = new Date('2025-11-09T00:00:00');

    function calculateTotalHours() {
      let totalHours = baseHours;
      const today = new Date(); today.setHours(0, 0, 0, 0);
      let currentDate = new Date(startDate.getTime()); currentDate.setHours(0, 0, 0, 0);
      const msPerWeek = 7 * 24 * 60 * 60 * 1000;
      const weeks = Math.floor((today - currentDate) / msPerWeek);
      if (weeks > 0) totalHours += weeklyHours * weeks;
      return totalHours;
    }

    function animateCounter(targetValue) {
      const el = document.getElementById('hours-counter-banner');
      if (!el) return;
      const duration = 2000; let startTimestamp = null; const startValue = 100;
      
      const step = (timestamp) => {
        if (!startTimestamp) startTimestamp = timestamp;
        const progress = Math.min((timestamp - startTimestamp) / duration, 1);
        const currentValue = Math.floor(progress * (targetValue - startValue) + startValue);
        el.textContent = currentValue.toLocaleString() + "+";
        if (progress < 1) window.requestAnimationFrame(step);
      };
      window.requestAnimationFrame(step);
    }
    animateCounter(calculateTotalHours());
  });
</script>
</body>
</html>
