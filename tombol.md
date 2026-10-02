<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TD Indo - Topup Diamond Game Terbaik & Terpercaya di Indonesia</title>
  
  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              dark: '#0a0f12',
              card: '#121a21',
              cardHover: '#18242e',
              cyan: '#00f2fe',
              cyanDark: '#00b8d4',
              accent: '#4facfe',
            }
          }
        }
      }
    }
  </script>

  <style>
    body {
      background-color: #070b0e;
      color: #e2e8f0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    .neon-text {
      text-shadow: 0 0 10px rgba(0, 242, 254, 0.5);
    }
    .card-border {
      border: 1px solid rgba(0, 242, 254, 0.15);
    }
    .card-border:hover {
      border-color: rgba(0, 242, 254, 0.6);
      transform: translateY(-2px);
    }
    .active-nav {
      color: #00f2fe !important;
      border-bottom: 2px solid #00f2fe;
    }
    ::-webkit-scrollbar {
      width: 8px;
    }
    ::-webkit-scrollbar-track {
      background: #070b0e;
    }
    ::-webkit-scrollbar-thumb {
      background: #18242e;
      border-radius: 4px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: #00f2fe;
    }
  </style>
</head>
<body class="min-h-screen flex flex-col justify-between selection:bg-cyan-500 selection:text-black">

  <!-- HEADER / NAVBAR -->
  <header class="bg-[#0b1217]/90 backdrop-blur-md sticky top-0 z-50 border-b border-cyan-900/30">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between gap-4">
      
      <!-- LOGO -->
      <a href="javascript:void(0)" onclick="navigateTo('home')" class="flex items-center gap-3 group">
        <div class="relative w-12 h-12 flex items-center justify-center bg-gradient-to-br from-cyan-400 to-blue-600 rounded-xl shadow-lg group-hover:scale-105 transition">
          <i class="fa-solid fa-gem text-white text-2xl"></i>
        </div>
        <div class="flex flex-col">
          <span class="text-2xl font-black italic tracking-wider text-white flex items-center">
            TD <span class="text-cyan-400 ml-1">Indo</span>
          </span>
          <span class="text-[10px] tracking-widest text-gray-400 -mt-1 font-semibold">TOPUP GAME STORE</span>
        </div>
      </a>

      <!-- SEARCH BAR -->
      <div class="hidden md:flex flex-1 max-w-md mx-6 relative">
        <input 
          type="text" 
          id="searchInput"
          placeholder="Cari Game..." 
          onkeyup="filterGames()"
          class="w-full bg-[#131d24] text-sm text-gray-200 placeholder-gray-500 rounded-full py-2.5 pl-11 pr-4 border border-cyan-900/40 focus:outline-none focus:border-cyan-400 transition"
        >
        <i class="fa-solid fa-magnifying-glass absolute left-4 top-3 text-gray-400"></i>
      </div>

      <!-- NAV MENU & LOGIN BUTTON -->
      <div class="flex items-center gap-6">
        <nav class="hidden lg:flex items-center gap-6 text-sm font-semibold text-gray-300">
          <a href="javascript:void(0)" id="nav-home" onclick="navigateTo('home')" class="active-nav pb-1 transition">BERANDA</a>
          <a href="javascript:void(0)" id="nav-games" onclick="navigateTo('games')" class="hover:text-cyan-400 pb-1 transition">GAME TERPOPULER</a>
          <a href="javascript:void(0)" id="nav-harga" onclick="navigateTo('harga')" class="hover:text-cyan-400 pb-1 transition">HARGA</a>
          <a href="javascript:void(0)" id="nav-layanan" onclick="navigateTo('layanan')" class="hover:text-cyan-400 pb-1 transition">LAYANAN</a>
          <a href="javascript:void(0)" id="nav-tentang" onclick="navigateTo('tentang')" class="hover:text-cyan-400 pb-1 transition">TENTANG KAMI</a>
          <a href="javascript:void(0)" id="nav-kontak" onclick="navigateTo('kontak')" class="hover:text-cyan-400 pb-1 transition">KONTAK</a>
        </nav>

        <button onclick="openAuthModal('login')" class="flex items-center gap-2 bg-gradient-to-r from-cyan-500 to-blue-600 hover:from-cyan-400 hover:to-blue-500 text-black font-bold text-xs uppercase px-5 py-2.5 rounded-full transition transform active:scale-95 shadow-md shadow-cyan-500/20">
          <i class="fa-solid fa-right-to-bracket"></i>
          <span>MASUK / DAFTAR</span>
        </button>
      </div>

    </div>
  </header>

  <!-- ================= HALAMAN 1: BERANDA ================= -->
  <div id="page-home" class="page-content">
    
    <!-- HERO SECTION -->
    <section class="relative py-12 md:py-16 overflow-hidden bg-gradient-to-b from-[#0e171e] via-[#091015] to-[#070b0e]">
      <div class="absolute inset-0 opacity-10 bg-[radial-gradient(#00f2fe_1px,transparent_1px)] [background-size:16px_16px]"></div>
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-96 h-96 bg-cyan-500/10 rounded-full blur-3xl pointer-events-none"></div>

      <div class="max-w-6xl mx-auto px-4 relative z-10 text-center">
        <h1 class="text-3xl md:text-5xl font-extrabold text-white tracking-wide uppercase mb-4 neon-text">
          TOPUP DIAMOND GAME TERBAIK & TERPERCAYA DI INDONESIA!
        </h1>
        <p class="text-gray-300 text-sm md:text-base max-w-2xl mx-auto mb-10 leading-relaxed">
          Beli Diamond, UC, CP, Genesis Crystals dengan harga murah, proses instan, dan pembayaran lengkap!
        </p>

        <!-- FITUR KEUNGGULAN -->
        <div class="grid grid-cols-2 md:grid-cols-4 gap-4 max-w-4xl mx-auto">
          <div class="bg-[#121c24]/80 backdrop-blur border border-cyan-500/20 rounded-xl p-3 flex items-center justify-center gap-3">
            <div class="w-8 h-8 rounded-full bg-cyan-500/20 text-cyan-400 flex items-center justify-center font-bold text-sm">
              <i class="fa-solid fa-bolt"></i>
            </div>
            <span class="text-xs md:text-sm font-semibold text-gray-200">1. Proses Instan</span>
          </div>

          <div class="bg-[#121c24]/80 backdrop-blur border border-cyan-500/20 rounded-xl p-3 flex items-center justify-center gap-3">
            <div class="w-8 h-8 rounded-full bg-cyan-500/20 text-cyan-400 flex items-center justify-center font-bold text-sm">
              <i class="fa-solid fa-shield-halved"></i>
            </div>
            <span class="text-xs md:text-sm font-semibold text-gray-200">2. Murah & Resmi</span>
          </div>

          <div class="bg-[#121c24]/80 backdrop-blur border border-cyan-500/20 rounded-xl p-3 flex items-center justify-center gap-3">
            <div class="w-8 h-8 rounded-full bg-cyan-500/20 text-cyan-400 flex items-center justify-center font-bold text-sm">
              <i class="fa-solid fa-gift"></i>
            </div>
            <span class="text-xs md:text-sm font-semibold text-gray-200">3. Banyak Bonus</span>
          </div>

          <div class="bg-[#121c24]/80 backdrop-blur border border-cyan-500/20 rounded-xl p-3 flex items-center justify-center gap-3">
            <div class="w-8 h-8 rounded-full bg-cyan-500/20 text-cyan-400 flex items-center justify-center font-bold text-sm">
              <i class="fa-solid fa-headset"></i>
            </div>
            <span class="text-xs md:text-sm font-semibold text-gray-200">4. Dukungan 24/7</span>
          </div>
        </div>
      </div>
    </section>

    <!-- DAFTAR GAME UTAMA -->
    <main class="max-w-6xl mx-auto px-4 py-10 flex-grow w-full">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6" id="gameGrid">

        <!-- GAME 1: MOBILE LEGENDS -->
        <div class="game-card bg-[#121a21] rounded-2xl p-4 card-border transition duration-300 relative group flex flex-col justify-between">
          <span class="absolute top-3 left-3 bg-cyan-950 text-cyan-400 text-xs font-bold px-2.5 py-1 rounded-md border border-cyan-800">1</span>
          <div class="flex items-center gap-4 mb-4 mt-2">
            <div class="w-20 h-20 rounded-xl bg-gradient-to-br from-blue-600 to-indigo-900 p-1 flex-shrink-0 shadow-md">
              <div class="w-full h-full bg-[#18242e] rounded-lg flex items-center justify-center overflow-hidden">
                <i class="fa-solid fa-gem text-3xl text-cyan-400"></i>
              </div>
            </div>
            <div>
              <h3 class="text-white font-extrabold text-base tracking-wide">MOBILE LEGENDS</h3>
              <p class="text-gray-400 text-xs mt-1">Diamond MLBB</p>
              <p class="text-cyan-400 text-xs font-semibold mt-0.5">10 - 10,000 D</p>
              <p class="text-white font-bold text-xs mt-1">Mulai Rp 1.500</p>
            </div>
          </div>
          <button onclick="openCheckout('Mobile Legends', 'Diamond MLBB', '10 - 10,000 D')" class="w-full bg-cyan-400 hover:bg-cyan-300 text-black font-extrabold text-xs uppercase py-2.5 rounded-lg transition transform active:scale-95 shadow-md shadow-cyan-400/20">
            BELI SEKARANG
          </button>
        </div>

        <!-- GAME 2: PUBG MOBILE -->
        <div class="game-card bg-[#121a21] rounded-2xl p-4 card-border transition duration-300 relative group flex flex-col justify-between">
          <span class="absolute top-3 left-3 bg-cyan-950 text-cyan-400 text-xs font-bold px-2.5 py-1 rounded-md border border-cyan-800">2</span>
          <div class="flex items-center gap-4 mb-4 mt-2">
            <div class="w-20 h-20 rounded-xl bg-gradient-to-br from-amber-500 to-amber-700 p-1 flex-shrink-0 shadow-md">
              <div class="w-full h-full bg-[#18242e] rounded-lg flex items-center justify-center font-black text-amber-400 text-xl tracking-wider">
                UC
              </div>
            </div>
            <div>
              <h3 class="text-white font-extrabold text-base tracking-wide">PUBG MOBILE</h3>
              <p class="text-gray-400 text-xs mt-1">UC PUBG</p>
              <p class="text-cyan-400 text-xs font-semibold mt-0.5">60 - 10,000 UC</p>
              <p class="text-white font-bold text-xs mt-1">Mulai Rp 3.000</p>
            </div>
          </div>
          <button onclick="openCheckout('PUBG Mobile', 'UC PUBG', '60 - 10,000 UC')" class="w-full bg-cyan-400 hover:bg-cyan-300 text-black font-extrabold text-xs uppercase py-2.5 rounded-lg transition transform active:scale-95 shadow-md shadow-cyan-400/20">
            BELI SEKARANG
          </button>
        </div>

        <!-- GAME 3: GENSHIN IMPACT -->
        <div class="game-card bg-[#121a21] rounded-2xl p-4 card-border transition duration-300 relative group flex flex-col justify-between">
          <span class="absolute top-3 left-3 bg-cyan-950 text-cyan-400 text-xs font-bold px-2.5 py-1 rounded-md border border-cyan-800">4</span>
          <div class="flex items-center gap-4 mb-4 mt-2">
            <div class="w-20 h-20 rounded-xl bg-gradient-to-br from-cyan-400 to-sky-700 p-1 flex-shrink-0 shadow-md">
              <div class="w-full h-full bg-[#18242e] rounded-lg flex items-center justify-center">
                <i class="fa-solid fa-wand-magic-sparkles text-3xl text-sky-300"></i>
              </div>
            </div>
            <div>
              <h3 class="text-white font-extrabold text-base tracking-wide">GENSHIN IMPACT</h3>
              <p class="text-gray-400 text-xs mt-1">Genshin Crystals</p>
              <p class="text-cyan-400 text-xs font-semibold mt-0.5">60 - 6,480 GC</p>
              <p class="text-white font-bold text-xs mt-1">Mulai Rp 12.000</p>
            </div>
          </div>
          <button onclick="openCheckout('Genshin Impact', 'Genesis Crystals', '60 - 6,480 GC')" class="w-full bg-cyan-400 hover:bg-cyan-300 text-black font-extrabold text-xs uppercase py-2.5 rounded-lg transition transform active:scale-95 shadow-md shadow-cyan-400/20">
            BELI SEKARANG
          </button>
        </div>

        <!-- GAME 4: CALL OF DUTY MOBILE -->
        <div class="game-card bg-[#121a21] rounded-2xl p-4 card-border transition duration-300 relative group flex flex-col justify-between">
          <span class="absolute top-3 left-3 bg-cyan-950 text-cyan-400 text-xs font-bold px-2.5 py-1 rounded-md border border-cyan-800">5</span>
          <div class="flex items-center gap-4 mb-4 mt-2">
            <div class="w-20 h-20 rounded-xl bg-gradient-to-br from-yellow-600 to-amber-900 p-1 flex-shrink-0 shadow-md">
              <div class="w-full h-full bg-[#18242e] rounded-lg flex items-center justify-center font-black text-yellow-500 text-xl">
                CP
              </div>
            </div>
            <div>
              <h3 class="text-white font-extrabold text-base tracking-wide">CALL OF DUTY MOBILE</h3>
              <p class="text-gray-400 text-xs mt-1">CP CODM</p>
              <p class="text-cyan-400 text-xs font-semibold mt-0.5">80 - 8,000 CP</p>
              <p class="text-white font-bold text-xs mt-1">Mulai Rp 5.000</p>
            </div>
          </div>
          <button onclick="openCheckout('Call of Duty Mobile', 'CP CODM', '80 - 8,000 CP')" class="w-full bg-cyan-400 hover:bg-cyan-300 text-black font-extrabold text-xs uppercase py-2.5 rounded-lg transition transform active:scale-95 shadow-md shadow-cyan-400/20">
            BELI SEKARANG
          </button>
        </div>

        <!-- GAME 5: ARENA OF VALOR -->
        <div class="game-card bg-[#121a21] rounded-2xl p-4 card-border transition duration-300 relative group flex flex-col justify-between">
          <span class="absolute top-3 left-3 bg-cyan-950 text-cyan-400 text-xs font-bold px-2.5 py-1 rounded-md border border-cyan-800">6</span>
          <div class="flex items-center gap-4 mb-4 mt-2">
            <div class="w-20 h-20 rounded-xl bg-gradient-to-br from-purple-600 to-blue-900 p-1 flex-shrink-0 shadow-md">
              <div class="w-full h-full bg-[#18242e] rounded-lg flex items-center justify-center">
                <i class="fa-solid fa-shield text-3xl text-purple-400"></i>
              </div>
            </div>
            <div>
              <h3 class="text-white font-extrabold text-base tracking-wide">ARENA OF VALOR</h3>
              <p class="text-gray-400 text-xs mt-1">AOV Vouchers</p>
              <p class="text-cyan-400 text-xs font-semibold mt-0.5">10 - 5,000 V</p>
              <p class="text-white font-bold text-xs mt-1">Mulai Rp 2.000</p>
            </div>
          </div>
          <button onclick="openCheckout('Arena of Valor', 'AOV Vouchers', '10 - 5,000 V')" class="w-full bg-cyan-400 hover:bg-cyan-300 text-black font-extrabold text-xs uppercase py-2.5 rounded-lg transition transform active:scale-95 shadow-md shadow-cyan-400/20">
            BELI SEKARANG
          </button>
        </div>

        <!-- GAME 6: VALORANT -->
        <div class="game-card bg-[#121a21] rounded-2xl p-4 card-border transition duration-300 relative group flex flex-col justify-between">
          <span class="absolute top-3 left-3 bg-cyan-950 text-cyan-400 text-xs font-bold px-2.5 py-1 rounded-md border border-cyan-800">7</span>
          <div class="flex items-center gap-4 mb-4 mt-2">
            <div class="w-20 h-20 rounded-xl bg-gradient-to-br from-red-500 to-rose-900 p-1 flex-shrink-0 shadow-md">
              <div class="w-full h-full bg-[#18242e] rounded-lg flex items-center justify-center">
                <i class="fa-solid fa-v text-3xl text-red-500 font-black"></i>
              </div>
            </div>
            <div>
              <h3 class="text-white font-extrabold text-base tracking-wide">VALORANT</h3>
              <p class="text-gray-400 text-xs mt-1">Valorant Points</p>
              <p class="text-cyan-400 text-xs font-semibold mt-0.5">100 - 10,000 VP</p>
              <p class="text-white font-bold text-xs mt-1">Mulai Rp 7.000</p>
            </div>
          </div>
          <button onclick="openCheckout('VALORANT', 'Valorant Points', '100 - 10,000 VP')" class="w-full bg-cyan-400 hover:bg-cyan-300 text-black font-extrabold text-xs uppercase py-2.5 rounded-lg transition transform active:scale-95 shadow-md shadow-cyan-400/20">
            BELI SEKARANG
          </button>
        </div>

      </div>
    </main>

    <!-- METODE PEMBAYARAN -->
    <section class="max-w-6xl mx-auto px-4 my-8 w-full">
      <div class="bg-[#121a21] border border-cyan-900/30 rounded-2xl p-6 text-center shadow-lg">
        <h3 class="text-white font-extrabold text-sm uppercase tracking-wider mb-4">
          PEMBAYARAN LENGKAP & AMAN!
        </h3>
        
        <div class="flex flex-wrap items-center justify-center gap-3">
          <div class="bg-[#008cff] text-white font-black italic px-4 py-2 rounded-lg text-xs shadow">DANA</div>
          <div class="bg-[#4c2a86] text-white font-black px-4 py-2 rounded-lg text-xs shadow">OVO</div>
          <div class="bg-[#00a5cf] text-white font-black px-4 py-2 rounded-lg text-xs shadow">gopay</div>
          <div class="bg-[#e1251b] text-white font-black px-4 py-2 rounded-lg text-xs shadow">LinkAja</div>
          <div class="bg-[#ee4d2d] text-white font-black px-4 py-2 rounded-lg text-xs shadow">ShopeePay</div>
          <div class="bg-[#00529c] text-white font-black px-4 py-2 rounded-lg text-xs shadow">BRI</div>
          <div class="bg-[#f15a24] text-white font-black px-4 py-2 rounded-lg text-xs shadow">BNI</div>
          <div class="bg-[#0060af] text-white font-black px-4 py-2 rounded-lg text-xs shadow">BCA</div>
          <div class="bg-[#002d62] text-amber-400 font-black px-4 py-2 rounded-lg text-xs shadow">mandırı</div>
        </div>
      </div>
    </section>
  </div>

  <!-- ================= HALAMAN 2: GAME TERPOPULER ================= -->
  <div id="page-games" class="page-content hidden max-w-6xl mx-auto px-4 py-12 w-full">
    <h2 class="text-2xl font-black text-white mb-2 uppercase tracking-wide flex items-center gap-2">
      <i class="fa-solid fa-fire text-cyan-400"></i> Semuanya Game Terpopuler
    </h2>
    <p class="text-gray-400 text-sm mb-8">Pilih game favoritmu dan nikmati penawaran diskon topup tercepat!</p>
    
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
      <div class="bg-[#121a21] border border-cyan-900/40 p-5 rounded-xl text-center">
        <i class="fa-solid fa-gem text-4xl text-cyan-400 mb-3"></i>
        <h3 class="text-white font-bold text-lg">Mobile Legends</h3>
        <p class="text-xs text-gray-400 my-2">Proses Kilat 1-3 Detik Lengkap dengan Bonus Diamond.</p>
        <button onclick="openCheckout('Mobile Legends', 'Diamond MLBB', '10 - 10,000 D')" class="mt-2 w-full bg-cyan-400 text-black font-bold py-2 rounded-lg text-xs">TOP UP NOW</button>
      </div>

      <div class="bg-[#121a21] border border-cyan-900/40 p-5 rounded-xl text-center">
        <i class="fa-solid fa-crosshairs text-4xl text-amber-400 mb-3"></i>
        <h3 class="text-white font-bold text-lg">PUBG Mobile</h3>
        <p class="text-xs text-gray-400 my-2">UC Murah Garansi Resmi Tencent Games.</p>
        <button onclick="openCheckout('PUBG Mobile', 'UC PUBG', '60 - 10,000 UC')" class="mt-2 w-full bg-cyan-400 text-black font-bold py-2 rounded-lg text-xs">TOP UP NOW</button>
      </div>

      <div class="bg-[#121a21] border border-cyan-900/40 p-5 rounded-xl text-center">
        <i class="fa-solid fa-star text-4xl text-sky-400 mb-3"></i>
        <h3 class="text-white font-bold text-lg">Genshin Impact</h3>
        <p class="text-xs text-gray-400 my-2">Blessing of the Welkin Moon & Genesis Crystals.</p>
        <button onclick="openCheckout('Genshin Impact', 'Genesis Crystals', '60 - 6,480 GC')" class="mt-2 w-full bg-cyan-400 text-black font-bold py-2 rounded-lg text-xs">TOP UP NOW</button>
      </div>
    </div>
  </div>

  <!-- ================= HALAMAN 3: DAFTAR HARGA ============
