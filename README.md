<!doctype html>
<html lang="pt-BR">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Rodrigo Bina — Designer Multimídia</title>
    <meta name="description" content="Portfólio de Rodrigo Bina — Design, Branding e Social Media." />

    <!-- Tailwind CSS via CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
      tailwind.config = {
        theme: {
          extend: {
            fontFamily: {
              inter: ["Inter", "ui-sans-serif", "system-ui", "-apple-system"],
            },
            colors: {
              base: {
                900: "#0a0a0b",
                800: "#111113",
                700: "#1a1a1e",
              },
              accent: {
                500: "#ffffff",
                400: "#d1d1d6",
                300: "#9ca3af",
                200: "#6b7280",
              },
            },
            boxShadow: {
              soft: "0 10px 30px rgba(0,0,0,.35)",
            },
            backdropBlur: {
              xs: '2px'
            }
          }
        }
      }
    </script>

    <!-- Inter font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

    <style>
      /* Big smooth underline for active nav */
      .nav-link { position: relative; }
      .nav-link.active::after { content: ""; position: absolute; left: 0; bottom: -6px; height: 2px; width: 100%; background: white; border-radius: 2px; }
      /* Glassy card edge highlight */
      .card-glow { box-shadow: inset 0 0 0 1px rgba(255,255,255,.06), 0 20px 50px rgba(0,0,0,.5); }
      /* Organic blob background */
      .blob {
        position: absolute; inset: -10% -20% auto auto; width: 58vw; height: 58vw; max-width: 880px; max-height: 880px; border-radius: 9999px;
        background: radial-gradient(55% 55% at 50% 50%, rgba(255,255,255,.12), rgba(20,20,24,.0) 60%),
                    radial-gradient(45% 45% at 30% 30%, rgba(255,255,255,.08), rgba(0,0,0,0) 60%),
                    radial-gradient(35% 35% at 70% 70%, rgba(255,255,255,.06), rgba(0,0,0,0) 60%);
        filter: blur(20px) saturate(120%);
        transform: translate3d(0,0,0);
      }
      .section { scroll-margin-top: 96px; }
      html { scroll-behavior: smooth; }
    </style>
  </head>

  <body class="min-h-screen bg-base-900 text-white font-inter antialiased">
    <!-- Social vertical (right) -->
    <aside class="hidden md:flex fixed right-4 top-1/2 -translate-y-1/2 z-40 flex-col items-center gap-4">
      <a aria-label="Instagram" href="#" class="p-3 rounded-full bg-base-800 hover:bg-white/10 transition shadow-soft" title="Instagram">
        <!-- Instagram icon -->
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" class="w-5 h-5"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg>
      </a>
      <a aria-label="LinkedIn" href="#" class="p-3 rounded-full bg-base-800 hover:bg-white/10 transition shadow-soft" title="LinkedIn">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-5 h-5" fill="currentColor"><path d="M4.98 3.5C4.98 4.88 3.86 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1s2.48 1.12 2.48 2.5zM.5 8h4V24h-4V8zm7.5 0h3.8v2.2h.05c.53-1 1.83-2.2 3.77-2.2 4.03 0 4.78 2.65 4.78 6.1V24h-4V15.2c0-2.1-.04-4.8-2.92-4.8-2.92 0-3.36 2.28-3.36 4.64V24h-4V8z"/></svg>
      </a>
      <a aria-label="WhatsApp" href="#" class="p-3 rounded-full bg-base-800 hover:bg-white/10 transition shadow-soft" title="WhatsApp">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" class="w-5 h-5 fill-current"><path d="M380.9 97.1C339 55.1 283.2 32 223.9 32 103.5 32 5 130.5 5 250.9c0 43.9 11.5 86.6 33.4 124.1L0 480l108.7-37.9c35.7 19.6 76 29.9 117.2 29.9h.1c120.3 0 218.9-98.5 218.9-218.9 0-59.3-23.1-115.1-64-157zM223.9 438.6c-37.6 0-74.5-10.1-106.6-29.2l-7.6-4.5-64.5 22.5 22.9-63.2-4.9-8C45.5 323.2 34 287.5 34 250.9 34 147 120 61 223.9 61c58 0 112.5 22.6 153.5 63.6 41 41 63.6 95.5 63.6 153.5 0 119.9-97.6 216.5-216.1 216.5zm121.9-159.1c-6.7-3.4-39.7-19.6-45.8-21.8-6.1-2.3-10.6-3.4-15.1 3.4-4.5 6.7-17.3 21.8-21.2 26.3-3.9 4.5-7.8 5.1-14.5 1.7-39.3-19.7-65.1-35.2-91.1-79.7-6.9-11.8 6.9-11 19.7-36.4 2.2-4.5 1.1-8.4-.6-11.7-1.7-3.4-15.1-36.5-20.7-50-5.4-12.9-10.9-11.1-15.1-11.3-3.9-.2-8.4-.2-12.9-.2s-11.7 1.7-17.9 8.4c-6.1 6.7-23.3 22.8-23.3 55.8s23.9 64.7 27.3 69.2c3.4 4.5 46.8 71.5 113.4 100.3 42.1 18.1 58.6 19.6 79.7 16.5 12.8-1.9 39.7-16.2 45.3-31.9 5.6-15.7 5.6-29.2 3.9-32.1-1.7-3.6-6.1-5.8-12.8-9.2z"/></svg>
      </a>
      <a aria-label="Behance" href="#" class="p-3 rounded-full bg-base-800 hover:bg-white/10 transition shadow-soft" title="Behance">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" class="w-5 h-5 fill-current"><path d="M232 237h-74v48h74c7 0 13-2 18-6 5-4 7-10 7-18 0-16-9-24-25-24zM224 176h-66v44h66c7 0 12-2 17-5 4-4 6-10 6-17 0-8-2-14-6-18-4-3-10-4-17-4zM386 236c-15 0-26 5-34 14-8 9-12 22-12 39h88c0-17-4-30-12-39-8-9-19-14-30-14zM512 64H64C28.7 64 0 92.7 0 128v256c0 35.3 28.7 64 64 64h448c35.3 0 64-28.7 64-64V128c0-35.3-28.7-64-64-64zM342 160h88v32h-88v-32zm-86 192H104V128h130c23 0 42 6 56 17 14 11 21 27 21 47 0 11-2 20-7 28-5 8-12 14-21 19 13 4 23 11 30 22 7 10 11 22 11 37 0 22-8 39-23 51-16 12-36 18-61 18zm208-42H340c0 24 7 43 22 57 14 15 34 22 59 22 27 0 50-7 68-21v33c-20 13-46 19-77 19-35 0-62-10-82-30-20-19-30-47-30-82 0-35 10-62 29-82 20-20 45-30 76-30 30 0 54 9 72 28 18 18 27 44 27 77v12z"/></svg>
      </a>
    </aside>

    <!-- Header -->
    <header class="fixed top-0 inset-x-0 z-50 backdrop-blur-xs bg-black/40 border-b border-white/5">
      <div class="mx-auto max-w-7xl px-6 py-4 flex items-center justify-between">
        <a href="#home" class="text-white font-extrabold tracking-wide">VICTOR HUGO PALMA</a>
        <nav class="hidden md:flex items-center gap-8 text-sm">
          <a href="#sobre" class="nav-link hover:text-white/90 text-white/70">SOBRE</a>
          <a href="#projetos" class="nav-link hover:text-white/90 text-white/70">PROJETOS</a>
          <a href="#depoimentos" class="nav-link hover:text-white/90 text-white/70">DEPOIMENTOS</a>
          <a href="#contato" class="nav-link hover:text-white/90 text-white/70">CONTATO</a>
        </nav>
      </div>
    </header>

    <!-- Hero -->
    <section id="home" class="section relative overflow-hidden pt-32 pb-24">
      <div class="blob"></div>
      <div class="mx-auto max-w-7xl px-6 grid grid-cols-1 lg:grid-cols-12 gap-10 items-center">
        <!-- Portrait card -->
        <div class="lg:col-span-5">
          <div class="relative rounded-3xl bg-base-800 card-glow p-2">
            <div class="aspect-[4/5] overflow-hidden rounded-2xl bg-gradient-to-b from-white/5 to-white/[0.02] flex items-center justify-center">
              <!-- Placeholder portrait. Substitua src por sua foto -->
              <img alt="Retrato de Victor Hugo Palma" src="https://images.unsplash.com/photo-1547106634-56dcd53ae883?q=80&w=900&auto=format&fit=crop" class="h-full w-full object-cover" />
            </div>
            <div class="absolute -bottom-4 left-6 select-none">
              <span class="inline-flex items-center px-4 py-2 rounded-xl bg-black/80 ring-1 ring-white/10 text-xs tracking-wider uppercase">Designer Gráfico</span>
            </div>
          </div>
        </div>
        <!-- Copy -->
        <div class="lg:col-span-7">
          <h1 class="text-4xl sm:text-5xl lg:text-6xl xl:text-7xl font-extrabold leading-tight uppercase">
            OLÁ, SOU O VICTOR.<br />
            DESIGNER GRÁFICO<br />
            CRIATIVO!
          </h1>
          <div class="mt-6 flex flex-wrap items-center gap-x-6 gap-y-2 text-sm text-white/70">
            <span>DESIGN</span>
            <span class="opacity-40">✳</span>
            <span>BRANDING</span>
            <span class="opacity-40">✳</span>
            <span>SOCIAL MEDIA</span>
          </div>
          <div class="mt-10 flex flex-wrap gap-4">
            <a href="#projetos" class="px-6 py-3 rounded-xl bg-white text-black font-semibold hover:bg-white/90 transition">Meus Projetos</a>
            <a href="#contato" class="px-6 py-3 rounded-xl border border-white/20 hover:border-white/40 font-semibold">Contato</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Sobre -->
    <section id="sobre" class="section py
