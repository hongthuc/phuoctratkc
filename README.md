<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC | Cửa Nhôm Xingfa & Kính Cường Lực Đà Nẵng</title>
  <meta name="description" content="CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC (phuoctratkc.com) - Chuyên thi công cửa nhôm Xingfa, cửa kính cường lực, cầu thang kính, phòng tắm kính, kính ốp bếp tại Đà Nẵng. Hotline: 0905.811.246." />

  <!-- Open Graph / Thumbnail chia sẻ link sử dụng logo công ty (không hiển thị nút xem thumbnail trên trang) -->
  <meta property="og:type" content="website" />
  <meta property="og:site_name" content="CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC" />
  <meta property="og:title" content="PHƯỚC TRÀ TKC | Cửa Nhôm Xingfa & Kính Cường Lực Chính Hãng Đà Nẵng" />
  <meta property="og:description" content="Thi công cửa nhôm Xingfa nhập khẩu, cửa kính cường lực, cửa tự động, phòng tắm kính, kính ốp bếp tại Đà Nẵng. Địa chỉ: 365/12 Tôn Đản, Phường An Khê, TP Đà Nẵng. Hotline: 0905.811.246." />
  <meta property="og:url" content="https://phuoctratkc.com" />
  <meta property="og:image" content="https://phuoctratkc.com/wp-content/uploads/logo-phuoc-tra-tkc-thumbnail.png" />
  <meta property="og:image:width" content="1200" />
  <meta property="og:image:height" content="630" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="PHƯỚC TRÀ TKC | Cửa Nhôm Xingfa & Kính Cường Lực Đà Nẵng" />
  <meta name="twitter:image" content="https://phuoctratkc.com/wp-content/uploads/logo-phuoc-tra-tkc-thumbnail.png" />

  <!-- Google Fonts: Inter -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />

  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" />

  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'system-ui', '-apple-system', 'sans-serif'],
          },
          colors: {
            brand: {
              50: '#eef6fc',
              100: '#d8eaf8',
              600: '#12548e',
              700: '#0b3b66',
              800: '#082c4d',
              900: '#051e36',
            },
            accent: {
              400: '#f59e0b',
              500: '#d97706',
              600: '#b45309',
            }
          }
        }
      }
    };
  </script>

  <style>
    /* Đảm bảo bố cục luôn căn giữa, không tràn viền, không lệch sang phải trên mọi thiết bị */
    *, *::before, *::after {
      box-sizing: border-box;
    }
    html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      max-width: 100%;
      overflow-x: hidden;
      font-family: 'Inter', system-ui, -apple-system, sans-serif;
      scroll-behavior: smooth;
      background-color: #f8fafc;
      color: #0f172a;
    }

    /* Chiều ngang giao diện trên máy tính bằng 95% kích thước màn hình */
    .tkc-container {
      width: 96%;
      max-width: 96%;
      margin-left: auto;
      margin-right: auto;
    }
    @media (min-width: 1024px) {
      .tkc-container {
        width: 95%;
        max-width: 95%;
      }
    }

    /* Banner tự trượt sử dụng CSS Grid overlap để 2 slide luôn có kích thước cao bằng nhau tuyệt đối và không bị cắt chữ */
    .hero-grid-track {
      display: grid;
      grid-template-columns: 1fr;
    }
    .hero-slide {
      grid-area: 1 / 1;
      transition: opacity 0.65s ease, transform 0.65s ease, visibility 0.65s ease;
    }
    .hero-slide.is-active {
      opacity: 1;
      visibility: visible;
      transform: translateX(0);
      z-index: 2;
      pointer-events: auto;
    }
    .hero-slide.is-inactive {
      opacity: 0;
      visibility: hidden;
      transform: translateX(16px);
      z-index: 1;
      pointer-events: none;
    }

    /* Flatsome Dropdown Hover mượt mà cho máy tính */
    .nav-item-has-children:hover > .nav-dropdown {
      opacity: 1;
      visibility: visible;
      transform: translateY(0);
      pointer-events: auto;
    }
    .nav-dropdown {
      opacity: 0;
      visibility: hidden;
      transform: translateY(6px);
      transition: all 0.2s ease;
      pointer-events: none;
    }

    /* Hiệu ứng nhịp nhẹ cho nút liên hệ nổi */
    @keyframes tkcPulse {
      0% { box-shadow: 0 0 0 0 rgba(217, 119, 6, 0.55); }
      70% { box-shadow: 0 0 0 10px rgba(217, 119, 6, 0); }
      100% { box-shadow: 0 0 0 0 rgba(217, 119, 6, 0); }
    }
    .pulse-ring {
      animation: tkcPulse 2s infinite;
    }

    /* Thanh cuộn gọn nhẹ cho bảng báo giá trên điện thoại */
    .no-scrollbar::-webkit-scrollbar {
      display: none;
    }
    .no-scrollbar {
      -ms-overflow-style: none;
      scrollbar-width: none;
    }
  </style>
