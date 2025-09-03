<!doctype html>
<html lang="pt-BR">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Rodrigo Bina — Designer Gráfico Criativo</title>
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
      .nav-link { position: relative; }
      .nav-link.active::after { content: ""; position: absolute; left: 0; bottom: -6px; height: 2px; width: 100%; background: white; border-radius: 2px; }
      .card-glow { box-shadow: inset 0 0 0 1px rgba(255,255,255,.06), 0 20px 50px rgba(0,0,0,.5); }
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
    <!-- Social vertical -->
    <aside class="hidden md:flex fixed right-4 top-1/2 -translate-y-1/2 z-40 flex-col items-center gap-4">
      <a aria-label="Instagram" href="#" class="p-3 rounded-full bg-base-800 hover:bg-white/10 transition shadow-soft" title="Instagram">Inserir link</a>
      <a aria-label="LinkedIn" href="#" class="p-3 rounded-full bg-base-800 hover:bg-white/10 transition shadow-soft" title="LinkedIn">Inserir link</a>
      <a aria-label="WhatsApp" href="#" class="p-3 rounded-full bg-base-800 hover:bg-white/10 transition shadow-soft" title="WhatsApp">Inserir link</a>
      <a aria-label="Behance" href="#" class="p-3 rounded-full bg-base-800 hover:bg-white/10 transition shadow-soft" title="Behance">Inserir link</a>
    </aside>

    <!-- Header -->
    <header class="fixed top-0 inset-x-0 z-50 backdrop-blur-xs bg-black/40 border-b border-white/5">
      <div class="mx-auto max-w-7xl px-6 py-4 flex items-center justify-between">
        <a href="#home" class="text-white font-extrabold tracking-wide">RODRIGO BINA</a>
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
        <div class="lg:col-span-5">
          <div class="relative rounded-3xl bg-base-800 card-glow p-2">
            <div class="aspect-[4/5] overflow-hidden rounded-2xl bg-gradient-to-b from-white/5 to-white/[0.02] flex items-center justify-center">
              <img alt="Retrato de Rodrigo Bina" src="inserir link" class="h-full w-full object-cover" />
            </div>
            <div class="absolute -bottom-4 left-6 select-none">
              <span class="inline-flex items-center px-4 py-2 rounded-xl bg-black/80 ring-1 ring-white/10 text-xs tracking-wider uppercase">Designer Gráfico</span>
            </div>
          </div>
        </div>
        <div class="lg:col-span-7">
          <h1 class="text-4xl sm:text-5xl lg:text-6xl xl:text-7xl font-extrabold leading-tight uppercase">
            OLÁ, SOU O RODRIGO.<br />
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
    <section id="sobre" class="section py-16 md:py-24 bg-gradient-to-b from-transparent to-white/[0.02]">
      <div class="mx-auto max-w-7xl px-6 grid grid-cols-1 md:grid-cols-12 gap-10 items-start">
        <div class="md:col-span-3">
          <h2 class="text-2xl font-extrabold tracking-tight">SOBRE</h2>
        </div>
        <div class="md:col-span-9 text-lg leading-relaxed text-white/80">
          <p>
            Sou Rodrigo Bina, designer gráfico apaixonado por transformar conceitos em experiências visuais marcantes. Há mais de 2 anos, ajudo marcas a traduzirem sua essência em design estratégico, que conecta, emociona e gera resultados.
          </p>
          <div class="mt-10 flex flex-wrap gap-6 text-sm font-semibold text-white/80">
            <span class="px-3 py-2 rounded-full bg-white/5 ring-1 ring-white/10">Kits</span>
            <span class="px-3 py-2 rounded-full bg-white/5 ring-1 ring-white/10">Identidade Visual</span>
            <span class="px-3 py-2 rounded-full bg-white/5 ring-1 ring-white/10">Branding</span>
            <span class="px-3 py-2 rounded-full bg-white/5 ring-1 ring-white/10">Redes Sociais</span>
            <span class="px-3 py-2 rounded-full bg-white/5 ring-1 ring-white/10">Mídia Kits</span>
          </div>
        </div>
      </div>
    </section>

    <!-- Serviços -->
    <section class="section py-12 md:py-16">
      <div class="mx-auto max-w-7xl px-6">
        <h3 class="text-sm uppercase tracking-[.3em] text-white/50">Meus Serviços</h3>
        <div class="mt-6 divide-y divide-white/10 rounded-2xl overflow-hidden border border-white/10">
          <details class="group open:bg-white/[0.02]">
            <summary class="flex w-full items-center justify-between px-6 py-6 cursor-pointer list-none">
              <span class="text-3xl md:text-5xl font-bold">Branding e Identidade Visual</span>
              <span class="ml-6 shrink-0 rounded-full border border-white/20 w-8 h-8 grid place-items-center group-open:rotate-45 transition">+</span>
            </summary>
            <div class="px-6 pb-6 text-white/75 max-w-3xl">
              Desenvolvimento de marca, plataforma verbal e visual, manual de identidade e aplicações.
            </div>
          </details>
          <details class="group">
            <summary class="flex w-full items-center justify-between px-6 py-6 cursor-pointer list-none">
              <span class="text-3xl md:text-5xl font-bold">Design de Mídias Sociais</span>
              <span class="ml-6 shrink-0 rounded-full border border-white/20 w-8 h-8 grid place-items-center group-open:rotate-45 transition">+</span>
            </summary>
            <div class="px-6 pb-6 text-white/75 max-w-3xl">Conteúdo estratégico e visual para Instagram, LinkedIn e outras plataformas.</div>
          </details>
          <details class="group">
            <summary class="flex w-full items-center justify-between px-6 py-6 cursor-pointer list-none">
              <span class="text-3xl md:text-5xl font-bold">Materiais Institucionais</span>
              <span class="ml-6 shrink-0 rounded-full border border-white/20 w-8 h-8 grid place-items-center