</head>
<body class="antialiased text-slate-800 bg-slate-50 pb-16 md:pb-0">

  <!-- ========================================================= -->
  <!-- PHẦN 1: TOP BAR THÔNG TIN (CHUẨN FLATSOME, KHÔNG CÓ THANH UXBUILDER) -->
  <!-- ========================================================= -->
  <div class="bg-brand-800 text-slate-100 text-[11px] sm:text-xs border-b border-brand-700/60">
    <div class="tkc-container py-1.5 flex flex-wrap items-center justify-between gap-2">
      <div class="flex items-center gap-3 sm:gap-5 min-w-0">
        <span class="flex items-center gap-1.5 truncate">
          <i class="fa-solid fa-location-dot text-accent-400 shrink-0"></i>
          <span class="truncate">365/12 Tôn Đản, Phường An Khê, TP Đà Nẵng</span>
        </span>
        <span class="hidden md:flex items-center gap-1.5 whitespace-nowrap">
          <i class="fa-solid fa-globe text-accent-400"></i>
          <span>phuoctratkc.com</span>
        </span>
      </div>
      <div class="flex items-center gap-3 sm:gap-4 shrink-0">
        <span class="hidden sm:inline-flex items-center gap-1.5 text-slate-200">
          <i class="fa-regular fa-clock text-accent-400"></i>
          <span>Làm việc: 07:30 - 18:00 (T2 - CN)</span>
        </span>
        <a href="tel:0905811246" class="inline-flex items-center gap-1.5 font-semibold text-accent-400 hover:text-amber-300 transition">
          <i class="fa-solid fa-phone-volume"></i>
          <span>0905.811.246</span>
        </a>
      </div>
    </div>
  </div>

  <!-- ========================================================= -->
  <!-- PHẦN 2: HEADER & MENU ĐIỀU HƯỚNG (LOGO GỌN NHỎ, 1 HÀNG TRÊN MÁY TÍNH, KHÔNG NÚT GỌI NGAY) -->
  <!-- ========================================================= -->
  <header class="sticky top-0 z-40 bg-white/95 backdrop-blur-md shadow-sm border-b border-slate-200 w-full">
    <div class="tkc-container py-2 sm:py-2.5 flex items-center justify-between gap-2 lg:gap-4">

      <!-- Logo Công Ty TNHH Đầu Tư Xây Dựng Phước Trà TKC (chỉnh gọn nhỏ chuyên nghiệp) -->
      <a href="#trang-chu" class="flex items-center gap-2 shrink-0 group focus:outline-none" aria-label="Phước Trà TKC Trang chủ">
        <svg class="w-9 h-9 sm:w-10 sm:h-10 shrink-0 transition-transform duration-200 group-hover:scale-105" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Logo Phước Trà TKC">
          <!-- Khung kiến trúc hiện đại -->
          <rect x="2" y="2" width="60" height="60" rx="12" fill="#0B3B66" />
          <rect x="5" y="5" width="54" height="54" rx="9" stroke="#F59E0B" stroke-opacity="0.35" stroke-width="1.5" />
          <!-- Biểu tượng mái & khung cửa nhôm kính -->
          <path d="M14 25L32 12L50 25" stroke="#F59E0B" stroke-width="3.2" stroke-linecap="round" stroke-linejoin="round" />
          <!-- Khung cửa đôi cách điệu chữ PT -->
          <rect x="17" y="27" width="13" height="23" rx="2" fill="#FFFFFF" />
          <rect x="20.5" y="31" width="6" height="7" rx="1" fill="#0B3B66" />
          <rect x="34" y="27" width="13" height="23" rx="2" fill="#F59E0B" />
          <rect x="37.5" y="31" width="6" height="15" rx="1" fill="#0B3B66" />
          <!-- Nền chân vững chắc -->
          <line x1="13" y1="52" x2="51" y2="52" stroke="#FFFFFF" stroke-width="2.4" stroke-linecap="round" />
        </svg>
        <div class="leading-tight">
          <div class="text-sm sm:text-[15px] font-extrabold tracking-tight text-brand-700 whitespace-nowrap">
            PHƯỚC TRÀ <span class="text-accent-500">TKC</span>
          </div>
          <div class="text-[9px] sm:text-[10px] font-semibold uppercase tracking-wider text-slate-500 whitespace-nowrap">
            Đầu Tư Xây Dựng • Nhôm Kính
          </div>
        </div>
      </a>

      <!-- Menu trên máy tính: Toàn bộ 9 danh mục viết liền trên 1 hàng chữ nhỏ gọn, tuyệt đối không xuống dòng -->
      <nav class="hidden lg:flex items-center justify-end flex-1 min-w-0" aria-label="Menu chính">
        <ul class="flex items-center justify-end gap-2 xl:gap-4 2xl:gap-5 list-none m-0 p-0">
          <li class="shrink-0">
            <a href="#trang-chu" class="block py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-brand-700 hover:text-accent-500 whitespace-nowrap transition border-b-2 border-accent-500">
              Trang chủ
            </a>
          </li>
          <li class="shrink-0">
            <a href="#gioi-thieu" class="block py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-slate-700 hover:text-brand-700 whitespace-nowrap transition border-b-2 border-transparent hover:border-accent-500">
              Giới thiệu
            </a>
          </li>

          <!-- Dropdown: Cửa nhôm xingfa -->
          <li class="relative shrink-0 nav-item-has-children">
            <a href="#san-pham" onclick="filterProducts('xingfa')" class="flex items-center gap-1 py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-slate-700 hover:text-brand-700 whitespace-nowrap transition border-b-2 border-transparent hover:border-accent-500">
              <span>Cửa nhôm xingfa</span>
              <i class="fa-solid fa-chevron-down text-[9px] text-slate-400"></i>
            </a>
            <ul class="nav-dropdown absolute left-0 top-full mt-0.5 w-56 bg-white rounded-xl shadow-xl border border-slate-200 py-1.5 z-50 list-none m-0">
              <li><a href="#san-pham" onclick="filterProducts('xingfa', '1 cánh')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhôm xingfa 1 cánh</a></li>
              <li><a href="#san-pham" onclick="filterProducts('xingfa', '2 cánh')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhôm xingfa 2 cánh</a></li>
              <li><a href="#san-pham" onclick="filterProducts('xingfa', '3 cánh')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhôm xingfa 3 cánh</a></li>
              <li><a href="#san-pham" onclick="filterProducts('xingfa', '4 cánh')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhôm xingfa 4 cánh</a></li>
              <li><a href="#san-pham" onclick="filterProducts('xingfa', 'xếp trượt')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhôm xingfa 5 cánh</a></li>
            </ul>
          </li>

          <li class="shrink-0">
            <a href="#san-pham" onclick="filterProducts('kinh-cuong-luc')" class="block py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-slate-700 hover:text-brand-700 whitespace-nowrap transition border-b-2 border-transparent hover:border-accent-500">
              Cửa kính cường lực
            </a>
          </li>

          <!-- Dropdown: Sản phẩm -->
          <li class="relative shrink-0 nav-item-has-children">
            <a href="#danh-muc-san-pham" class="flex items-center gap-1 py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-slate-700 hover:text-brand-700 whitespace-nowrap transition border-b-2 border-transparent hover:border-accent-500">
              <span>Sản phẩm</span>
              <i class="fa-solid fa-chevron-down text-[9px] text-slate-400"></i>
            </a>
            <ul class="nav-dropdown absolute left-0 top-full mt-0.5 w-52 bg-white rounded-xl shadow-xl border border-slate-200 py-1.5 z-50 list-none m-0">
              <li><a href="#san-pham" onclick="filterProducts('xingfa')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhôm xingfa</a></li>
              <li><a href="#san-pham" onclick="filterProducts('nhua-loi-thep')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhựa lõi thép</a></li>
              <li><a href="#san-pham" onclick="filterProducts('tu-dong')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa kính tự động</a></li>
              <li><a href="#san-pham" onclick="filterProducts('cau-thang-kinh')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cầu thang kính</a></li>
              <li><a href="#san-pham" onclick="filterProducts('kinh-op-bep')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Kính ốp bếp</a></li>
              <li><a href="#san-pham" onclick="filterProducts('phong-tam-kinh')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Phòng tắm kính</a></li>
            </ul>
          </li>

          <li class="shrink-0">
            <a href="#cong-trinh" class="block py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-slate-700 hover:text-brand-700 whitespace-nowrap transition border-b-2 border-transparent hover:border-accent-500">
              Công trình
            </a>
          </li>
          <li class="shrink-0">
            <a href="#bao-gia" class="block py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-slate-700 hover:text-brand-700 whitespace-nowrap transition border-b-2 border-transparent hover:border-accent-500">
              Báo giá
            </a>
          </li>
          <li class="shrink-0">
            <a href="#tin-tuc" class="block py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-slate-700 hover:text-brand-700 whitespace-nowrap transition border-b-2 border-transparent hover:border-accent-500">
              Tin tức
            </a>
          </li>
          <li class="shrink-0">
            <a href="#lien-he" class="block py-2 px-1 text-[11px] xl:text-[12.5px] font-bold uppercase tracking-tight text-slate-700 hover:text-brand-700 whitespace-nowrap transition border-b-2 border-transparent hover:border-accent-500">
              Liên hệ
            </a>
          </li>
        </ul>
      </nav>

      <!-- Nút mở menu trên điện thoại & máy tính bảng (không đặt nút Gọi Ngay trên header) -->
      <button id="mobileMenuBtn" type="button" class="lg:hidden inline-flex items-center justify-center w-10 h-10 rounded-lg border border-slate-200 text-brand-700 hover:bg-brand-50 transition shrink-0" aria-label="Mở danh mục menu">
        <i class="fa-solid fa-bars text-lg"></i>
      </button>
    </div>
  </header>

  <!-- ========================================================= -->
  <!-- DRAWER MENU CHO ĐIỆN THOẠI (FLATSOME OFF-CANVAS STYLE) -->
  <!-- ========================================================= -->
  <div id="mobileDrawerBackdrop" class="fixed inset-0 bg-slate-900/60 backdrop-blur-xs z-50 hidden opacity-0 transition-opacity duration-300" onclick="closeMobileMenu()"></div>
  <aside id="mobileDrawer" class="fixed top-0 left-0 h-full w-[84%] max-w-[320px] bg-white z-50 shadow-2xl transform -translate-x-full transition-transform duration-300 flex flex-col overflow-hidden" aria-label="Menu di động">
    <div class="flex items-center justify-between px-4 py-3 bg-brand-700 text-white">
      <div class="font-bold text-sm tracking-tight">DANH MỤC PHƯỚC TRÀ TKC</div>
      <button type="button" onclick="closeMobileMenu()" class="w-8 h-8 rounded-lg bg-white/15 hover:bg-white/25 flex items-center justify-center transition" aria-label="Đóng menu">
        <i class="fa-solid fa-xmark text-base"></i>
      </button>
    </div>

    <div class="flex-1 overflow-y-auto divide-y divide-slate-100">
      <a href="#trang-chu" onclick="closeMobileMenu()" class="block px-4 py-3 text-sm font-semibold text-brand-700 hover:bg-brand-50">Trang chủ</a>
      <a href="#gioi-thieu" onclick="closeMobileMenu()" class="block px-4 py-3 text-sm font-semibold text-slate-700 hover:bg-brand-50">Giới thiệu</a>

      <!-- Accordion: Cửa nhôm xingfa -->
      <div>
        <button type="button" onclick="toggleSubmenu('sub-xingfa', this)" class="w-full flex items-center justify-between px-4 py-3 text-sm font-semibold text-slate-700 hover:bg-brand-50">
          <span>Cửa nhôm xingfa</span>
          <i class="fa-solid fa-chevron-down text-xs text-slate-400 transition-transform duration-200"></i>
        </button>
        <div id="sub-xingfa" class="hidden bg-slate-50 pl-6 pr-4 py-1 space-y-0.5">
          <a href="#san-pham" onclick="filterProducts('xingfa', '1 cánh'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cửa nhôm xingfa 1 cánh</a>
          <a href="#san-pham" onclick="filterProducts('xingfa', '2 cánh'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cửa nhôm xingfa 2 cánh</a>
          <a href="#san-pham" onclick="filterProducts('xingfa', '3 cánh'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cửa nhôm xingfa 3 cánh</a>
          <a href="#san-pham" onclick="filterProducts('xingfa', '4 cánh'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cửa nhôm xingfa 4 cánh</a>
          <a href="#san-pham" onclick="filterProducts('xingfa', 'xếp trượt'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cửa nhôm xingfa 5 cánh</a>
        </div>
      </div>

      <a href="#san-pham" onclick="filterProducts('kinh-cuong-luc'); closeMobileMenu()" class="block px-4 py-3 text-sm font-semibold text-slate-700 hover:bg-brand-50">Cửa kính cường lực</a>

      <!-- Accordion: Sản phẩm -->
      <div>
        <button type="button" onclick="toggleSubmenu('sub-sanpham', this)" class="w-full flex items-center justify-between px-4 py-3 text-sm font-semibold text-slate-700 hover:bg-brand-50">
          <span>Sản phẩm</span>
          <i class="fa-solid fa-chevron-down text-xs text-slate-400 transition-transform duration-200"></i>
        </button>
        <div id="sub-sanpham" class="hidden bg-slate-50 pl-6 pr-4 py-1 space-y-0.5">
          <a href="#san-pham" onclick="filterProducts('xingfa'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cửa nhôm xingfa</a>
          <a href="#san-pham" onclick="filterProducts('nhua-loi-thep'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cửa nhựa lõi thép</a>
          <a href="#san-pham" onclick="filterProducts('tu-dong'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cửa kính tự động</a>
          <a href="#san-pham" onclick="filterProducts('cau-thang-kinh'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Cầu thang kính</a>
          <a href="#san-pham" onclick="filterProducts('kinh-op-bep'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Kính ốp bếp</a>
          <a href="#san-pham" onclick="filterProducts('phong-tam-kinh'); closeMobileMenu()" class="block py-2 text-xs font-medium text-slate-600 hover:text-brand-700">+ Phòng tắm kính</a>
        </div>
      </div>

      <a href="#cong-trinh" onclick="closeMobileMenu()" class="block px-4 py-3 text-sm font-semibold text-slate-700 hover:bg-brand-50">Công trình</a>
      <a href="#bao-gia" onclick="closeMobileMenu()" class="block px-4 py-3 text-sm font-semibold text-slate-700 hover:bg-brand-50">Báo giá</a>
      <a href="#tin-tuc" onclick="closeMobileMenu()" class="block px-4 py-3 text-sm font-semibold text-slate-700 hover:bg-brand-50">Tin tức</a>
      <a href="#lien-he" onclick="closeMobileMenu()" class="block px-4 py-3 text-sm font-semibold text-slate-700 hover:bg-brand-50">Liên hệ</a>
    </div>

    <div class="p-4 bg-slate-50 border-t border-slate-200 text-xs text-slate-600 space-y-1.5">
      <div class="font-bold text-brand-700">PHƯỚC TRÀ TKC • ĐÀ NẴNG</div>
      <div><i class="fa-solid fa-location-dot text-accent-500 mr-1.5"></i>365/12 Tôn Đản, P. An Khê, TP Đà Nẵng</div>
      <div><i class="fa-solid fa-phone text-accent-500 mr-1.5"></i>Hotline: <a href="tel:0905811246" class="font-bold text-brand-700">0905.811.246</a></div>
    </div>
  </aside>

  <!-- ========================================================= -->
  <!-- PHẦN 3: 2 BANNER TỰ TRƯỢT CHUYÊN NGHIỆP (KÍCH THƯỚC BẰNG NHAU, CHỮ CÁCH XA VIỀN, KHÔNG THIẾU CHỮ) -->
  <!-- ========================================================= -->
  <section id="trang-chu" class="pt-3 sm:pt-4 pb-4 sm:pb-6">
    <div class="tkc-container">
      <div id="heroSlider" class="relative rounded-2xl overflow-hidden shadow-lg bg-brand-900 select-none">
        <div class="hero-grid-track">

          <!-- BANNER 1 -->
          <div class="hero-slide is-active relative bg-gradient-to-br from-brand-900 via-brand-700 to-brand-600 text-white" data-slide="0">
            <!-- Họa tiết kiến trúc nền mờ nằm trọn bên trong banner -->
            <div class="absolute inset-0 opacity-15 pointer-events-none" style="background-image: radial-gradient(#ffffff 1px, transparent 1px); background-size: 24px 24px;"></div>

            <!-- Vùng an toàn chữ cách xa viền banner ở cả 4 phía -->
            <div class="relative z-10 px-9 sm:px-14 md:px-16 lg:px-20 py-8 sm:py-11 md:py-14 grid grid-cols-1 md:grid-cols-12 gap-6 lg:gap-10 items-center">
              <div class="md:col-span-7 space-y-3 sm:space-y-4">
                <p class="text-[11px] sm:text-xs font-bold uppercase tracking-[0.16em] text-accent-400">
                  CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC
                </p>
                <h1 class="text-xl sm:text-3xl lg:text-4xl font-extrabold leading-snug text-white">
                  Cửa Nhôm Xingfa Nhập Khẩu &amp; Kính Cường Lực Tại Đà Nẵng
                </h1>
                <p class="text-xs sm:text-sm lg:text-[15px] text-slate-200 leading-relaxed max-w-2xl">
                  Trực tiếp sản xuất, gia công và thi công trọn gói cửa nhôm Xingfa tem đỏ Quảng Đông, cửa kính cường lực, phòng tắm kính, cầu thang kính cho nhà phố, biệt thự và khách sạn tại Miền Trung.
                </p>
                <div class="pt-1 flex flex-wrap items-center gap-3">
                  <a href="#form-bao-gia" class="inline-flex items-center gap-2 bg-accent-500 hover:bg-accent-400 text-white font-bold text-xs sm:text-sm px-5 py-2.5 rounded-xl shadow-md transition">
                    <i class="fa-solid fa-file-invoice-dollar"></i>
                    <span>Nhận Báo Giá Nhanh</span>
                  </a>
                  <a href="#san-pham" class="inline-flex items-center gap-2 bg-white/15 hover:bg-white/25 border border-white/30 text-white font-semibold text-xs sm:text-sm px-5 py-2.5 rounded-xl transition">
                    <span>Xem Mẫu Cửa Đẹp</span>
                    <i class="fa-solid fa-arrow-right text-xs"></i>
                  </a>
                </div>
              </div>

              <!-- Khung ảnh sản phẩm thực tế đặt gọn bên trong banner -->
              <div class="md:col-span-5 flex justify-center">
                <div class="w-full max-w-md rounded-xl overflow-hidden border-2 border-white/25 shadow-2xl bg-brand-800 aspect-[16/10]">
                  <img
                    src="https://drive.google.com/thumbnail?id=1lxzMKWX3e_HJn7UELFZDOURuxh-NYZg-&sz=w1000"
                    alt="Cửa đi quay mở 4 cánh nhôm Xingfa Phước Trà TKC"
                    class="w-full h-full object-cover"
                    onerror="handleImgError(this, '1lxzMKWX3e_HJn7UELFZDOURuxh-NYZg-', 'Cua Nhom Xingfa Phuoc Tra TKC')"
                  />
                </div>
              </div>
            </div>
          </div>

          <!-- BANNER 2 -->
          <div class="hero-slide is-inactive relative bg-gradient-to-br from-slate-900 via-brand-800 to-brand-700 text-white" data-slide="1">
            <div class="absolute inset-0 opacity-15 pointer-events-none" style="background-image: linear-gradient(135deg, rgba(245,158,11,0.22) 0%, transparent 55%);"></div>

            <!-- Vùng an toàn chữ cách xa viền banner tương đồng hoàn toàn với Banner 1 -->
            <div class="relative z-10 px-9 sm:px-14 md:px-16 lg:px-20 py-8 sm:py-11 md:py-14 grid grid-cols-1 md:grid-cols-12 gap-6 lg:gap-10 items-center">
              <div class="md:col-span-7 space-y-3 sm:space-y-4">
                <p class="text-[11px] sm:text-xs font-bold uppercase tracking-[0.16em] text-accent-400">
                  GIẢI PHÁP CÔNG TRÌNH • PHUOCTRATKC.COM
                </p>
                <h2 class="text-xl sm:text-3xl lg:text-4xl font-extrabold leading-snug text-white">
                  Thi Công Hạng Mục Nhôm Kính Khách Sạn, Resort &amp; Biệt Thự
                </h2>
                <p class="text-xs sm:text-sm lg:text-[15px] text-slate-200 leading-relaxed max-w-2xl">
                  Đồng hành cùng hàng trăm công trình trọng điểm tại Đà Nẵng và Quảng Nam. Khảo sát tận nơi miễn phí, tư vấn kỹ thuật chuẩn xác, báo giá minh bạch trực tiếp tại xưởng sản xuất.
                </p>
                <div class="pt-1 flex flex-wrap items-center gap-3">
                  <a href="#cong-trinh" class="inline-flex items-center gap-2 bg-accent-500 hover:bg-accent-400 text-white font-bold text-xs sm:text-sm px-5 py-2.5 rounded-xl shadow-md transition">
                    <i class="fa-solid fa-building"></i>
                    <span>Xem Công Trình Đà Nẵng</span>
                  </a>
                  <a href="tel:0905811246" class="inline-flex items-center gap-2 bg-white/15 hover:bg-white/25 border border-white/30 text-white font-semibold text-xs sm:text-sm px-5 py-2.5 rounded-xl transition">
                    <i class="fa-solid fa-phone"></i>
                    <span>0905.811.246</span>
                  </a>
                </div>
              </div>

              <!-- Khung ảnh dự án thực tế đặt gọn bên trong banner -->
              <div class="md:col-span-5 flex justify-center">
                <div class="w-full max-w-md rounded-xl overflow-hidden border-2 border-white/25 shadow-2xl bg-brand-800 aspect-[16/10]">
                  <img
                    src="https://drive.google.com/thumbnail?id=1MmAfsyp3s3YCaEMymrkk8TZbD38jCsAQ&sz=w1000"
                    alt="Dự án Resort Mỹ Sơn 4 sao do Phước Trà TKC thi công"
                    class="w-full h-full object-cover"
                    onerror="handleImgError(this, '1MmAfsyp3s3YCaEMymrkk8TZbD38jCsAQ', 'Du An Khach San Da Nang')"
                  />
                </div>
              </div>
            </div>
          </div>

        </div>

        <!-- Nút chuyển slide trái / phải đặt sát mép gọn gàng, không đè lên chữ -->
        <button type="button" onclick="prevSlide()" class="absolute left-2 sm:left-3 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-9 sm:h-9 rounded-full bg-black/30 hover:bg-accent-500 text-white flex items-center justify-center transition" aria-label="Banner trước">
          <i class="fa-solid fa-chevron-left text-xs sm:text-sm"></i>
        </button>
        <button type="button" onclick="nextSlide()" class="absolute right-2 sm:right-3 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-9 sm:h-9 rounded-full bg-black/30 hover:bg-accent-500 text-white flex items-center justify-center transition" aria-label="Banner tiếp theo">
          <i class="fa-solid fa-chevron-right text-xs sm:text-sm"></i>
        </button>

        <!-- Dấu chấm chỉ báo slide -->
        <div class="absolute bottom-2.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
          <button type="button" onclick="goToSlide(0)" class="hero-dot w-6 h-2 rounded-full bg-accent-400 transition-all" aria-label="Xem banner 1"></button>
          <button type="button" onclick="goToSlide(1)" class="hero-dot w-2.5 h-2 rounded-full bg-white/45 hover:bg-white/80 transition-all" aria-label="Xem banner 2"></button>
        </div>
      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 4: DANH MỤC SẢN PHẨM (LẤY THEO WEB MẪU, CHỮ NHỎ GỌN) -->
  <!-- ========================================================= -->
  <section id="danh-muc-san-pham" class="py-6 sm:py-8">
    <div class="tkc-container">
      <!-- Tiêu đề Flatsome Section Divider -->
      <div class="flex items-center gap-3 mb-5">
        <span class="h-[2px] flex-1 bg-slate-200"></span>
        <h2 class="text-sm sm:text-lg font-extrabold uppercase tracking-wide text-brand-700 text-center">
          Danh Mục Sản Phẩm
        </h2>
        <span class="h-[2px] flex-1 bg-slate-200"></span>
      </div>

      <!-- 6 Danh mục sản phẩm với ảnh Google Drive thực tế -->
      <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-6 gap-2.5 sm:gap-4">
        <a href="#san-pham" onclick="filterProducts('xingfa')" class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md hover:border-brand-600 transition flex flex-col">
          <div class="aspect-[4/3] overflow-hidden bg-slate-100">
            <img src="https://drive.google.com/thumbnail?id=1zRlHJBAneXS7EQ1jdT__hVRCTf2mzOiX&sz=w800" alt="Cửa nhôm xingfa" class="w-full h-full object-cover group-hover:scale-105 transition duration-300" onerror="handleImgError(this, '1zRlHJBAneXS7EQ1jdT__hVRCTf2mzOiX', 'Cua Nhom Xingfa')" />
          </div>
          <div class="p-2.5 text-center flex-1 flex items-center justify-center">
            <span class="text-[11px] sm:text-xs font-bold uppercase text-brand-700 group-hover:text-accent-500 leading-tight transition">Cửa nhôm xingfa</span>
          </div>
        </a>

        <a href="#san-pham" onclick="filterProducts('nhua-loi-thep')" class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md hover:border-brand-600 transition flex flex-col">
          <div class="aspect-[4/3] overflow-hidden bg-slate-100">
            <img src="https://drive.google.com/thumbnail?id=1jiHBW-2MoWUHjQUicSe-rO6NlmfNuZNA&sz=w800" alt="Cửa nhựa lõi thép" class="w-full h-full object-cover group-hover:scale-105 transition duration-300" onerror="handleImgError(this, '1jiHBW-2MoWUHjQUicSe-rO6NlmfNuZNA', 'Cua Nhua Loi Thep')" />
          </div>
          <div class="p-2.5 text-center flex-1 flex items-center justify-center">
            <span class="text-[11px] sm:text-xs font-bold uppercase text-brand-700 group-hover:text-accent-500 leading-tight transition">Cửa nhựa lõi thép</span>
          </div>
        </a>

        <a href="#san-pham" onclick="filterProducts('tu-dong')" class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md hover:border-brand-600 transition flex flex-col">
          <div class="aspect-[4/3] overflow-hidden bg-slate-100">
            <img src="https://drive.google.com/thumbnail?id=1PIFP1UCQs_FIaKCgGwcJWt-5wTnST9iJ&sz=w800" alt="Cửa kính tự động" class="w-full h-full object-cover group-hover:scale-105 transition duration-300" onerror="handleImgError(this, '1PIFP1UCQs_FIaKCgGwcJWt-5wTnST9iJ', 'Cua Kinh Tu Dong')" />
          </div>
          <div class="p-2.5 text-center flex-1 flex items-center justify-center">
            <span class="text-[11px] sm:text-xs font-bold uppercase text-brand-700 group-hover:text-accent-500 leading-tight transition">Cửa kính tự động</span>
          </div>
        </a>

        <a href="#san-pham" onclick="filterProducts('cau-thang-kinh')" class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md hover:border-brand-600 transition flex flex-col">
          <div class="aspect-[4/3] overflow-hidden bg-slate-100">
            <img src="https://drive.google.com/thumbnail?id=1FnuITlKMjk-xTxkIV96ABv43S1PG--Ul&sz=w800" alt="Cầu thang kính" class="w-full h-full object-cover group-hover:scale-105 transition duration-300" onerror="handleImgError(this, '1FnuITlKMjk-xTxkIV96ABv43S1PG--Ul', 'Cau Thang Kinh')" />
          </div>
          <div class="p-2.5 text-center flex-1 flex items-center justify-center">
            <span class="text-[11px] sm:text-xs font-bold uppercase text-brand-700 group-hover:text-accent-500 leading-tight transition">Cầu thang kính</span>
          </div>
        </a>

        <a href="#san-pham" onclick="filterProducts('kinh-op-bep')" class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md hover:border-brand-600 transition flex flex-col">
          <div class="aspect-[4/3] overflow-hidden bg-slate-100">
            <img src="https://drive.google.com/thumbnail?id=1ilanOshTrs9llnMXWl5iZ8DtgptJ0hCb&sz=w800" alt="Kính ốp bếp" class="w-full h-full object-cover group-hover:scale-105 transition duration-300" onerror="handleImgError(this, '1ilanOshTrs9llnMXWl5iZ8DtgptJ0hCb', 'Kinh Op Bep')" />
          </div>
          <div class="p-2.5 text-center flex-1 flex items-center justify-center">
            <span class="text-[11px] sm:text-xs font-bold uppercase text-brand-700 group-hover:text-accent-500 leading-tight transition">Kính ốp bếp</span>
          </div>
        </a>

        <a href="#san-pham" onclick="filterProducts('phong-tam-kinh')" class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md hover:border-brand-600 transition flex flex-col">
          <div class="aspect-[4/3] overflow-hidden bg-slate-100">
            <img src="https://drive.google.com/thumbnail?id=1MhCILHQ5goD1cAPTt1hZsY_ajeOMs-qH&sz=w800" alt="Phòng tắm kính" class="w-full h-full object-cover group-hover:scale-105 transition duration-300" onerror="handleImgError(this, '1MhCILHQ5goD1cAPTt1hZsY_ajeOMs-qH', 'Phong Tam Kinh')" />
          </div>
          <div class="p-2.5 text-center flex-1 flex items-center justify-center">
            <span class="text-[11px] sm:text-xs font-bold uppercase text-brand-700 group-hover:text-accent-500 leading-tight transition">Phòng tắm kính</span>
          </div>
        </a>
      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 5: SẢN PHẨM NỔI BẬT (2 CỘT TRÊN ĐIỆN THOẠI, GIÁ & GIẢM GIÁ % GÓC TRÊN TRÁI) -->
  <!-- ========================================================= -->
  <section id="san-pham" class="py-6 sm:py-9 bg-white border-y border-slate-200">
    <div class="tkc-container">
      <div class="flex items-center gap-3 mb-4">
        <span class="h-[2px] flex-1 bg-slate-200"></span>
        <h2 class="text-sm sm:text-lg font-extrabold uppercase tracking-wide text-brand-700 text-center">
          Sản Phẩm Cửa Nhôm Xingfa &amp; Kính Cường Lực
        </h2>
        <span class="h-[2px] flex-1 bg-slate-200"></span>
      </div>

      <!-- Thanh lọc danh mục sản phẩm gọn nhẹ -->
      <div id="productFilterTabs" class="flex flex-wrap items-center justify-center gap-1.5 sm:gap-2 mb-5">
        <button type="button" data-cat="all" onclick="filterProducts('all')" class="filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-brand-700 text-white transition">Tất cả</button>
        <button type="button" data-cat="xingfa" onclick="filterProducts('xingfa')" class="filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-slate-100 text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhôm Xingfa</button>
        <button type="button" data-cat="kinh-cuong-luc" onclick="filterProducts('kinh-cuong-luc')" class="filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-slate-100 text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa kính cường lực</button>
        <button type="button" data-cat="nhua-loi-thep" onclick="filterProducts('nhua-loi-thep')" class="filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-slate-100 text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa nhựa lõi thép</button>
        <button type="button" data-cat="tu-dong" onclick="filterProducts('tu-dong')" class="filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-slate-100 text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cửa tự động</button>
        <button type="button" data-cat="cau-thang-kinh" onclick="filterProducts('cau-thang-kinh')" class="filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-slate-100 text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Cầu thang kính</button>
        <button type="button" data-cat="kinh-op-bep" onclick="filterProducts('kinh-op-bep')" class="filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-slate-100 text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Kính ốp bếp</button>
        <button type="button" data-cat="phong-tam-kinh" onclick="filterProducts('phong-tam-kinh')" class="filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-slate-100 text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition">Phòng tắm kính</button>
      </div>

      <!-- Lưới sản phẩm: 2 cột trên điện thoại (grid-cols-2), 3 cột trên tablet, 4 cột trên máy tính -->
      <div id="productGrid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-2.5 sm:gap-4 lg:gap-5">
        <!-- Dữ liệu sản phẩm được render tự động qua JavaScript đảm bảo hiển thị đầy đủ tên không cắt chữ -->
      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 6: GIỚI THIỆU CÔNG TY & BẢNG BÁO GIÁ THAM KHẢO -->
  <!-- ========================================================= -->
  <section id="gioi-thieu" class="py-7 sm:py-10">
    <div class="tkc-container">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-start">

        <!-- Giới thiệu ngắn gọn chuẩn Flatsome -->
        <div class="lg:col-span-5 bg-white rounded-2xl border border-slate-200 p-5 sm:p-6 shadow-xs space-y-4">
          <div class="border-l-4 border-accent-500 pl-3">
            <p class="text-[11px] font-bold uppercase tracking-wider text-accent-600">Về chúng tôi</p>
            <h2 class="text-base sm:text-xl font-extrabold text-brand-700 leading-snug">
              CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC
            </h2>
          </div>

          <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
            <strong>Phước Trà TKC</strong> là đơn vị chuyên thiết kế, gia công và thi công lắp đặt các hạng mục nhôm kính cao cấp hàng đầu tại Đà Nẵng và khu vực Miền Trung. Các dòng sản phẩm chủ lực gồm: <strong>Cửa nhôm Xingfa nhập khẩu tem đỏ Quảng Đông</strong>, cửa kính cường lực, cửa nhựa lõi thép, cửa kính tự động, cầu thang kính, phòng tắm kính và kính màu ốp bếp.
          </p>
          <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
            Với quy trình ép góc tự động hiện đại, phụ kiện đồng bộ chính hãng cùng đội ngũ kỹ thuật tay nghề cao, chúng tôi cam kết mang đến không gian sang trọng, bền bỉ trước khí hậu ven biển và chính sách bảo hành minh bạch dài hạn.
          </p>

          <!-- 4 chỉ số nổi bật tinh giản -->
          <div class="grid grid-cols-2 gap-3 pt-2">
            <div class="bg-brand-50 rounded-xl p-3 text-center border border-brand-100">
              <div class="text-lg sm:text-xl font-extrabold text-brand-700">150+</div>
              <div class="text-[11px] sm:text-xs font-medium text-slate-600">Công trình hoàn thiện</div>
            </div>
            <div class="bg-brand-50 rounded-xl p-3 text-center border border-brand-100">
              <div class="text-lg sm:text-xl font-extrabold text-brand-700">50+</div>
              <div class="text-[11px] sm:text-xs font-medium text-slate-600">Kỹ thuật viên kinh nghiệm</div>
            </div>
            <div class="bg-brand-50 rounded-xl p-3 text-center border border-brand-100">
              <div class="text-lg sm:text-xl font-extrabold text-brand-700">100+</div>
              <div class="text-[11px] sm:text-xs font-medium text-slate-600">Mẫu cửa nhôm kính</div>
            </div>
            <div class="bg-brand-50 rounded-xl p-3 text-center border border-brand-100">
              <div class="text-lg sm:text-xl font-extrabold text-brand-700">100%</div>
              <div class="text-[11px] sm:text-xs font-medium text-slate-600">Khách hàng hài lòng</div>
            </div>
          </div>
        </div>

        <!-- Bảng báo giá cửa nhôm Xingfa & kính cường lực Đà Nẵng -->
        <div id="bao-gia" class="lg:col-span-7 bg-white rounded-2xl border border-slate-200 p-5 sm:p-6 shadow-xs">
          <div class="flex flex-wrap items-center justify-between gap-2 mb-4">
            <div class="border-l-4 border-brand-700 pl-3">
              <p class="text-[11px] font-bold uppercase tracking-wider text-brand-600">Cập nhật mới nhất</p>
              <h2 class="text-base sm:text-xl font-extrabold text-brand-700">
                Bảng Báo Giá Cửa Nhôm Xingfa Đà Nẵng
              </h2>
            </div>
            <a href="#form-bao-gia" class="text-xs font-bold text-accent-600 hover:text-brand-700 transition">
              Nhận báo giá chi tiết <i class="fa-solid fa-arrow-right ml-1"></i>
            </a>
          </div>

          <div class="overflow-x-auto rounded-xl border border-slate-200">
            <table class="w-full text-left border-collapse text-xs sm:text-sm">
              <thead>
                <tr class="bg-brand-700 text-white">
                  <th class="py-2.5 px-3 font-semibold">Hạng mục cửa nhôm Xingfa nhập khẩu</th>
                  <th class="py-2.5 px-3 font-semibold whitespace-nowrap">Hệ nhôm / Độ dày</th>
                  <th class="py-2.5 px-3 font-semibold text-right whitespace-nowrap">Đơn giá (VNĐ/m²)</th>
                </tr>
              </thead>
              <tbody class="divide-y divide-slate-200">
                <tr class="hover:bg-slate-50">
                  <td class="py-2.5 px-3 font-medium text-slate-800">Cửa sổ mở trượt / mở quay / mở hất</td>
                  <td class="py-2.5 px-3 text-slate-600 whitespace-nowrap">Hệ 55 / 93 (1.4mm)</td>
                  <td class="py-2.5 px-3 text-right font-bold text-red-600 whitespace-nowrap">1.750.000 ₫</td>
                </tr>
                <tr class="hover:bg-slate-50">
                  <td class="py-2.5 px-3 font-medium text-slate-800">Cửa đi mở quay 1 cánh, 2 cánh</td>
                  <td class="py-2.5 px-3 text-slate-600 whitespace-nowrap">Hệ 55 (2.0mm)</td>
                  <td class="py-2.5 px-3 text-right font-bold text-red-600 whitespace-nowrap">2.100.000 ₫</td>
                </tr>
                <tr class="hover:bg-slate-50">
                  <td class="py-2.5 px-3 font-medium text-slate-800">Cửa đi mở quay 3 cánh, 4 cánh</td>
                  <td class="py-2.5 px-3 text-slate-600 whitespace-nowrap">Hệ 55 (2.0mm)</td>
                  <td class="py-2.5 px-3 text-right font-bold text-red-600 whitespace-nowrap">2.100.000 ₫</td>
                </tr>
                <tr class="hover:bg-slate-50">
                  <td class="py-2.5 px-3 font-medium text-slate-800">Cửa đi xếp trượt gấp 4 - 6 cánh</td>
                  <td class="py-2.5 px-3 text-slate-600 whitespace-nowrap">Hệ 63 (2.0mm)</td>
                  <td class="py-2.5 px-3 text-right font-bold text-red-600 whitespace-nowrap">2.150.000 ₫</td>
                </tr>
                <tr class="hover:bg-slate-50">
                  <td class="py-2.5 px-3 font-medium text-slate-800">Cửa kính cường lực 10mm bản lề sàn</td>
                  <td class="py-2.5 px-3 text-slate-600 whitespace-nowrap">Kính 10mm + VVP</td>
                  <td class="py-2.5 px-3 text-right font-bold text-red-600 whitespace-nowrap">850.000 ₫</td>
                </tr>
                <tr class="hover:bg-slate-50">
                  <td class="py-2.5 px-3 font-medium text-slate-800">Phòng tắm kính / Cầu thang kính cường lực</td>
                  <td class="py-2.5 px-3 text-slate-600 whitespace-nowrap">Kính 10mm Inox 304</td>
                  <td class="py-2.5 px-3 text-right font-bold text-red-600 whitespace-nowrap">1.150.000 ₫</td>
                </tr>
              </tbody>
            </table>
          </div>
          <p class="mt-3 text-[11px] sm:text-xs text-slate-500">
            * Đơn giá tham khảo đã bao gồm kính an toàn 6.38mm hoặc cường lực 8mm, vận chuyển và lắp đặt tại nội thành Đà Nẵng. Liên hệ <strong>0905.811.246</strong> để nhận chiết khấu cho công trình diện tích lớn.
          </p>
        </div>

      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 7: CÁC DỰ ÁN TIÊU BIỂU TẠI ĐÀ NẴNG -->
  <!-- ========================================================= -->
  <section id="cong-trinh" class="py-7 sm:py-10 bg-white border-y border-slate-200">
    <div class="tkc-container">
      <div class="flex items-center gap-3 mb-5">
        <span class="h-[2px] flex-1 bg-slate-200"></span>
        <h2 class="text-sm sm:text-lg font-extrabold uppercase tracking-wide text-brand-700 text-center">
          Các Dự Án Tiêu Biểu Tại Đà Nẵng
        </h2>
        <span class="h-[2px] flex-1 bg-slate-200"></span>
      </div>

      <div id="projectGrid" class="grid grid-cols-2 lg:grid-cols-3 gap-3 sm:gap-5">
        <!-- Render 6 dự án Đà Nẵng từ dữ liệu Google Drive chính xác -->
      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 8: FORM YÊU CẦU TƯ VẤN & BÁO GIÁ TRANG CHỦ -->
  <!-- ========================================================= -->
  <section id="form-bao-gia" class="py-7 sm:py-10 bg-gradient-to-br from-brand-800 via-brand-700 to-brand-900 text-white">
    <div class="tkc-container">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 lg:gap-10 items-center">
        <div class="lg:col-span-5 space-y-3">
          <p class="text-xs font-bold uppercase tracking-widest text-accent-400">Tư vấn &amp; Khảo sát miễn phí</p>
          <h2 class="text-xl sm:text-2xl lg:text-3xl font-extrabold leading-snug">
            Đăng Ký Nhận Báo Giá Trực Tiếp Từ Xưởng Phước Trà TKC
          </h2>
          <p class="text-xs sm:text-sm text-slate-200 leading-relaxed">
            Để lại thông tin hạng mục cần thi công, đội ngũ kỹ sư của <strong>CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC</strong> sẽ liên hệ tư vấn giải pháp tối ưu và gửi bảng dự toán chi tiết trong vòng 15 phút.
          </p>
          <div class="pt-2 space-y-2 text-xs sm:text-sm text-slate-100">
            <div class="flex items-center gap-2.5">
              <i class="fa-solid fa-check-circle text-accent-400"></i>
              <span>Đo đạc khảo sát tận công trình tại Đà Nẵng &amp; lân cận</span>
            </div>
            <div class="flex items-center gap-2.5">
              <i class="fa-solid fa-check-circle text-accent-400"></i>
              <span>Bóc tách khối lượng minh bạch, không phát sinh chi phí</span>
            </div>
            <div class="flex items-center gap-2.5">
              <i class="fa-solid fa-check-circle text-accent-400"></i>
              <span>Hotline hỗ trợ kỹ thuật 24/7: <a href="tel:0905811246" class="font-bold text-accent-400 underline">0905.811.246</a></span>
            </div>
          </div>
        </div>

        <div class="lg:col-span-7">
          <form id="quoteForm" class="bg-white text-slate-800 rounded-2xl p-5 sm:p-7 shadow-xl space-y-4">
            <h3 class="text-base sm:text-lg font-extrabold text-brand-700">Form Yêu Cầu &amp; Báo Giá Nhanh</h3>
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
              <div>
                <label for="qName" class="block text-xs font-semibold text-slate-700 mb-1">Họ và tên *</label>
                <input id="qName" type="text" required placeholder="Nhập họ tên quý khách..." class="w-full px-3.5 py-2.5 text-sm rounded-xl border border-slate-300 focus:border-brand-600 focus:ring-2 focus:ring-brand-100 outline-none transition" />
              </div>
              <div>
                <label for="qPhone" class="block text-xs font-semibold text-slate-700 mb-1">Số điện thoại / Zalo *</label>
                <input id="qPhone" type="tel" required placeholder="VD: 0905.xxx.xxx" class="w-full px-3.5 py-2.5 text-sm rounded-xl border border-slate-300 focus:border-brand-600 focus:ring-2 focus:ring-brand-100 outline-none transition" />
              </div>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
              <div>
                <label for="qService" class="block text-xs font-semibold text-slate-700 mb-1">Danh mục sản phẩm quan tâm</label>
                <select id="qService" class="w-full px-3.5 py-2.5 text-sm rounded-xl border border-slate-300 focus:border-brand-600 focus:ring-2 focus:ring-brand-100 outline-none bg-white transition">
                  <option value="Cửa nhôm Xingfa nhập khẩu">Cửa nhôm Xingfa nhập khẩu</option>
                  <option value="Cửa kính cường lực">Cửa kính cường lực</option>
                  <option value="Cửa nhựa lõi thép">Cửa nhựa lõi thép</option>
                  <option value="Cửa kính tự động">Cửa kính tự động</option>
                  <option value="Cầu thang kính cường lực">Cầu thang kính cường lực</option>
                  <option value="Kính ốp bếp cường lực">Kính ốp bếp cường lực</option>
                  <option value="Phòng tắm kính">Phòng tắm kính</option>
                </select>
              </div>
              <div>
                <label for="qArea" class="block text-xs font-semibold text-slate-700 mb-1">Địa điểm công trình</label>
                <input id="qArea" type="text" placeholder="VD: Quận Thanh Khê, TP Đà Nẵng" class="w-full px-3.5 py-2.5 text-sm rounded-xl border border-slate-300 focus:border-brand-600 focus:ring-2 focus:ring-brand-100 outline-none transition" />
              </div>
            </div>

            <div>
              <label for="qNote" class="block text-xs font-semibold text-slate-700 mb-1">Nội dung yêu cầu / Kích thước dự kiến</label>
              <textarea id="qNote" rows="3" placeholder="Mô tả số lượng bộ cửa, diện tích dự kiến hoặc yêu cầu kỹ thuật..." class="w-full px-3.5 py-2.5 text-sm rounded-xl border border-slate-300 focus:border-brand-600 focus:ring-2 focus:ring-brand-100 outline-none transition"></textarea>
            </div>

            <button type="submit" class="w-full sm:w-auto inline-flex items-center justify-center gap-2 bg-accent-500 hover:bg-accent-600 text-white font-bold text-sm px-7 py-3 rounded-xl shadow-md transition cursor-pointer">
              <i class="fa-solid fa-paper-plane"></i>
              <span>Gửi Yêu Cầu Báo Giá Ngay</span>
            </button>
          </form>
        </div>
      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 9: DANH MỤC CÁC BÀI VIẾT / TIN TỨC TRANG CHỦ -->
  <!-- ========================================================= -->
  <section id="tin-tuc" class="py-7 sm:py-10">
    <div class="tkc-container">
      <div class="flex items-center gap-3 mb-4">
        <span class="h-[2px] flex-1 bg-slate-200"></span>
        <h2 class="text-sm sm:text-lg font-extrabold uppercase tracking-wide text-brand-700 text-center">
          Tin Tức &amp; Kinh Nghiệm Nhôm Kính
        </h2>
        <span class="h-[2px] flex-1 bg-slate-200"></span>
      </div>

      <!-- Danh mục các bài viết trang chủ -->
      <div class="flex flex-wrap items-center justify-center gap-1.5 sm:gap-2 mb-5">
        <button type="button" onclick="filterArticles('all', this)" class="article-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-brand-700 text-white transition">Tất cả bài viết</button>
        <button type="button" onclick="filterArticles('tu-van', this)" class="article-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-white border border-slate-200 text-slate-700 hover:bg-brand-50 transition">Tư vấn cửa nhôm</button>
        <button type="button" onclick="filterArticles('ky-thuat', this)" class="article-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-white border border-slate-200 text-slate-700 hover:bg-brand-50 transition">Kỹ thuật thi công</button>
        <button type="button" onclick="filterArticles('bao-gia-tin', this)" class="article-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-white border border-slate-200 text-slate-700 hover:bg-brand-50 transition">Kinh nghiệm báo giá</button>
      </div>

      <div id="articleGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
        <!-- Bài viết được render từ JS -->
      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 10: ĐỐI TÁC CỦA CHÚNG TÔI (6 ẢNH ĐỐI TÁC GOOGLE DRIVE) -->
  <!-- ========================================================= -->
  <section class="py-7 sm:py-9 bg-white border-y border-slate-200">
    <div class="tkc-container">
      <div class="flex items-center gap-3 mb-5">
        <span class="h-[2px] flex-1 bg-slate-200"></span>
        <h2 class="text-sm sm:text-lg font-extrabold uppercase tracking-wide text-brand-700 text-center">
          Đối Tác Của Chúng Tôi
        </h2>
        <span class="h-[2px] flex-1 bg-slate-200"></span>
      </div>

      <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-6 gap-3 sm:gap-4">
        <div class="bg-white rounded-xl border border-slate-200 p-3 h-20 sm:h-24 flex items-center justify-center hover:shadow-md transition">
          <img src="https://drive.google.com/thumbnail?id=13il4TeS8ZnrK0CD4VDPMdNX3EKxY8AFk&sz=w600" alt="Đối tác Phước Trà TKC 1" class="max-h-full max-w-full object-contain" onerror="handleImgError(this, '13il4TeS8ZnrK0CD4VDPMdNX3EKxY8AFk', 'Doi Tac 1')" />
        </div>
        <div class="bg-white rounded-xl border border-slate-200 p-3 h-20 sm:h-24 flex items-center justify-center hover:shadow-md transition">
          <img src="https://drive.google.com/thumbnail?id=1QRcPtjWfg5PEQXw6UMg6ZylQhg8BpzUq&sz=w600" alt="Đối tác Phước Trà TKC 2" class="max-h-full max-w-full object-contain" onerror="handleImgError(this, '1QRcPtjWfg5PEQXw6UMg6ZylQhg8BpzUq', 'Doi Tac 2')" />
        </div>
        <div class="bg-white rounded-xl border border-slate-200 p-3 h-20 sm:h-24 flex items-center justify-center hover:shadow-md transition">
          <img src="https://drive.google.com/thumbnail?id=1-Ka-zScPzx653Tg2oWE9-qmFtTdn3Svn&sz=w600" alt="Đối tác Phước Trà TKC 3" class="max-h-full max-w-full object-contain" onerror="handleImgError(this, '1-Ka-zScPzx653Tg2oWE9-qmFtTdn3Svn', 'Doi Tac 3')" />
        </div>
        <div class="bg-white rounded-xl border border-slate-200 p-3 h-20 sm:h-24 flex items-center justify-center hover:shadow-md transition">
          <img src="https://drive.google.com/thumbnail?id=1Oy52Wdfy5x6DKF1lyfYxpZTD5fvGH5vT&sz=w600" alt="Đối tác Phước Trà TKC 4" class="max-h-full max-w-full object-contain" onerror="handleImgError(this, '1Oy52Wdfy5x6DKF1lyfYxpZTD5fvGH5vT', 'Doi Tac 4')" />
        </div>
        <div class="bg-white rounded-xl border border-slate-200 p-3 h-20 sm:h-24 flex items-center justify-center hover:shadow-md transition">
          <img src="https://drive.google.com/thumbnail?id=1SDcarhnX0yypmqdbawICjYBRtFnKngn-&sz=w600" alt="Đối tác Phước Trà TKC 5" class="max-h-full max-w-full object-contain" onerror="handleImgError(this, '1SDcarhnX0yypmqdbawICjYBRtFnKngn-', 'Doi Tac 5')" />
        </div>
        <div class="bg-white rounded-xl border border-slate-200 p-3 h-20 sm:h-24 flex items-center justify-center hover:shadow-md transition">
          <img src="https://drive.google.com/thumbnail?id=1Ua4C1iiZqrjkWx-3h2quvqM0w_Xj33fg&sz=w600" alt="Đối tác Phước Trà TKC 6" class="max-h-full max-w-full object-contain" onerror="handleImgError(this, '1Ua4C1iiZqrjkWx-3h2quvqM0w_Xj33fg', 'Doi Tac 6')" />
        </div>
      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 11: BẢN ĐỒ GOOGLE MAP & FANPAGE FACEBOOK NGOÀI TRANG CHỦ -->
  <!-- ========================================================= -->
  <section id="lien-he" class="py-7 sm:py-10">
    <div class="tkc-container">
      <div class="flex items-center gap-3 mb-5">
        <span class="h-[2px] flex-1 bg-slate-200"></span>
        <h2 class="text-sm sm:text-lg font-extrabold uppercase tracking-wide text-brand-700 text-center">
          Bản Đồ Chỉ Đường &amp; Fanpage Facebook
        </h2>
        <span class="h-[2px] flex-1 bg-slate-200"></span>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-5 items-stretch">
        <!-- Google Map trực tiếp trên trang chủ -->
        <div class="lg:col-span-7 bg-white rounded-2xl border border-slate-200 shadow-xs overflow-hidden flex flex-col">
          <div class="px-4 py-3 bg-slate-50 border-b border-slate-200 flex flex-wrap items-center justify-between gap-2">
            <div class="flex items-center gap-2 text-xs sm:text-sm font-bold text-brand-700">
              <i class="fa-solid fa-map-location-dot text-accent-500"></i>
              <span>365/12 Tôn Đản, Phường An Khê, TP Đà Nẵng</span>
            </div>
            <a href="https://www.google.com/maps/search/?api=1&query=365%2F12+T%C3%B4n+%C4%90%E1%BA%A3n,+Ph%C6%B0%E1%BB%9Dng+An+Kh%C3%AA,+TP+%C4%90%C3%A0+N%E1%BA%B5ng" target="_blank" rel="noopener noreferrer" class="text-xs font-semibold text-brand-600 hover:text-accent-600 transition">
              Mở Google Maps <i class="fa-solid fa-arrow-up-right-from-square ml-1 text-[10px]"></i>
            </a>
          </div>
          <div class="w-full flex-1 min-h-[280px] sm:min-h-[340px] bg-slate-100">
            <iframe
              title="Bản đồ Công Ty TNHH Đầu Tư Xây Dựng Phước Trà TKC"
              src="https://maps.google.com/maps?q=365%2F12%20T%C3%B4n%20%C4%90%E1%BA%A3n%2C%20An%20Kh%C3%AA%2C%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=16&ie=UTF8&iwloc=&output=embed"
              class="w-full h-full min-h-[280px] sm:min-h-[340px] border-0"
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"
              allowfullscreen>
            </iframe>
          </div>
        </div>

        <!-- Fanpage Facebook trực tiếp ngoài trang chủ -->
        <div class="lg:col-span-5 bg-white rounded-2xl border border-slate-200 shadow-xs overflow-hidden flex flex-col">
          <div class="px-4 py-3 bg-[#1877F2] text-white flex items-center justify-between">
            <div class="flex items-center gap-2 text-xs sm:text-sm font-bold">
              <i class="fa-brands fa-facebook text-base"></i>
              <span>Fanpage Chính Thức Phước Trà TKC</span>
            </div>
            <span class="text-[11px] bg-white/20 px-2 py-0.5 rounded-full">Facebook</span>
          </div>

          <!-- Khung hiển thị Fanpage Facebook chuyên nghiệp -->
          <div class="p-4 flex-1 flex flex-col justify-between gap-4">
            <div class="relative rounded-xl overflow-hidden border border-slate-200 bg-brand-900">
              <img
                src="https://drive.google.com/thumbnail?id=1wH-JJ2rOYRmDGsNapl3bIBjfiG3Qm6zZ&sz=w800"
                alt="Ảnh bìa Fanpage Phước Trà TKC"
                class="w-full h-36 object-cover opacity-55"
                onerror="handleImgError(this, '1wH-JJ2rOYRmDGsNapl3bIBjfiG3Qm6zZ', 'Fanpage Phuoc Tra TKC')"
              />
              <div class="absolute inset-0 bg-gradient-to-t from-slate-900/90 via-slate-900/35 to-transparent p-3.5 flex flex-col justify-between">
                <div class="flex items-center gap-3">
                  <div class="w-12 h-12 rounded-xl bg-white p-1 shadow-md shrink-0 flex items-center justify-center">
                    <svg class="w-10 h-10" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <rect x="2" y="2" width="60" height="60" rx="12" fill="#0B3B66" />
                      <path d="M14 25L32 12L50 25" stroke="#F59E0B" stroke-width="3.2" stroke-linecap="round" stroke-linejoin="round" />
                      <rect x="17" y="27" width="13" height="23" rx="2" fill="#FFFFFF" />
                      <rect x="34" y="27" width="13" height="23" rx="2" fill="#F59E0B" />
                    </svg>
                  </div>
                  <div class="min-w-0 text-white">
                    <div class="font-bold text-sm leading-tight truncate">Nhôm Kính Phước Trà TKC Đà Nẵng</div>
                    <div class="text-[11px] text-slate-200 mt-0.5">5.840 người theo dõi • Xây dựng &amp; Nhôm kính</div>
                  </div>
                </div>

                <div class="flex items-center justify-between gap-2">
                  <a href="https://facebook.com" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 bg-white text-slate-800 hover:bg-slate-100 text-xs font-bold px-3 py-1.5 rounded-lg shadow transition">
                    <i class="fa-brands fa-facebook-square text-[#1877F2]"></i>
                    <span>Theo dõi Trang</span>
                  </a>
                  <a href="https://m.me" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 bg-[#1877F2] hover:bg-blue-700 text-white text-xs font-bold px-3 py-1.5 rounded-lg shadow transition">
                    <i class="fa-brands fa-facebook-messenger"></i>
                    <span>Nhắn tin</span>
                  </a>
                </div>
              </div>
            </div>

            <!-- Bài đăng mới nhất trên Fanpage -->
            <div class="rounded-xl bg-slate-50 border border-slate-200 p-3.5 space-y-2 text-xs text-slate-700">
              <div class="flex items-center justify-between text-[11px] text-slate-500">
                <span class="font-bold text-brand-700">Phước Trà TKC • Cập nhật công trình</span>
                <span>Vừa xong</span>
              </div>
              <p class="leading-relaxed">
                Hoàn thiện bàn giao hệ thống cửa đi nhôm Xingfa 4 cánh mở quay &amp; phòng tắm kính cường lực tại Phường An Khê, TP Đà Nẵng. Cảm ơn Quý khách hàng đã tin tưởng <strong>phuoctratkc.com</strong>!
              </p>
              <div class="flex items-center justify-between pt-1 text-[11px] text-slate-500 border-t border-slate-200">
                <span><i class="fa-solid fa-thumbs-up text-[#1877F2] mr-1"></i>128 lượt thích</span>
                <a href="https://facebook.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-[#1877F2] hover:underline">Xem trên Facebook</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========================================================= -->
  <!-- PHẦN 12: FOOTER (CHUẨN FLATSOME) -->
  <!-- ========================================================= -->
  <footer class="bg-brand-900 text-slate-300 pt-10 pb-6 border-t-4 border-accent-500">
    <div class="tkc-container">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-7 pb-8 border-b border-white/10">

        <!-- Cột 1: Thông tin công ty -->
        <div class="space-y-3">
          <div class="flex items-center gap-2.5">
            <svg class="w-9 h-9 shrink-0" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect x="2" y="2" width="60" height="60" rx="12" fill="#0B3B66" stroke="#F59E0B" stroke-width="2" />
              <path d="M14 25L32 12L50 25" stroke="#F59E0B" stroke-width="3.2" stroke-linecap="round" stroke-linejoin="round" />
              <rect x="17" y="27" width="13" height="23" rx="2" fill="#FFFFFF" />
              <rect x="34" y="27" width="13" height="23" rx="2" fill="#F59E0B" />
            </svg>
            <div>
              <div class="text-sm font-extrabold text-white">PHƯỚC TRÀ <span class="text-accent-400">TKC</span></div>
              <div class="text-[10px] uppercase tracking-wider text-slate-400">phuoctratkc.com</div>
            </div>
          </div>
          <p class="text-xs font-bold text-white leading-snug">
            CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC
          </p>
          <ul class="space-y-2 text-xs text-slate-300 list-none m-0 p-0">
            <li class="flex items-start gap-2">
              <i class="fa-solid fa-location-dot text-accent-400 mt-0.5 shrink-0"></i>
              <span>365/12 Tôn Đản, Phường An Khê, TP Đà Nẵng</span>
            </li>
            <li class="flex items-center gap-2">
              <i class="fa-solid fa-phone text-accent-400 shrink-0"></i>
              <a href="tel:0905811246" class="hover:text-white font-semibold">Hotline: 0905.811.246</a>
            </li>
            <li class="flex items-center gap-2">
              <i class="fa-solid fa-globe text-accent-400 shrink-0"></i>
              <span>Website: phuoctratkc.com</span>
            </li>
          </ul>
        </div>

        <!-- Cột 2: Cửa nhôm xingfa -->
        <div>
          <h3 class="text-xs sm:text-sm font-bold uppercase tracking-wider text-white mb-3 pb-2 border-b border-white/10">
            Cửa Nhôm Xingfa
          </h3>
          <ul class="space-y-2 text-xs list-none m-0 p-0">
            <li><a href="#san-pham" onclick="filterProducts('xingfa', '1 cánh')" class="hover:text-accent-400 transition">Cửa nhôm xingfa 1 cánh</a></li>
            <li><a href="#san-pham" onclick="filterProducts('xingfa', '2 cánh')" class="hover:text-accent-400 transition">Cửa nhôm xingfa 2 cánh</a></li>
            <li><a href="#san-pham" onclick="filterProducts('xingfa', '3 cánh')" class="hover:text-accent-400 transition">Cửa nhôm xingfa 3 cánh</a></li>
            <li><a href="#san-pham" onclick="filterProducts('xingfa', '4 cánh')" class="hover:text-accent-400 transition">Cửa nhôm xingfa 4 cánh</a></li>
            <li><a href="#san-pham" onclick="filterProducts('xingfa', 'xếp trượt')" class="hover:text-accent-400 transition">Cửa nhôm xingfa 5 cánh / Xếp trượt</a></li>
          </ul>
        </div>

        <!-- Cột 3: Danh mục sản phẩm -->
        <div>
          <h3 class="text-xs sm:text-sm font-bold uppercase tracking-wider text-white mb-3 pb-2 border-b border-white/10">
            Danh Mục Sản Phẩm
          </h3>
          <ul class="space-y-2 text-xs list-none m-0 p-0">
            <li><a href="#san-pham" onclick="filterProducts('kinh-cuong-luc')" class="hover:text-accent-400 transition">Cửa kính cường lực Đà Nẵng</a></li>
            <li><a href="#san-pham" onclick="filterProducts('nhua-loi-thep')" class="hover:text-accent-400 transition">Cửa nhựa lõi thép uPVC</a></li>
            <li><a href="#san-pham" onclick="filterProducts('tu-dong')" class="hover:text-accent-400 transition">Cửa kính tự động</a></li>
            <li><a href="#san-pham" onclick="filterProducts('cau-thang-kinh')" class="hover:text-accent-400 transition">Cầu thang kính cường lực</a></li>
            <li><a href="#san-pham" onclick="filterProducts('kinh-op-bep')" class="hover:text-accent-400 transition">Kính ốp bếp &amp; Phòng tắm kính</a></li>
          </ul>
        </div>

        <!-- Cột 4: Liên kết nhanh -->
        <div>
          <h3 class="text-xs sm:text-sm font-bold uppercase tracking-wider text-white mb-3 pb-2 border-b border-white/10">
            Liên Kết Nhanh
          </h3>
          <ul class="space-y-2 text-xs list-none m-0 p-0">
            <li><a href="#gioi-thieu" class="hover:text-accent-400 transition">Giới thiệu Phước Trà TKC</a></li>
            <li><a href="#cong-trinh" class="hover:text-accent-400 transition">Công trình tiêu biểu tại Đà Nẵng</a></li>
            <li><a href="#bao-gia" class="hover:text-accent-400 transition">Bảng báo giá nhôm kính 2026</a></li>
            <li><a href="#tin-tuc" class="hover:text-accent-400 transition">Tin tức &amp; Tư vấn kỹ thuật</a></li>
            <li><a href="#form-bao-gia" class="hover:text-accent-400 transition">Yêu cầu khảo sát miễn phí</a></li>
          </ul>
        </div>
      </div>

      <div class="pt-5 flex flex-col sm:flex-row items-center justify-between gap-2 text-[11px] sm:text-xs text-slate-400 text-center sm:text-left">
        <div>Copyright 2026 &copy; <strong>CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC</strong> - phuoctratkc.com</div>
        <div>Thiết kế chuẩn Flatsome • Tối ưu di động &amp; máy tính</div>
      </div>
    </div>
  </footer>

  <!-- ========================================================= -->
  <!-- PHẦN 13: CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE) -->
  <!-- ========================================================= -->

  <!-- Hiển thị trên Máy tính & Tablet (nổi bên góc phải dưới, không tràn viền) -->
  <div class="hidden md:flex fixed right-4 bottom-5 z-40 flex-col gap-2.5">
    <a href="https://zalo.me/0905811246" target="_blank" rel="noopener noreferrer" class="group flex items-center gap-2.5 bg-[#0068FF] hover:bg-blue-600 text-white pl-3 pr-4 py-2.5 rounded-full shadow-lg transition transform hover:-translate-y-0.5" aria-label="Liên hệ Zalo 0905.811.246">
      <span class="w-7 h-7 rounded-full bg-white text-[#0068FF] font-extrabold text-[11px] flex items-center justify-center shrink-0">Zalo</span>
      <span class="text-xs font-bold whitespace-nowrap">Chat Zalo</span>
    </a>

    <a href="https://facebook.com" target="_blank" rel="noopener noreferrer" class="group flex items-center gap-2.5 bg-[#1877F2] hover:bg-blue-700 text-white pl-3 pr-4 py-2.5 rounded-full shadow-lg transition transform hover:-translate-y-0.5" aria-label="Liên hệ Facebook Phước Trà TKC">
      <span class="w-7 h-7 rounded-full bg-white text-[#1877F2] flex items-center justify-center shrink-0">
        <i class="fa-brands fa-facebook-f text-sm"></i>
      </span>
      <span class="text-xs font-bold whitespace-nowrap">Facebook</span>
    </a>

    <a href="tel:0905811246" class="pulse-ring flex items-center gap-2.5 bg-accent-500 hover:bg-accent-600 text-white pl-3 pr-4 py-2.5 rounded-full shadow-xl transition transform hover:-translate-y-0.5" aria-label="Gọi Hotline 0905.811.246">
      <span class="w-7 h-7 rounded-full bg-white text-accent-600 flex items-center justify-center shrink-0">
        <i class="fa-solid fa-phone-volume text-sm"></i>
      </span>
      <span class="text-xs font-extrabold whitespace-nowrap">0905.811.246</span>
    </a>
  </div>

  <!-- Hiển thị trên Điện thoại (thanh liên hệ cố định dưới đáy màn hình dễ bấm bằng ngón cái) -->
  <div class="md:hidden fixed bottom-0 left-0 right-0 z-40 bg-white border-t border-slate-200 shadow-[0_-4px_14px_rgba(15,23,42,0.08)] px-2 py-1.5">
    <div class="grid grid-cols-3 gap-1.5">
      <a href="tel:0905811246" class="flex items-center justify-center gap-1.5 bg-accent-500 active:bg-accent-600 text-white font-bold text-xs py-2.5 rounded-xl shadow-xs">
        <i class="fa-solid fa-phone-volume"></i>
        <span>Gọi Ngay</span>
      </a>
      <a href="https://zalo.me/0905811246" target="_blank" rel="noopener noreferrer" class="flex items-center justify-center gap-1.5 bg-[#0068FF] active:bg-blue-700 text-white font-bold text-xs py-2.5 rounded-xl shadow-xs">
        <span class="font-extrabold text-[11px] bg-white text-[#0068FF] px-1 rounded">Z</span>
        <span>Chat Zalo</span>
      </a>
      <a href="https://facebook.com" target="_blank" rel="noopener noreferrer" class="flex items-center justify-center gap-1.5 bg-[#1877F2] active:bg-blue-800 text-white font-bold text-xs py-2.5 rounded-xl shadow-xs">
        <i class="fa-brands fa-facebook-f"></i>
        <span>Facebook</span>
      </a>
    </div>
  </div>

  <!-- ========================================================= -->
  <!-- MODAL XEM NHANH SẢN PHẨM / DỰ ÁN / BÀI VIẾT / THÔNG BÁO -->
  <!-- ========================================================= -->
  <div id="detailModal" class="fixed inset-0 z-50 hidden items-center justify-center p-3 sm:p-5 bg-slate-900/65 backdrop-blur-xs" onclick="closeModal(event)">
    <div class="bg-white rounded-2xl max-w-2xl w-full max-h-[90vh] overflow-y-auto shadow-2xl border border-slate-200 relative" onclick="event.stopPropagation()">
      <button type="button" onclick="forceCloseModal()" class="absolute top-3 right-3 z-10 w-8 h-8 rounded-full bg-slate-100 hover:bg-red-50 hover:text-red-600 text-slate-600 flex items-center justify-center transition" aria-label="Đóng cửa sổ">
        <i class="fa-solid fa-xmark"></i>
      </button>
      <div id="detailModalBody" class="p-5 sm:p-6"></div>
    </div>
  </div>

  <!-- ========================================================= -->
  <!-- JAVASCRIPT XỬ LÝ TƯƠNG TÁC, SLIDER, LỌC SẢN PHẨM, FORM -->
  <!-- ========================================================= -->
  <script>
    /**
     * Hàm xử lý fallback khi tải ảnh Google Drive (thử lh3.googleusercontent trước khi dùng placeholder)
     */
    function handleImgError(img, driveId, label) {
      if (!img.dataset.fallbackStep) {
        img.dataset.fallbackStep = '1';
        img.src = 'https://lh3.googleusercontent.com/d/' + driveId;
      } else if (img.dataset.fallbackStep === '1') {
        img.dataset.fallbackStep = '2';
        img.src = 'https://placehold.co/800x600/0B3B66/FFFFFF?text=' + encodeURIComponent(label || 'Phuoc Tra TKC');
      }
    }

    /**
     * Định dạng tiền tệ VNĐ
     */
    function formatVND(amount) {
      return amount.toString().replace(/\B(?=(\d{3})+(?!\d))/g, '.') + ' ₫';
    }

    /**
     * Danh sách sản phẩm chuẩn thực tế kèm mã ảnh Google Drive, giá gốc, giá ưu đãi và % giảm giá
     */
    const PRODUCTS = [
      {
        id: 'p1',
        name: 'Cửa đi quay mở 1 cánh nhôm xingfa',
        category: 'xingfa',
        subTag: '1 cánh',
        driveId: '1-0eBWGjPwzQ-C9c1Wjws9wt0gbsulkPm',
        oldPrice: 2450000,
        price: 2100000,
        discount: 14,
        specs: 'Nhôm Xingfa nhập khẩu tem đỏ hệ 55, độ dày 2.0mm, kính an toàn 6.38mm hoặc cường lực 8mm, phụ kiện Kinlong đồng bộ.'
      },
      {
        id: 'p2',
        name: 'Cửa đi quay mở 2 cánh nhôm xingfa',
        category: 'xingfa',
        subTag: '2 cánh',
        driveId: '1h2r2rbPrEL7dgLE-MiE5lBBuE8gFNehb',
        oldPrice: 2400000,
        price: 2100000,
        discount: 13,
        specs: 'Nhôm Xingfa Quảng Đông hệ 55 dày 2.0mm, kết cấu khoang rỗng gân gia cường, kín khít tuyệt đối với gioăng EPDM.'
      },
      {
        id: 'p3',
        name: 'Cửa đi quay mở 3 cánh nhôm xingfa',
        category: 'xingfa',
        subTag: '3 cánh',
        driveId: '17Qi2D8ntACnVrTeRPZ2V7rC0FmI8ecaR',
        oldPrice: 2500000,
        price: 2100000,
        discount: 16,
        specs: 'Thiết kế mở rộng tối đa không gian mặt tiền, công nghệ ép góc tự động CNC, sơn tĩnh điện ngoài trời bền màu.'
      },
      {
        id: 'p4',
        name: 'Cửa đi quay mở 4 cánh nhôm xingfa',
        category: 'xingfa',
        subTag: '4 cánh',
        driveId: '1lxzMKWX3e_HJn7UELFZDOURuxh-NYZg-',
        oldPrice: 2450000,
        price: 2100000,
        discount: 14,
        specs: 'Giải pháp hoàn hảo cho cửa chính nhà phố và biệt thự. Chịu lực gió bão miền Trung cực tốt, cách âm cách nhiệt cao.'
      },
      {
        id: 'p5',
        name: 'Cửa Nhôm Xingfa Cửa Đi Xếp Trượt',
        category: 'xingfa',
        subTag: 'xếp trượt',
        driveId: '1lJpUJBpR_cJp8mIaZ4FnRTynQ_-paNwZ',
        oldPrice: 2550000,
        price: 2100000,
        discount: 18,
        specs: 'Nhôm Xingfa hệ 63 xếp gấp 4 - 5 - 6 cánh linh hoạt, vận hành êm ái trên ray trượt hợp kim cao cấp.'
      },
      {
        id: 'p6',
        name: 'Cửa sổ mở hất 2 cánh nhôm Xingfa',
        category: 'xingfa',
        subTag: '2 cánh',
        driveId: '11fS_oEeJtnDICQZ77fJlYl6GhHf-GOhA',
        oldPrice: 2350000,
        price: 2050000,
        discount: 13,
        specs: 'Nhôm hệ 55 dày 1.4mm, định vị góc mở tối đa 45 độ chống hắt mưa và chịu áp lực gió giật an toàn.'
      },
      {
        id: 'p7',
        name: 'Cửa kính cường lực mở quay bản lề sàn',
        category: 'kinh-cuong-luc',
        subTag: 'kính cường lực',
        driveId: '1PIFP1UCQs_FIaKCgGwcJWt-5wTnST9iJ',
        oldPrice: 1050000,
        price: 890000,
        discount: 15,
        specs: 'Kính cường lực 10mm - 12mm tiêu chuẩn an toàn, phụ kiện bản lề thủy lực VVP Thái Lan / Hafele đóng mở êm ái.'
      },
      {
        id: 'p8',
        name: 'Cửa nhựa lõi thép uPVC cách âm cao cấp',
        category: 'nhua-loi-thep',
        subTag: 'nhựa lõi thép',
        driveId: '1jiHBW-2MoWUHjQUicSe-rO6NlmfNuZNA',
        oldPrice: 1850000,
        price: 1590000,
        discount: 14,
        specs: 'Thanh profile uPVC lõi thép mạ kẽm gia cường dày 1.4mm, khả năng cách âm và cách nhiệt vượt trội cho phòng ngủ.'
      },
      {
        id: 'p9',
        name: 'Cửa kính trượt tự động cảm biến radar',
        category: 'tu-dong',
        subTag: 'tự động',
        driveId: '1PIFP1UCQs_FIaKCgGwcJWt-5wTnST9iJ',
        oldPrice: 28500000,
        price: 24500000,
        discount: 14,
        specs: 'Hệ thống motor cảm biến tự động nhập khẩu Hàn Quốc / Nhật Bản, kèm mắt thần an toàn hồng ngoại cho showroom, khách sạn.'
      },
      {
        id: 'p10',
        name: 'Cầu thang kính cường lực tay vịn gỗ',
        category: 'cau-thang-kinh',
        subTag: 'cầu thang',
        driveId: '1FnuITlKMjk-xTxkIV96ABv43S1PG--Ul',
        oldPrice: 1450000,
        price: 1250000,
        discount: 14,
        specs: 'Kính cường lực 10mm - 12mm kết hợp trụ Inox 304 chống gỉ và tay vịn gỗ tự nhiên sang trọng, mở rộng ánh sáng không gian.'
      },
      {
        id: 'p11',
        name: 'Kính ốp bếp cường lực sơn màu chịu nhiệt',
        category: 'kinh-op-bep',
        subTag: 'kính bếp',
        driveId: '1ilanOshTrs9llnMXWl5iZ8DtgptJ0hCb',
        oldPrice: 950000,
        price: 790000,
        discount: 17,
        specs: 'Kính cường lực 8mm sơn màu chịu nhiệt đa dạng tông màu, bề mặt liền mạch chống bám dầu mỡ, cực kỳ dễ lau chùi.'
      },
      {
        id: 'p12',
        name: 'Phòng tắm kính cường lực vách ngăn 10mm',
        category: 'phong-tam-kinh',
        subTag: 'phòng tắm',
        driveId: '1MhCILHQ5goD1cAPTt1hZsY_ajeOMs-qH',
        oldPrice: 1350000,
        price: 1150000,
        discount: 15,
        specs: 'Vách kính cường lực 10mm phụ kiện Inox 304 bóng gương, ngăn nước tuyệt đối giữ phòng tắm luôn khô ráo sạch sẽ.'
      }
    ];

    /**
     * Danh sách 6 dự án Đà Nẵng thực tế theo yêu cầu
     */
    const PROJECTS = [
      {
        title: 'DỰ ÁN RESORT MỸ SƠN 4 SAO “MY SON HERITAGE RESORT & SPA”',
        driveId: '1MmAfsyp3s3YCaEMymrkk8TZbD38jCsAQ',
        location: 'Quảng Nam - Đà Nẵng',
        scope: 'Thi công trọn gói hệ thống cửa nhôm Xingfa nhập khẩu, vách kính mặt dựng và phòng tắm kính cao cấp tiêu chuẩn 4 sao.'
      },
      {
        title: 'THI CÔNG DỰ ÁN KHÁCH SẠN GODEN LINE',
        driveId: '1YeuDLiSXUK_Epupq9QiGzM90_EGW3Kfy',
        location: 'TP Đà Nẵng',
        scope: 'Cung cấp và lắp đặt cửa đi ban công nhôm Xingfa hệ 55 chống ồn, vách kính cường lực và lan can kính an toàn.'
      },
      {
        title: 'DỰ ÁN KHÁCH SẠN RUBY LIGHT',
        driveId: '1wH-JJ2rOYRmDGsNapl3bIBjfiG3Qm6zZ',
        location: 'TP Đà Nẵng',
        scope: 'Hạng mục cửa kính tự động sảnh chính, cửa sổ nhôm Xingfa chống bão và hệ phòng tắm kính đồng bộ.'
      },
      {
        title: 'THI CÔNG DỰ ÁN RAON ĐÀ NẴNG BEACH HOTEL',
        driveId: '1za_IJpAm850uulT6IuhBsk1THb3LuPuc',
        location: 'Ven biển Mỹ Khê, TP Đà Nẵng',
        scope: 'Thi công cửa nhôm kính chuyên dụng kháng muối biển, kính hộp cách âm và hệ cửa kính cường lực toàn khách sạn.'
      },
      {
        title: 'THI CÔNG DỰ ÁN KHÁCH SẠN JOLIA',
        driveId: '1WRgx-EUIrn8IKFZdpmdv6Z2Xyb7L8_64',
        location: 'TP Đà Nẵng',
        scope: 'Lắp đặt đồng bộ hệ cửa nhôm Xingfa tem đỏ Quảng Đông, phụ kiện Kinlong chính hãng và kính cường lực 10mm.'
      },
      {
        title: 'THI CÔNG DỰ ÁN KHÁCH SẠN SOHO',
        driveId: '1-C5bdt4K-PpLX_KqSN6QAR5ULo1WnNzt',
        location: 'TP Đà Nẵng',
        scope: 'Thiết kế và thi công toàn bộ hệ mặt dựng nhôm kính, cửa ra vào kính cường lực bản lề sàn và vách tắm kính.'
      }
    ];

    /**
     * Danh sách bài viết trang chủ (kèm danh mục bài viết)
     */
    const ARTICLES = [
      {
        id: 'a1',
        cat: 'tu-van',
        catLabel: 'Tư vấn cửa nhôm',
        date: '18/11/2026',
        title: 'Cửa nhôm Xingfa có phù hợp với khí hậu mưa bão miền Trung không?',
        driveId: '1zRlHJBAneXS7EQ1jdT__hVRCTf2mzOiX',
        excerpt: 'Nhờ kết cấu khoang rỗng kết hợp 2 đường gân gia cường cùng hệ gioăng EPDM kín khít, cửa nhôm Xingfa chịu lực gió cực tốt tại Đà Nẵng.',
        content: 'Tại khu vực Đà Nẵng và Miền Trung thường xuyên chịu ảnh hưởng của nắng nóng gay gắt và gió bão ven biển, cửa nhôm Xingfa nhập khẩu tem đỏ Quảng Đông là giải pháp tối ưu. Bề mặt thanh nhôm được xử lý sơn tĩnh điện ngoài trời chống oxy hóa, kết hợp công nghệ ép góc tự động giúp bộ cửa cứng cáp, chống nước thấm tuyệt đối và giữ màu bền bỉ hàng chục năm.'
      },
      {
        id: 'a2',
        cat: 'ky-thuat',
        catLabel: 'Kỹ thuật thi công',
        date: '12/11/2026',
        title: 'Phân biệt các hệ nhôm Xingfa 55, 63, 93 để chọn đúng cho từng vị trí cửa',
        driveId: '1lJpUJBpR_cJp8mIaZ4FnRTynQ_-paNwZ',
        excerpt: 'Mỗi quy cách mở quay, mở lùa hay xếp trượt đều sử dụng hệ profile nhôm Xingfa chuyên biệt để đảm bảo độ bền và vận hành êm ái.',
        content: 'Nhôm Xingfa hệ 55 (dày 1.4mm cho cửa sổ và 2.0mm cho cửa đi) chuyên dùng cho cửa mở quay và mở hất. Hệ 93 được thiết kế tối ưu cho cửa mở trượt lùa tiết kiệm diện tích. Hệ 63 dùng cho cửa đi xếp trượt gấp nhiều cánh giúp mở rộng tối đa tầm nhìn ra sân vườn hoặc ban công.'
      },
      {
        id: 'a3',
        cat: 'bao-gia-tin',
        catLabel: 'Kinh nghiệm báo giá',
        date: '05/11/2026',
        title: 'Cách tính giá 1 bộ cửa nhôm Xingfa chính hãng trọn gói tại Đà Nẵng',
        driveId: '1lxzMKWX3e_HJn7UELFZDOURuxh-NYZg-',
        excerpt: 'Hướng dẫn công thức tính chi phí theo diện tích m² kính nhôm kết hợp bộ phụ kiện đồng bộ giúp chủ nhà dự trù ngân sách chuẩn xác.',
        content: 'Công thức chuẩn: Tổng giá trị bộ cửa = (Diện tích cửa m² x Đơn giá hệ nhôm kính) + Đơn giá bộ phụ kiện đồng bộ (bản lề, khóa đa điểm, tay nắm). Tại Phước Trà TKC, khách hàng được khảo sát đo đạc thực tế miễn phí và nhận bảng dự toán chi tiết từng hạng mục trước khi ký hợp đồng.'
      },
      {
        id: 'a4',
        cat: 'ky-thuat',
        catLabel: 'Kỹ thuật thi công',
        date: '29/10/2026',
        title: 'Lưu ý quan trọng khi lắp đặt phòng tắm kính và kính ốp bếp cường lực',
        driveId: '1MhCILHQ5goD1cAPTt1hZsY_ajeOMs-qH',
        excerpt: 'Chọn độ dày kính 8mm - 10mm đạt chuẩn cùng phụ kiện Inox 304 chống gỉ sét sẽ giúp không gian nội thất luôn sáng đẹp và an toàn.',
        content: 'Đối với phòng tắm kính, nên sử dụng kính cường lực dày 10mm kết hợp phụ kiện Inox 304 chính hãng và gioăng từ chắn nước kín khít. Đối với kính ốp bếp, kính cường lực 8mm sơn màu chịu nhiệt giúp chống bám dầu mỡ, chịu sốc nhiệt khu vực bếp nấu và dễ dàng vệ sinh hàng ngày.'
      }
    ];

    /**
     * Render danh sách sản phẩm (đảm bảo 2 cột trên mobile, giá + giảm % góc trên trái, tên sản phẩm hiển thị đủ 100%)
     */
    function renderProducts(category = 'all', keyword = '') {
      const grid = document.getElementById('productGrid');
      if (!grid) return;

      const filtered = PRODUCTS.filter((p) => {
        const matchCat = category === 'all' || p.category === category;
        const matchKey = !keyword || p.name.toLowerCase().includes(keyword.toLowerCase()) || p.subTag.toLowerCase().includes(keyword.toLowerCase());
        return matchCat && matchKey;
      });

      const listToShow = filtered.length > 0 ? filtered : PRODUCTS;

      grid.innerHTML = listToShow.map((p) => `
        <article class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-lg hover:border-brand-600/50 transition flex flex-col">
          <div class="relative aspect-[4/3] bg-slate-100 overflow-hidden cursor-pointer" onclick="openProductModal('${p.id}')">
            <!-- Giảm giá % góc trên bên trái sản phẩm -->
            <span class="absolute top-2 left-2 z-10 bg-red-600 text-white text-[10px] sm:text-xs font-extrabold px-2 py-0.5 rounded-md shadow-sm">
              -${p.discount}%
            </span>
            <img
              src="https://drive.google.com/thumbnail?id=${p.driveId}&sz=w800"
              alt="${p.name}"
              loading="lazy"
              class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
              onerror="handleImgError(this, '${p.driveId}', '${p.name.replace(/'/g, '')}')"
            />
          </div>

          <div class="p-2.5 sm:p-3.5 flex-1 flex flex-col justify-between gap-2">
            <!-- Tên sản phẩm đầy đủ, không cắt chữ, không tràn viền trên 2 cột mobile -->
            <h3 onclick="openProductModal('${p.id}')" class="text-[12px] sm:text-sm font-bold text-slate-800 group-hover:text-brand-700 leading-snug break-words cursor-pointer transition">
              ${p.name}
            </h3>

            <div class="space-y-2">
              <div class="flex flex-wrap items-baseline gap-x-2 gap-y-0.5">
                <span class="text-xs sm:text-[15px] font-extrabold text-red-600">${formatVND(p.price)}</span>
                <span class="text-[10px] sm:text-xs text-slate-400 line-through">${formatVND(p.oldPrice)}</span>
              </div>

              <div class="grid grid-cols-2 gap-1.5">
                <button type="button" onclick="openProductModal('${p.id}')" class="py-1.5 px-2 rounded-lg border border-brand-700 text-brand-700 hover:bg-brand-50 text-[10px] sm:text-xs font-bold transition cursor-pointer">
                  Xem nhanh
                </button>
                <a href="#form-bao-gia" onclick="prefillQuote('${p.name.replace(/'/g, '')}')" class="py-1.5 px-2 rounded-lg bg-brand-700 hover:bg-accent-500 text-white text-[10px] sm:text-xs font-bold text-center transition">
                  Báo giá
                </a>
              </div>
            </div>
          </div>
        </article>
      `).join('');
    }

    /**
     * Lọc sản phẩm theo danh mục & đồng bộ trạng thái nút tab
     */
    function filterProducts(category, keyword = '') {
      renderProducts(category, keyword);
      document.querySelectorAll('.filter-tab').forEach((btn) => {
        const isActive = btn.dataset.cat === category;
        btn.className = isActive
          ? 'filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-brand-700 text-white transition cursor-pointer'
          : 'filter-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-slate-100 text-slate-700 hover:bg-brand-50 hover:text-brand-700 transition cursor-pointer';
      });
    }

    /**
     * Render 6 dự án Đà Nẵng
     */
    function renderProjects() {
      const grid = document.getElementById('projectGrid');
      if (!grid) return;

      grid.innerHTML = PROJECTS.map((proj, idx) => `
        <article onclick="openProjectModal(${idx})" class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-lg transition cursor-pointer flex flex-col">
          <div class="aspect-[16/10] bg-slate-100 overflow-hidden">
            <img
              src="https://drive.google.com/thumbnail?id=${proj.driveId}&sz=w900"
              alt="${proj.title}"
              loading="lazy"
              class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
              onerror="handleImgError(this, '${proj.driveId}', 'Du An Da Nang')"
            />
          </div>
          <div class="p-3 sm:p-4 flex-1 flex flex-col justify-between gap-1.5">
            <h3 class="text-[11.5px] sm:text-sm font-bold text-brand-700 group-hover:text-accent-600 leading-snug break-words transition">
              ${proj.title}
            </h3>
            <div class="text-[10.5px] sm:text-xs text-slate-500 flex items-center gap-1">
              <i class="fa-solid fa-location-dot text-accent-500"></i>
              <span>${proj.location}</span>
            </div>
          </div>
        </article>
      `).join('');
    }

    /**
     * Render bài viết trang chủ theo danh mục
     */
    function renderArticles(cat = 'all') {
      const grid = document.getElementById('articleGrid');
      if (!grid) return;
      const list = cat === 'all' ? ARTICLES : ARTICLES.filter((a) => a.cat === cat);

      grid.innerHTML = list.map((art) => `
        <article onclick="openArticleModal('${art.id}')" class="group bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md transition cursor-pointer flex flex-col">
          <div class="aspect-[16/10] bg-slate-100 overflow-hidden">
            <img
              src="https://drive.google.com/thumbnail?id=${art.driveId}&sz=w700"
              alt="${art.title}"
              loading="lazy"
              class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
              onerror="handleImgError(this, '${art.driveId}', 'Tin Tuc Phuoc Tra TKC')"
            />
          </div>
          <div class="p-3.5 flex-1 flex flex-col justify-between gap-2">
            <div class="space-y-1.5">
              <div class="flex items-center justify-between text-[11px] text-slate-500">
                <span class="font-semibold text-accent-600">${art.catLabel}</span>
                <span>${art.date}</span>
              </div>
              <h3 class="text-xs sm:text-sm font-bold text-slate-800 group-hover:text-brand-700 leading-snug transition">
                ${art.title}
              </h3>
              <p class="text-xs text-slate-600 leading-relaxed">${art.excerpt}</p>
            </div>
            <span class="text-xs font-bold text-brand-700 group-hover:text-accent-600 inline-flex items-center gap-1 pt-1">
              Xem chi tiết <i class="fa-solid fa-arrow-right text-[10px]"></i>
            </span>
          </div>
        </article>
      `).join('');
    }

    function filterArticles(cat, clickedBtn) {
      renderArticles(cat);
      document.querySelectorAll('.article-tab').forEach((btn) => {
        btn.className = 'article-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-white border border-slate-200 text-slate-700 hover:bg-brand-50 transition cursor-pointer';
      });
      if (clickedBtn) {
        clickedBtn.className = 'article-tab px-3 py-1.5 rounded-lg text-[11px] sm:text-xs font-semibold bg-brand-700 text-white transition cursor-pointer';
      }
    }

    /**
     * Điền sẵn tên sản phẩm vào form báo giá
     */
    function prefillQuote(productName) {
      const noteEl = document.getElementById('qNote');
      if (noteEl) {
        noteEl.value = 'Tôi cần tư vấn và nhận báo giá cho sản phẩm: ' + productName;
      }
    }

    /**
     * Modal xem nhanh sản phẩm, dự án, bài viết
     */
    function showModalContent(html) {
      const modal = document.getElementById('detailModal');
      const body = document.getElementById('detailModalBody');
      body.innerHTML = html;
      modal.classList.remove('hidden');
      modal.classList.add('flex');
      document.body.style.overflow = 'hidden';
    }

    function closeModal(event) {
      if (event.target.id === 'detailModal') {
        forceCloseModal();
      }
    }

    function forceCloseModal() {
      const modal = document.getElementById('detailModal');
      modal.classList.add('hidden');
      modal.classList.remove('flex');
      document.body.style.overflow = '';
    }

    function openProductModal(id) {
      const p = PRODUCTS.find((item) => item.id === id);
      if (!p) return;
      showModalContent(`
        <div class="grid grid-cols-1 sm:grid-cols-2 gap-5 items-start">
          <div class="relative rounded-xl overflow-hidden bg-slate-100 border border-slate-200 aspect-[4/3]">
            <span class="absolute top-2.5 left-2.5 bg-red-600 text-white text-xs font-extrabold px-2.5 py-0.5 rounded-md">-${p.discount}%</span>
            <img src="https://drive.google.com/thumbnail?id=${p.driveId}&sz=w900" alt="${p.name}" class="w-full h-full object-cover" onerror="handleImgError(this, '${p.driveId}', '${p.name.replace(/'/g, '')}')" />
          </div>
          <div class="space-y-3">
            <h3 class="text-base sm:text-lg font-extrabold text-brand-700 leading-snug">${p.name}</h3>
            <div class="flex items-baseline gap-2.5">
              <span class="text-xl font-extrabold text-red-600">${formatVND(p.price)}</span>
              <span class="text-sm text-slate-400 line-through">${formatVND(p.oldPrice)}</span>
            </div>
            <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">${p.specs}</p>
            <div class="text-xs text-slate-600 bg-slate-50 p-3 rounded-xl border border-slate-200 space-y-1">
              <div><strong>Đơn vị thi công:</strong> CÔNG TY TNHH ĐẦU TƯ XÂY DỰNG PHƯỚC TRÀ TKC</div>
              <div><strong>Khu vực:</strong> Đà Nẵng &amp; các tỉnh Miền Trung</div>
              <div><strong>Hotline tư vấn:</strong> <a href="tel:0905811246" class="font-bold text-brand-700">0905.811.246</a></div>
            </div>
            <div class="flex flex-wrap gap-2 pt-1">
              <a href="#form-bao-gia" onclick="prefillQuote('${p.name.replace(/'/g, '')}'); forceCloseModal()" class="flex-1 text-center bg-accent-500 hover:bg-accent-600 text-white font-bold text-xs sm:text-sm py-2.5 px-4 rounded-xl transition">Yêu cầu báo giá</a>
              <a href="tel:0905811246" class="flex-1 text-center bg-brand-700 hover:bg-brand-800 text-white font-bold text-xs sm:text-sm py-2.5 px-4 rounded-xl transition">Gọi 0905.811.246</a>
            </div>
          </div>
        </div>
      `);
    }

    function openProjectModal(index) {
      const proj = PROJECTS[index];
      if (!proj) return;
      showModalContent(`
        <div class="space-y-4">
          <div class="rounded-xl overflow-hidden bg-slate-100 aspect-[16/10] border border-slate-200">
            <img src="https://drive.google.com/thumbnail?id=${proj.driveId}&sz=w1000" alt="${proj.title}" class="w-full h-full object-cover" onerror="handleImgError(this, '${proj.driveId}', 'Du An Da Nang')" />
          </div>
          <div class="space-y-2">
            <div class="text-xs font-bold text-accent-600 uppercase"><i class="fa-solid fa-location-dot mr-1"></i>${proj.location}</div>
            <h3 class="text-base sm:text-xl font-extrabold text-brand-700 leading-snug">${proj.title}</h3>
            <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">${proj.scope}</p>
          </div>
          <div class="pt-2 flex flex-wrap gap-2">
            <a href="#form-bao-gia" onclick="prefillQuote('Tư vấn hạng mục tương tự ${proj.title.replace(/'/g, '')}'); forceCloseModal()" class="bg-brand-700 hover:bg-brand-800 text-white text-xs sm:text-sm font-bold px-5 py-2.5 rounded-xl transition">Nhận tư vấn công trình</a>
            <a href="tel:0905811246" class="bg-accent-500 hover:bg-accent-600 text-white text-xs sm:text-sm font-bold px-5 py-2.5 rounded-xl transition">Hotline: 0905.811.246</a>
          </div>
        </div>
      `);
    }

    function openArticleModal(id) {
      const art = ARTICLES.find((a) => a.id === id);
      if (!art) return;
      showModalContent(`
        <div class="space-y-4">
          <div class="rounded-xl overflow-hidden bg-slate-100 aspect-[16/9]">
            <img src="https://drive.google.com/thumbnail?id=${art.driveId}&sz=w900" alt="${art.title}" class="w-full h-full object-cover" onerror="handleImgError(this, '${art.driveId}', 'Tin Tuc')" />
          </div>
          <div class="flex items-center gap-3 text-xs text-slate-500">
            <span class="font-bold text-accent-600">${art.catLabel}</span>
            <span>&bull;</span>
            <span>${art.date}</span>
          </div>
          <h3 class="text-base sm:text-xl font-extrabold text-brand-700 leading-snug">${art.title}</h3>
          <p class="text-xs sm:text-sm text-slate-700 leading-relaxed">${art.content}</p>
          <div class="pt-2 border-t border-slate-200 flex items-center justify-between gap-3">
            <span class="text-xs text-slate-500">Nguồn: <strong>phuoctratkc.com</strong></span>
            <a href="#form-bao-gia" onclick="forceCloseModal()" class="text-xs font-bold text-brand-700 hover:text-accent-600">Nhận báo giá miễn phí &rarr;</a>
          </div>
        </div>
      `);
    }

    /**
     * Xử lý Banner tự trượt chuyên nghiệp (2 slide kích thước bằng nhau + hỗ trợ vuốt cảm ứng)
     */
    let currentSlide = 0;
    const totalSlides = 2;
    let sliderTimer = null;

    function updateSlider() {
      const slides = document.querySelectorAll('.hero-slide');
      const dots = document.querySelectorAll('.hero-dot');
      slides.forEach((slide, index) => {
        if (index === currentSlide) {
          slide.classList.add('is-active');
          slide.classList.remove('is-inactive');
        } else {
          slide.classList.remove('is-active');
          slide.classList.add('is-inactive');
        }
      });
      dots.forEach((dot, index) => {
        if (index === currentSlide) {
          dot.className = 'hero-dot w-6 h-2 rounded-full bg-accent-400 transition-all cursor-pointer';
        } else {
          dot.className = 'hero-dot w-2.5 h-2 rounded-full bg-white/45 hover:bg-white/80 transition-all cursor-pointer';
        }
      });
    }

    function nextSlide() {
      currentSlide = (currentSlide + 1) % totalSlides;
      updateSlider();
      resetSliderTimer();
    }

    function prevSlide() {
      currentSlide = (currentSlide - 1 + totalSlides) % totalSlides;
      updateSlider();
      resetSliderTimer();
    }

    function goToSlide(index) {
      currentSlide = index;
      updateSlider();
      resetSliderTimer();
    }

    function resetSliderTimer() {
      if (sliderTimer) clearInterval(sliderTimer);
      sliderTimer = setInterval(() => {
        currentSlide = (currentSlide + 1) % totalSlides;
        updateSlider();
      }, 5500);
    }

    /**
     * Điều khiển Drawer menu di động
     */
    function openMobileMenu() {
      const backdrop = document.getElementById('mobileDrawerBackdrop');
      const drawer = document.getElementById('mobileDrawer');
      backdrop.classList.remove('hidden');
      requestAnimationFrame(() => {
        backdrop.classList.remove('opacity-0');
        drawer.classList.remove('-translate-x-full');
      });
      document.body.style.overflow = 'hidden';
    }

    function closeMobileMenu() {
      const backdrop = document.getElementById('mobileDrawerBackdrop');
      const drawer = document.getElementById('mobileDrawer');
      backdrop.classList.add('opacity-0');
      drawer.classList.add('-translate-x-full');
      setTimeout(() => {
        backdrop.classList.add('hidden');
      }, 280);
      document.body.style.overflow = '';
    }

    function toggleSubmenu(subId, btn) {
      const el = document.getElementById(subId);
      const icon = btn.querySelector('i');
      if (!el) return;
      el.classList.toggle('hidden');
      if (icon) icon.classList.toggle('rotate-180');
    }

    /**
     * Khởi tạo toàn bộ sự kiện khi trang tải xong
     */
    window.addEventListener('DOMContentLoaded', () => {
      renderProducts('all');
      renderProjects();
      renderArticles('all');
      resetSliderTimer();

      const mobileBtn = document.getElementById('mobileMenuBtn');
      if (mobileBtn) mobileBtn.addEventListener('click', openMobileMenu);

      // Hỗ trợ vuốt cảm ứng trái/phải trên banner điện thoại
      const sliderEl = document.getElementById('heroSlider');
      if (sliderEl) {
        let touchStartX = 0;
        sliderEl.addEventListener('touchstart', (e) => {
          touchStartX = e.changedTouches[0].screenX;
        }, { passive: true });
        sliderEl.addEventListener('touchend', (e) => {
          const diff = e.changedTouches[0].screenX - touchStartX;
          if (Math.abs(diff) > 45) {
            if (diff < 0) nextSlide();
            else prevSlide();
          }
        }, { passive: true });
      }

      // Xử lý gửi form yêu cầu & báo giá (không sử dụng alert())
      const quoteForm = document.getElementById('quoteForm');
      if (quoteForm) {
        quoteForm.addEventListener('submit', (e) => {
          e.preventDefault();
          const name = document.getElementById('qName').value.trim();
          const phone = document.getElementById('qPhone').value.trim();
          const service = document.getElementById('qService').value;

          showModalContent(`
            <div class="text-center py-4 space-y-3">
              <div class="w-14 h-14 mx-auto rounded-full bg-emerald-100 text-emerald-600 flex items-center justify-center text-2xl">
                <i class="fa-solid fa-check"></i>
              </div>
              <h3 class="text-lg font-extrabold text-brand-700">Đã Tiếp Nhận Yêu Cầu Báo Giá!</h3>
              <p class="text-sm text-slate-600 leading-relaxed">
                Cảm ơn Quý khách <strong>${name}</strong>. Đội ngũ <strong>PHƯỚC TRÀ TKC</strong> đã nhận thông tin quan tâm hạng mục <strong>${service}</strong> và sẽ liên hệ lại số <strong>${phone}</strong> trong ít phút tới.
              </p>
              <div class="pt-2">
                <button type="button" onclick="forceCloseModal()" class="bg-brand-700 hover:bg-brand-800 text-white font-bold text-sm px-6 py-2.5 rounded-xl transition cursor-pointer">
                  Đóng thông báo
                </button>
              </div>
            </div>
          `);
          quoteForm.reset();
        });
      }
    });
  </script>
</body>
</html>
