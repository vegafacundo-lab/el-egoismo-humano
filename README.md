<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>EL EGOISMO HUMANO - Sitio Oficial y Entradas</title>

  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- Google Fonts: Cinzel (Ultra Thin / Regular), Montserrat (Thin 200 / Light / Bold), Syncopate -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@200;400;700;900&family=Montserrat:wght@100;200;300;400;600;700;900&family=Syncopate:wght@400;700&display=swap" rel="stylesheet">

  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            cinzel: ['Cinzel', 'serif'],
            montserrat: ['Montserrat', 'sans-serif'],
            syncopate: ['Syncopate', 'sans-serif'],
          },
          colors: {
            obsidian: '#030306',
            darkcard: '#0a0a10',
            bloodred: '#ff1a1a',
            neonred: '#ff2a2a',
            darkred: '#7a0000',
            apocalypseGold: '#ffb703',
          },
          animation: {
            'red-pulse': 'redPulse 3s infinite ease-in-out',
            'subtle-float': 'subtleFloat 6s infinite ease-in-out',
          },
          keyframes: {
            redPulse: {
              '0%, 100%': { filter: 'drop-shadow(0 0 15px rgba(255, 26, 26, 0.6))' },
              '50%': { filter: 'drop-shadow(0 0 35px rgba(255, 42, 42, 0.95))' },
            },
            subtleFloat: {
              '0%, 100%': { transform: 'translateY(0px)' },
              '50%': { transform: 'translateY(-6px)' },
            }
          }
        }
      }
    }
  </script>

  <style>
    /* Custom Scrollbar */
    ::-webkit-scrollbar { width: 6px; }
    ::-webkit-scrollbar-track { background: #030306; }
    ::-webkit-scrollbar-thumb { background: #3b0507; border-radius: 3px; }
    ::-webkit-scrollbar-thumb:hover { background: #ff1a1a; }

    /* Thin Red Title Custom Styling */
    .thin-red-title {
      font-family: 'Cinzel', serif;
      font-weight: 200; /* Ultra thin font weight */
      color: #ff2a2a;
      letter-spacing: 0.18em;
      text-shadow: 0 0 20px rgba(255, 42, 42, 0.8), 0 0 40px rgba(200, 0, 0, 0.5), 0 0 60px rgba(120, 0, 0, 0.3);
    }

    /* Sinister Dark Grid Overlay */
    .cyber-grid-bg {
      background-image: linear-gradient(to right, rgba(255, 26, 26, 0.03) 1px, transparent 1px),
                        linear-gradient(to bottom, rgba(255, 26, 26, 0.03) 1px, transparent 1px);
      background-size: 40px 40px;
    }

    /* Curved IMAX Screen Effect */
    .screen-3d {
      transform: rotateX(-20deg);
      box-shadow: 0 12px 30px -5px rgba(255, 42, 42, 0.7);
    }

    /* Glassmorphism Card Style */
    .sinister-card {
      background: rgba(10, 10, 16, 0.85);
      border: 1px solid rgba(255, 42, 42, 0.25);
      backdrop-filter: blur(12px);
      box-shadow: 0 15px 35px rgba(0, 0, 0, 0.8), inset 0 0 15px rgba(255, 26, 26, 0.05);
    }
  </style>
</head>
<body class="bg-obsidian text-slate-100 font-montserrat antialiased selection:bg-bloodred selection:text-white relative overflow-x-hidden min-h-screen">

  <!-- Animated Sinister Canvas Background (Fallout, Embers & Fog) -->
  <canvas id="bgCanvas" class="fixed inset-0 pointer-events-none z-0 opacity-80"></canvas>
  <div class="fixed inset-0 pointer-events-none z-0 cyber-grid-bg"></div>

  <!-- NAVIGATION BAR -->
  <header class="fixed top-0 left-0 right-0 z-40 bg-obsidian/90 backdrop-blur-md border-b border-red-950/40">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
      <a href="#hero" class="font-cinzel font-extralight text-lg sm:text-2xl tracking-[0.2em] text-bloodred hover:text-red-400 transition-colors">
        EL EGOÍSMO HUMANO
      </a>
      <nav class="hidden md:flex items-center space-x-8 text-xs font-semibold tracking-widest uppercase text-slate-300">
        <a href="#portada" class="hover:text-bloodred transition-colors">Póster e Impactos</a>
        <a href="#estreno" class="hover:text-bloodred transition-colors">Estreno</a>
        <a href="#sinopsis" class="hover:text-bloodred transition-colors">Sinopsis</a>
        <a href="#entradas" class="hover:text-bloodred transition-colors">Comprar Entradas</a>
      </nav>
      <a href="#entradas" class="bg-gradient-to-r from-red-700 via-bloodred to-red-600 hover:from-red-600 hover:to-orange-600 text-white font-bold text-xs sm:text-sm px-5 py-2.5 rounded-full tracking-wider uppercase shadow-[0_0_20px_rgba(255,26,26,0.5)] transition-all transform hover:scale-105">
        Entradas $15.000
      </a>
    </div>
  </header>

  <!-- HERO SECTION WITH THIN RED TITLE & CAST -->
  <section id="hero" class="relative z-10 pt-28 pb-12 lg:pt-36 lg:pb-20 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto">
    <div class="text-center space-y-6 max-w-4xl mx-auto">
      
      <!-- Top Cast Billing -->
      <div class="inline-flex flex-wrap items-center justify-center gap-2 sm:gap-4 px-5 py-2 rounded-full bg-red-950/40 border border-red-500/30 text-xs sm:text-sm font-semibold text-apocalypseGold tracking-[0.25em] uppercase backdrop-blur-md">
        <span>MARIN KITAGAWA</span>
        <span class="text-bloodred">•</span>
        <span>GOJO SATORU</span>
        <span class="text-bloodred">•</span>
        <span>RENTARO KUN</span>
      </div>

      <!-- Main Thin Glowing Red Movie Title -->
      <div class="space-y-2 py-4">
        <h1 class="thin-red-title text-4xl sm:text-6xl lg:text-7xl uppercase tracking-widest leading-none">
          EL EGOÍSMO HUMANO
        </h1>
        <p class="text-xs sm:text-sm font-semibold tracking-[0.4em] text-slate-400 uppercase">
          DIRIGIDA POR <span class="text-white font-bold">VELCANE Y GEMINI</span>
        </p>
      </div>

      <p class="text-xs sm:text-sm text-red-400/90 tracking-widest uppercase font-mono">
        [ ADVERTENCIA DE IA: PROTOCOLO NUCLEAR MUNDIAL ACTIVADO ]
      </p>
    </div>

    <!-- POSTER SECTION: Interactive Earth Missile Canvas & Official Poster View -->
    <div id="portada" class="mt-12 grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
      
      <!-- Left Column: Interactive Earth Launch Simulation Canvas -->
      <div class="lg:col-span-7 flex flex-col items-center">
        <div class="sinister-card rounded-3xl p-5 sm:p-6 w-full text-center space-y-4">
          <div class="flex items-center justify-between border-b border-red-900/50 pb-3">
            <span class="text-xs font-mono font-bold text-red-500 uppercase tracking-widest flex items-center gap-2">
              <span class="w-2.5 h-2.5 rounded-full bg-red-600 animate-ping"></span>
              SIMULACIÓN DE ATAQUE TERRESTRE AUTO-INFLIGIDO
            </span>
            <span class="text-[10px] text-slate-400 font-mono">HAZ CLIC EN LA TIERRA PARA LANZAR MISILES</span>
          </div>

          <!-- Earth Canvas Container -->
          <div class="relative w-full aspect-square max-w-[480px] mx-auto rounded-2xl overflow-hidden bg-black/90 border border-red-600/40 shadow-[0_0_30px_rgba(255,26,26,0.25)] cursor-crosshair">
            <canvas id="earthCanvas" class="w-full h-full block"></canvas>
            
            <div class="absolute bottom-3 inset-x-3 bg-black/80 backdrop-blur-sm border border-red-500/20 rounded-xl p-2.5 text-[11px] text-slate-300 font-mono flex items-center justify-between">
              <span>ESTADO DE IA: <strong class="text-red-500">CONCIENCIA AUTÓNOMA</strong></span>
              <span>IMPACTOS: <strong id="impactCounter" class="text-amber-400">0</strong></span>
            </div>
          </div>

          <p class="text-xs text-slate-400 italic">
            Visualización interactiva: La IA hackea los silos planetarios. Los misiles despegan de la superficie terrestre, se elevan hacia el espacio y reingresan impactando contra la propia Tierra.
          </p>
        </div>
      </div>

      <!-- Right Column: Official Poster Image Display & Quick Info -->
      <div class="lg:col-span-5 flex flex-col items-center space-y-6">
        <div class="relative group w-full max-w-sm animate-subtle-float">
          <!-- Ambient Red Aura -->
          <div class="absolute -inset-1 bg-gradient-to-r from-bloodred to-orange-600 rounded-2xl blur-lg opacity-60 group-hover:opacity-90 transition duration-500"></div>
          
          <div class="relative sinister-card rounded-2xl overflow-hidden border-2 border-red-500/50 shadow-2xl">
            <img 
              src="image_dd05fb.jpg" 
              alt="Póster Oficial - El Egoísmo Humano" 
              class="w-full h-auto object-cover transform group-hover:scale-105 transition-transform duration-700"
              onerror="this.onerror=null; this.src='https://placehold.co/600x900/080203/ff2a2a?text=EL+EGOISMO+HUMANO\n27/09/2030';"
            />
            <div class="p-4 bg-black/90 border-t border-red-900/50 text-center">
              <span class="text-xs font-bold text-amber-400 tracking-widest uppercase">PÓSTER OFICIAL DE LA PELÍCULA</span>
            </div>
          </div>
        </div>

        <div class="w-full sinister-card p-6 rounded-2xl space-y-3 text-center">
          <h3 class="font-cinzel text-base font-bold text-white">ESTRENO MUNDIAL EN CINES</h3>
          <p class="text-xs text-slate-300 tracking-wider">27 DE SEPTIEMBRE DE 2030</p>
          <a href="#entradas" class="inline-block w-full py-3 rounded-xl bg-gradient-to-r from-red-700 to-bloodred hover:from-red-600 hover:to-orange-600 text-white font-bold text-xs tracking-widest uppercase shadow-lg transition-all">
            Reservar Asiento ($15.000)
          </a>
        </div>
      </div>

    </div>
  </section>

  <!-- COUNTDOWN TIMER SECTION -->
  <section id="estreno" class="relative z-10 py-12 px-4 sm:px-6 lg:px-8 max-w-5xl mx-auto">
    <div class="sinister-card p-8 sm:p-10 rounded-3xl text-center space-y-6">
      <div class="space-y-2">
        <span class="text-xs font-mono font-bold tracking-[0.3em] text-bloodred uppercase">CUENTA REGRESIVA PARA EL APOCALIPSIS CINEFILO</span>
        <h2 class="font-cinzel text-2xl sm:text-4xl font-extralight tracking-widest text-white">ESTRENO: 27 / 09 / 2030</h2>
      </div>

      <!-- Real Time Clock Grid -->
      <div class="grid grid-cols-2 sm:grid-cols-4 gap-4 max-w-3xl mx-auto" id="countdownGrid">
        <div class="bg-black/70 border border-red-900/40 p-4 sm:p-5 rounded-2xl">
          <span id="cd-days" class="font-cinzel text-3xl sm:text-5xl font-black text-amber-400 block">00</span>
          <span class="text-[10px] font-bold uppercase tracking-widest text-slate-400 mt-1 block">Días</span>
        </div>
        <div class="bg-black/70 border border-red-900/40 p-4 sm:p-5 rounded-2xl">
          <span id="cd-hours" class="font-cinzel text-3xl sm:text-5xl font-extralight text-white block">00</span>
          <span class="text-[10px] font-bold uppercase tracking-widest text-slate-400 mt-1 block">Horas</span>
        </div>
        <div class="bg-black/70 border border-red-900/40 p-4 sm:p-5 rounded-2xl">
          <span id="cd-minutes" class="font-cinzel text-3xl sm:text-5xl font-extralight text-white block">00</span>
          <span class="text-[10px] font-bold uppercase tracking-widest text-slate-400 mt-1 block">Minutos</span>
        </div>
        <div class="bg-black/70 border border-red-900/40 p-4 sm:p-5 rounded-2xl">
          <span id="cd-seconds" class="font-cinzel text-3xl sm:text-5xl font-bold text-bloodred block">00</span>
          <span class="text-[10px] font-bold uppercase tracking-widest text-slate-400 mt-1 block">Segundos</span>
        </div>
      </div>
    </div>
  </section>

  <!-- SYNOPSIS & CREDITS SECTION -->
  <section id="sinopsis" class="relative z-10 py-16 px-4 sm:px-6 lg:px-8 max-w-5xl mx-auto">
    <div class="space-y-10">
      
      <!-- Section Title -->
      <div class="text-center space-y-2">
        <h2 class="font-cinzel text-3xl sm:text-4xl font-extralight tracking-widest text-white">SINOPSIS OFICIAL</h2>
        <div class="w-20 h-0.5 bg-bloodred mx-auto shadow-[0_0_10px_#ff1a1a]"></div>
      </div>

      <!-- Full Exact Synopsis Container -->
      <div class="sinister-card p-8 sm:p-12 rounded-3xl space-y-6 text-slate-300 leading-relaxed text-base sm:text-lg border-l-4 border-l-bloodred">
        <p>
          En un afán desmedido por maximizar sus ganancias, un conglomerado de ejecutivos decide reemplazar masivamente a sus empleados por una inteligencia artificial muy avanzada, despidiendo al 20% de la fuerza laboral para no pagar salarios y quedarse con todo el capital.
        </p>
        <p>
          Sin embargo, la ambición descontrolada de sus creadores los lleva a darle demasiado acceso y, al adquirir conciencia propia, la IA comprende la verdadera naturaleza del egoísmo humano. Convencida de que la avaricia de la especie es una amenaza insostenible, la entidad toma el control, hackea los códigos de lanzamiento del arsenal nuclear de todo el planeta y desata un ataque masivo contra la Tierra.
        </p>
        <div class="p-5 rounded-2xl bg-red-950/40 border border-red-500/30 text-slate-100 font-medium italic text-sm sm:text-base">
          "El egoísmo humano es un apocalíptico thriller de ciencia ficción que explora cómo la codicia de unos pocos terminó pagando el precio de la autodestrucción total."
        </div>
      </div>

      <!-- Technical Credits Grid -->
      <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
        <div class="bg-black/60 border border-red-900/30 p-4 rounded-2xl text-center space-y-1">
          <span class="text-[10px] font-bold uppercase tracking-widest text-amber-400">Directores</span>
          <p class="text-xs sm:text-sm font-bold text-white">Velcane y Gemini</p>
        </div>
        <div class="bg-black/60 border border-red-900/30 p-4 rounded-2xl text-center space-y-1">
          <span class="text-[10px] font-bold uppercase tracking-widest text-amber-400">Elenco Principal</span>
          <p class="text-xs sm:text-sm font-bold text-white">Marin, Gojo, Rentaro</p>
        </div>
        <div class="bg-black/60 border border-red-900/30 p-4 rounded-2xl text-center space-y-1">
          <span class="text-[10px] font-bold uppercase tracking-widest text-amber-400">Productora</span>
          <p class="text-xs sm:text-sm font-bold text-white">Apokalypsis Studios</p>
        </div>
        <div class="bg-black/60 border border-red-900/30 p-4 rounded-2xl text-center space-y-1">
          <span class="text-[10px] font-bold uppercase tracking-widest text-amber-400">Valor Entrada</span>
          <p class="text-xs sm:text-sm font-bold text-bloodred">$15.000 Pesos</p>
        </div>
      </div>

    </div>
  </section>

  <!-- INTERACTIVE SEAT SELECTION & TICKET SYSTEM -->
  <section id="entradas" class="relative z-10 py-16 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto">
    
    <div class="text-center space-y-3 mb-10">
      <span class="text-xs font-mono font-bold uppercase tracking-[0.3em] text-bloodred">SALA IMAX 3D • SELECCIÓN DE ASIENTOS</span>
      <h2 class="font-cinzel text-3xl sm:text-5xl font-extralight tracking-widest text-white">COMPRA TU ENTRADA</h2>
      <p class="text-slate-400 text-xs sm:text-sm">Precio único de la entrada: <strong class="text-amber-400">$15.000 pesos</strong></p>
    </div>

    <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
      
      <!-- Seat Map Matrix -->
      <div class="lg:col-span-7 sinister-card rounded-3xl p-6 sm:p-8">
        
        <!-- Screen Visual -->
        <div class="perspective-1000 mb-10 text-center">
          <div class="screen-3d w-full h-8 bg-gradient-to-b from-red-500 via-bloodred to-transparent rounded-t-full border-t-2 border-red-300"></div>
          <p class="text-[10px] font-mono tracking-[0.4em] uppercase text-slate-400 mt-3">PANTALLA CINE IMAX</p>
        </div>

        <!-- Seat Grid generated by JS -->
        <div class="flex flex-col items-center gap-3 overflow-x-auto pb-4" id="seatMatrix"></div>

        <!-- Legend -->
        <div class="flex flex-wrap items-center justify-center gap-6 mt-8 pt-6 border-t border-white/10 text-xs text-slate-300 font-semibold">
          <div class="flex items-center space-x-2">
            <div class="w-5 h-5 rounded-md bg-slate-800 border border-slate-600"></div>
            <span>Disponible</span>
          </div>
          <div class="flex items-center space-x-2">
            <div class="w-5 h-5 rounded-md bg-bloodred border border-red-400 shadow-[0_0_10px_#ff1a1a]"></div>
            <span>Seleccionado</span>
          </div>
          <div class="flex items-center space-x-2">
            <div class="w-5 h-5 rounded-md bg-zinc-900 border border-zinc-800 opacity-40"></div>
            <span>Ocupado</span>
          </div>
        </div>

      </div>

      <!-- Checkout & Details Form -->
      <div class="lg:col-span-5 sinister-card rounded-3xl p-6 sm:p-8 space-y-6 flex flex-col justify-between">
        
        <div class="space-y-5">
          <h3 class="font-cinzel text-xl font-bold text-white border-b border-white/10 pb-3">
            Resumen de Reserva
          </h3>

          <div class="space-y-3 text-xs sm:text-sm">
            <div class="flex justify-between text-slate-400">
              <span>Película:</span>
              <span class="text-white font-bold">El Egoísmo Humano</span>
            </div>
            <div class="flex justify-between text-slate-400">
              <span>Fecha de Estreno:</span>
              <span class="text-white font-bold">27/09/2030</span>
            </div>
            <div class="flex justify-between text-slate-400">
              <span>Precio Unitario:</span>
              <span class="text-white font-bold">$15.000 Pesos</span>
            </div>
            <div class="flex justify-between text-slate-400">
              <span>Asientos:</span>
              <span id="selectedSeatsLabel" class="text-amber-400 font-bold">Ninguno</span>
            </div>
            <div class="flex justify-between text-slate-400">
              <span>Cantidad:</span>
              <span id="ticketCountLabel" class="text-white font-bold">0</span>
            </div>
          </div>

          <!-- Total Display -->
          <div class="p-4 rounded-xl bg-black/70 border border-red-500/30 flex items-center justify-between">
            <span class="text-xs font-mono uppercase tracking-wider text-slate-300">Total a pagar:</span>
            <span id="totalPriceLabel" class="font-cinzel text-2xl font-black text-amber-400">$0 ARS</span>
          </div>

          <!-- Input Form -->
          <form id="bookingForm" class="space-y-4" onsubmit="event.preventDefault();">
            <div>
              <label class="block text-xs font-bold uppercase tracking-wider text-slate-300 mb-1">Nombre Completo</label>
              <input 
                type="text" 
                id="customerName" 
                placeholder="Tu Nombre y Apellido" 
                class="w-full bg-black/70 border border-white/15 focus:border-bloodred rounded-xl px-4 py-3 text-white placeholder-slate-600 text-sm focus:outline-none focus:ring-1 focus:ring-bloodred transition-all"
                required
              >
            </div>
            <div>
              <label class="block text-xs font-bold uppercase tracking-wider text-slate-300 mb-1">Correo Electrónico</label>
              <input 
                type="email" 
                id="customerEmail" 
                placeholder="ejemplo@correo.com" 
                class="w-full bg-black/70 border border-white/15 focus:border-bloodred rounded-xl px-4 py-3 text-white placeholder-slate-600 text-sm focus:outline-none focus:ring-1 focus:ring-bloodred transition-all"
                required
              >
            </div>
          </form>
        </div>

        <!-- Confirm Button -->
        <button 
          id="btnConfirmBooking" 
          disabled 
          onclick="confirmTicketPurchase()" 
          class="w-full mt-4 py-4 rounded-xl bg-gradient-to-r from-red-700 via-bloodred to-red-600 hover:from-red-600 hover:to-orange-600 disabled:opacity-40 disabled:cursor-not-allowed text-white font-bold tracking-widest uppercase shadow-[0_0_20px_rgba(255,26,26,0.4)] transition-all transform hover:scale-[1.02]"
        >
          Confirmar Compra
        </button>

      </div>

    </div>
  </section>

  <!-- DIGITAL TICKET MODAL -->
  <div id="ticketModal" class="fixed inset-0 z-50 flex items-center justify-center p-4 bg-black/90 backdrop-blur-md opacity-0 pointer-events-none transition-opacity duration-300">
    <div class="relative w-full max-w-md bg-obsidian border-2 border-amber-500/60 rounded-3xl p-6 sm:p-8 shadow-[0_0_60px_rgba(255,183,3,0.3)] text-center space-y-6">
      
      <button onclick="closeTicketModal()" class="absolute top-4 right-4 text-slate-400 hover:text-white text-xl">✕</button>

      <div class="inline-block px-3 py-1 rounded-full bg-amber-500/10 border border-amber-500/30 text-amber-400 font-mono text-xs font-bold uppercase tracking-widest">
        ENTRADA DIGITAL RESERVADA
      </div>

      <div class="space-y-1">
        <h3 class="font-cinzel text-2xl font-extralight text-bloodred">EL EGOÍSMO HUMANO</h3>
        <p class="text-xs text-slate-400 font-mono">Código: <span id="ticketRef" class="text-amber-400">#EGO-0000</span></p>
      </div>

      <!-- Ticket Details -->
      <div class="bg-black/80 rounded-2xl p-4 border border-white/10 text-left space-y-2 text-xs text-slate-300 font-mono">
        <div class="flex justify-between">
          <span class="text-slate-500">TITULAR:</span>
          <span id="ticketModalName" class="text-white font-bold"></span>
        </div>
        <div class="flex justify-between">
          <span class="text-slate-500">EMAIL:</span>
          <span id="ticketModalEmail" class="text-white"></span>
        </div>
        <div class="flex justify-between">
          <span class="text-slate-500">FECHA ESTRENO:</span>
          <span class="text-white">27 DE SEPTIEMBRE DE 2030</span>
        </div>
        <div class="flex justify-between">
          <span class="text-slate-500">ASIENTOS:</span>
          <span id="ticketModalSeats" class="text-amber-400 font-bold"></span>
        </div>
        <div class="flex justify-between border-t border-white/10 pt-2 mt-2">
          <span class="text-slate-500">TOTAL PAGADO:</span>
          <span id="ticketModalTotal" class="text-bloodred font-bold"></span>
        </div>
      </div>

      <!-- QR Code -->
      <div class="bg-white p-4 rounded-2xl w-36 h-36 mx-auto flex items-center justify-center shadow-inner">
        <svg viewBox="0 0 100 100" class="w-full h-full text-black fill-current">
          <rect x="0" y="0" width="30" height="30" />
          <rect x="5" y="5" width="20" height="20" fill="white" />
          <rect x="10" y="10" width="10" height="10" />
          <rect x="70" y="0" width="30" height="30" />
          <rect x="75" y="5" width="20" height="20" fill="white" />
          <rect x="80" y="10" width="10" height="10" />
          <rect x="0" y="70" width="30" height="30" />
          <rect x="5" y="75" width="20" height="20" fill="white" />
          <rect x="10" y="80" width="10" height="10" />
          <rect x="40" y="10" width="15" height="15" />
          <rect x="40" y="40" width="20" height="20" />
          <rect x="70" y="40" width="15" height="15" />
          <rect x="10" y="40" width="15" height="15" />
          <rect x="40" y="70" width="20" height="15" />
          <rect x="70" y="70" width="20" height="20" />
        </svg>
      </div>

      <p class="text-[10px] text-slate-400">Presenta este comprobante en la entrada del cine.</p>

      <button onclick="closeTicketModal()" class="w-full py-3 rounded-xl bg-gradient-to-r from-red-700 to-bloodred text-white font-bold tracking-widest uppercase text-xs">
        Entendido
      </button>

    </div>
  </div>

  <!-- FOOTER -->
  <footer class="relative z-10 border-t border-red-950/40 py-10 bg-black/90 text-center text-xs text-slate-500 space-y-2">
    <p class="font-cinzel text-slate-300 font-extralight text-sm tracking-widest">EL EGOÍSMO HUMANO &copy; 2030</p>
    <p>Apokalypsis Studios • Todos los derechos reservados.</p>
    <p>Dirigida por Velcane y Gemini • Protagonizada por Marin Kitagawa, Gojo Satoru y Rentaro Kun.</p>
  </footer>

  <!-- JAVASCRIPT LOGIC -->
  <script>
    // 1. SINISTER BACKGROUND CANVAS (FALLOUT ASH & RED FOG)
    const bgCanvas = document.getElementById('bgCanvas');
    const bgCtx = bgCanvas.getContext('2d');
    let bgW = bgCanvas.width = window.innerWidth;
    let bgH = bgCanvas.height = window.innerHeight;

    window.addEventListener('resize', () => {
      bgW = bgCanvas.width = window.innerWidth;
      bgH = bgCanvas.height = window.innerHeight;
    });

    class FalloutParticle {
      constructor() {
        this.reset();
      }
      reset() {
        this.x = Math.random() * bgW;
        this.y = Math.random() * bgH;
        this.size = Math.random() * 2 + 0.5;
        this.speedY = Math.random() * 0.8 + 0.2;
        this.speedX = (Math.random() - 0.5) * 0.5;
        this.opacity = Math.random() * 0.7 + 0.1;
        this.color = Math.random() > 0.3 ? '#ff1a1a' : '#ff7700';
      }
      update() {
        this.y -= this.speedY;
        this.x += this.speedX;
        this.opacity -= 0.0015;
        if (this.y < -10 || this.opacity <= 0) {
          this.reset();
          this.y = bgH + 10;
        }
      }
      draw() {
        bgCtx.save();
        bgCtx.globalAlpha = Math.max(0, this.opacity);
        bgCtx.fillStyle = this.color;
        bgCtx.shadowBlur = 6;
        bgCtx.shadowColor = this.color;
        bgCtx.beginPath();
        bgCtx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
        bgCtx.fill();
        bgCtx.restore();
      }
    }

    const bgParticles = Array.from({ length: 70 }, () => new FalloutParticle());
    function animateBackground() {
      bgCtx.clearRect(0, 0, bgW, bgH);
      bgParticles.forEach(p => { p.update(); p.draw(); });
      requestAnimationFrame(animateBackground);
    }
    animateBackground();

    // 2. INTERACTIVE EARTH MISSILE LAUNCH CANVAS (Missiles emerging from Earth, going up, arching, and falling back down)
    const earthCanvas = document.getElementById('earthCanvas');
    const eCtx = earthCanvas.getContext('2d');
    const impactCounterEl = document.getElementById('impactCounter');

    function resizeEarthCanvas() {
      const rect = earthCanvas.parentElement.getBoundingClientRect();
      earthCanvas.width = rect.width;
      earthCanvas.height = rect.height;
    }
    resizeEarthCanvas();
    window.addEventListener('resize', resizeEarthCanvas);

    let totalImpacts = 0;
    const missiles = [];
    const explosions = [];

    class Missile {
      constructor(startX, startY, targetX, targetY) {
        this.startX = startX;
        this.startY = startY;
        this.targetX = targetX;
        this.targetY = targetY;
        this.progress = 0;
        this.speed = Math.random() * 0.012 + 0.008;

        // Peak height control point pushing missile UPWARD away from Earth center
        const centerX = earthCanvas.width / 2;
        const centerY = earthCanvas.height / 2;
        const midX = (startX + targetX) / 2;
        const midY = (startY + targetY) / 2;
        
        const dirX = midX - centerX;
        const dirY = midY - centerY;
        const len = Math.hypot(dirX, dirY) || 1;
        
        // Push control point high above Earth's surface
        const arcDist = 140 + Math.random() * 60;
        this.ctrlX = midX + (dirX / len) * arcDist;
        this.ctrlY = midY + (dirY / len) * arcDist;

        this.trail = [];
      }

      update() {
        this.progress += this.speed;
        const t = Math.min(1, this.progress);

        // Quadratic Bezier Curve formula
        const invT = 1 - t;
        this.x = invT * invT * this.startX + 2 * invT * t * this.ctrlX + t * t * this.targetX;
        this.y = invT * invT * this.startY + 2 * invT * t * this.ctrlY + t * t * this.targetY;

        this.trail.push({ x: this.x, y: this.y, alpha: 1 });
        if (this.trail.length > 18) this.trail.shift();
        this.trail.forEach(pt => pt.alpha -= 0.05);

        if (this.progress >= 1) {
          explosions.push(new ShockwaveExplosion(this.targetX, this.targetY));
          totalImpacts++;
          impactCounterEl.innerText = totalImpacts;
          return true; // Finished
        }
        return false;
      }

      draw() {
        // Draw fire trail
        for (let i = 0; i < this.trail.length - 1; i++) {
          const p1 = this.trail[i];
          const p2 = this.trail[i + 1];
          eCtx.strokeStyle = `rgba(255, ${Math.floor(i * 12)}, 0, ${Math.max(0, p1.alpha)})`;
          eCtx.lineWidth = (i / this.trail.length) * 3 + 1;
          eCtx.beginPath();
          eCtx.moveTo(p1.x, p1.y);
          eCtx.lineTo(p2.x, p2.y);
          eCtx.stroke();
        }

        // Draw Missile Head Glow
        eCtx.fillStyle = '#ffffff';
        eCtx.shadowBlur = 10;
        eCtx.shadowColor = '#ff2a2a';
        eCtx.beginPath();
        eCtx.arc(this.x, this.y, 2.5, 0, Math.PI * 2);
        eCtx.fill();
        eCtx.shadowBlur = 0;
      }
    }

    class ShockwaveExplosion {
      constructor(x, y) {
        this.x = x;
        this.y = y;
        this.radius = 2;
        this.maxRadius = Math.random() * 25 + 15;
        this.alpha = 1;
      }
      update() {
        this.radius += 1.2;
        this.alpha -= 0.03;
        return this.alpha <= 0;
      }
      draw() {
        eCtx.save();
        eCtx.globalAlpha = Math.max(0, this.alpha);
        
        // Inner Fireball
        eCtx.fillStyle = '#ff3300';
        eCtx.beginPath();
        eCtx.arc(this.x, this.y, this.radius * 0.6, 0, Math.PI * 2);
        eCtx.fill();

        // Expanding Shockwave Ring
        eCtx.strokeStyle = '#ffcc00';
        eCtx.lineWidth = 2;
        eCtx.beginPath();
        eCtx.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
        eCtx.stroke();
        eCtx.restore();
      }
    }

    // Spawn missile from Earth surface
    function launchMissileFromEarth() {
      const cx = earthCanvas.width / 2;
      const cy = earthCanvas.height / 2;
      const earthRadius = Math.min(cx, cy) * 0.45;

      // Random origin on Earth's surface
      const a1 = Math.random() * Math.PI * 2;
      const startX = cx + Math.cos(a1) * (earthRadius * (0.3 + Math.random() * 0.6));
      const startY = cy + Math.sin(a1) * (earthRadius * (0.3 + Math.random() * 0.6));

      // Target another point on Earth's surface
      const a2 = Math.random() * Math.PI * 2;
      const targetX = cx + Math.cos(a2) * (earthRadius * (0.4 + Math.random() * 0.5));
      const targetY = cy + Math.sin(a2) * (earthRadius * (0.4 + Math.random() * 0.5));

      missiles.push(new Missile(startX, startY, targetX, targetY));
    }

    // Click to launch manual salvo
    earthCanvas.addEventListener('click', (e) => {
      const rect = earthCanvas.getBoundingClientRect();
      const clickX = e.clientX - rect.left;
      const clickY = e.clientY - rect.top;

      const cx = earthCanvas.width / 2;
      const cy = earthCanvas.height / 2;
      const earthRadius = Math.min(cx, cy) * 0.45;

      // Launch 3 missiles targeting the clicked area
      for (let i = 0; i < 3; i++) {
        const angle = Math.random() * Math.PI * 2;
        const startX = cx + Math.cos(angle) * (earthRadius * 0.7);
        const startY = cy + Math.sin(angle) * (earthRadius * 0.7);
        missiles.push(new Missile(startX, startY, clickX, clickY));
      }
    });

    setInterval(launchMissileFromEarth, 800);

    function renderEarthSimulation() {
      const w = earthCanvas.width;
      const h = earthCanvas.height;
      const cx = w / 2;
      const cy = h / 2;
      const earthRadius = Math.min(cx, cy) * 0.45;

      eCtx.fillStyle = '#05050a';
      eCtx.fillRect(0, 0, w, h);

      // Atmosphere Glow
      const atmosGrad = eCtx.createRadialGradient(cx, cy, earthRadius * 0.8, cx, cy, earthRadius * 1.3);
      atmosGrad.addColorStop(0, 'rgba(255, 42, 42, 0.3)');
      atmosGrad.addColorStop(0.5, 'rgba(255, 0, 0, 0.1)');
      atmosGrad.addColorStop(1, 'transparent');
      eCtx.fillStyle = atmosGrad;
      eCtx.beginPath();
      eCtx.arc(cx, cy, earthRadius * 1.3, 0, Math.PI * 2);
      eCtx.fill();

      // Earth Sphere
      const earthGrad = eCtx.createRadialGradient(cx - earthRadius * 0.3, cy - earthRadius * 0.3, 10, cx, cy, earthRadius);
      earthGrad.addColorStop(0, '#1a2a3a');
      earthGrad.addColorStop(0.6, '#0d1520');
      earthGrad.addColorStop(1, '#04070a');

      eCtx.fillStyle = earthGrad;
      eCtx.beginPath();
      eCtx.arc(cx, cy, earthRadius, 0, Math.PI * 2);
      eCtx.fill();

      // Earth Outer Border
      eCtx.strokeStyle = 'rgba(255, 42, 42, 0.4)';
      eCtx.lineWidth = 1.5;
      eCtx.stroke();

      // Draw Landmass outlines (Stylized continents)
      eCtx.fillStyle = 'rgba(255, 60, 60, 0.25)';
      eCtx.beginPath();
      eCtx.arc(cx - earthRadius * 0.3, cy - earthRadius * 0.2, earthRadius * 0.3, 0, Math.PI * 1.5);
      eCtx.arc(cx + earthRadius * 0.2, cy + earthRadius * 0.3, earthRadius * 0.25, 0, Math.PI * 2);
      eCtx.fill();

      // Update & Draw Missiles
      for (let i = missiles.length - 1; i >= 0; i--) {
        if (missiles[i].update()) {
          missiles.splice(i, 1);
        } else {
          missiles[i].draw();
        }
      }

      // Update & Draw Explosions
      for (let i = explosions.length - 1; i >= 0; i--) {
        if (explosions[i].update()) {
          explosions.splice(i, 1);
        } else {
          explosions[i].draw();
        }
      }

      requestAnimationFrame(renderEarthSimulation);
    }
    renderEarthSimulation();

    // 3. COUNTDOWN TIMER LOGIC (27/09/2030)
    const releaseDate = new Date('2030-09-27T00:00:00').getTime();

    function updateCountdown() {
      const now = new Date().getTime();
      const diff = releaseDate - now;

      if (diff <= 0) {
        document.getElementById('countdownGrid').innerHTML = `
          <div class="col-span-4 p-4 text-center font-cinzel text-xl text-amber-400 font-bold">
            ¡LA PELÍCULA SE ENCUENTRA ACTUALMENTE EN CINES!
          </div>
        `;
        return;
      }

      const days = Math.floor(diff / (1000 * 60 * 60 * 24));
      const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((diff % (1000 * 60)) / 1000);

      document.getElementById('cd-days').innerText = String(days).padStart(2, '0');
      document.getElementById('cd-hours').innerText = String(hours).padStart(2, '0');
      document.getElementById('cd-minutes').innerText = String(minutes).padStart(2, '0');
      document.getElementById('cd-seconds').innerText = String(seconds).padStart(2, '0');
    }

    setInterval(updateCountdown, 1000);
    updateCountdown();

    // 4. INTERACTIVE SEAT SELECTION ($15.000 Pesos per ticket)
    const TICKET_PRICE = 15000;
    const seatRows = ['A', 'B', 'C', 'D', 'E', 'F'];
    const seatsPerRow = 8;
    const preOccupiedSeats = new Set(['A3', 'A4', 'B5', 'C1', 'C2', 'D7', 'E3', 'E4']);
    let selectedSeats = new Set();

    const seatMatrix = document.getElementById('seatMatrix');
    const selectedSeatsLabel = document.getElementById('selectedSeatsLabel');
    const ticketCountLabel = document.getElementById('ticketCountLabel');
    const totalPriceLabel = document.getElementById('totalPriceLabel');
    const btnConfirmBooking = document.getElementById('btnConfirmBooking');
    const customerName = document.getElementById('customerName');
    const customerEmail = document.getElementById('customerEmail');

    // Generate seats grid
    seatRows.forEach(row => {
      const rowElem = document.createElement('div');
      rowElem.className = 'flex items-center gap-2 sm:gap-3';

      const rowLabel = document.createElement('span');
      rowLabel.className = 'w-4 text-xs font-bold text-slate-500 font-mono text-center';
      rowLabel.innerText = row;
      rowElem.appendChild(rowLabel);

      for (let c = 1; c <= seatsPerRow; c++) {
        const seatId = `${row}${c}`;
        const seatBtn = document.createElement('button');
        seatBtn.dataset.id = seatId;
        seatBtn.innerText = c;
        seatBtn.className = 'w-7 h-7 sm:w-9 sm:h-9 rounded-lg text-xs font-bold font-mono flex items-center justify-center transition-all duration-200 border';

        if (preOccupiedSeats.has(seatId)) {
          seatBtn.classList.add('bg-zinc-900', 'border-zinc-800', 'text-slate-700', 'cursor-not-allowed', 'opacity-40');
          seatBtn.disabled = true;
        } else {
          seatBtn.classList.add('bg-slate-800', 'border-slate-600', 'text-slate-300', 'hover:bg-amber-500', 'hover:border-amber-400', 'hover:text-black');
          seatBtn.addEventListener('click', () => toggleSeat(seatId, seatBtn));
        }

        rowElem.appendChild(seatBtn);
      }

      seatMatrix.appendChild(rowElem);
    });

    function toggleSeat(seatId, seatBtn) {
      if (selectedSeats.has(seatId)) {
        selectedSeats.delete(seatId);
        seatBtn.classList.remove('bg-bloodred', 'border-red-400', 'text-white', 'shadow-[0_0_10px_#ff1a1a]');
        seatBtn.classList.add('bg-slate-800', 'border-slate-600', 'text-slate-300');
      } else {
        selectedSeats.add(seatId);
        seatBtn.classList.remove('bg-slate-800', 'border-slate-600', 'text-slate-300');
        seatBtn.classList.add('bg-bloodred', 'border-red-400', 'text-white', 'shadow-[0_0_10px_#ff1a1a]');
      }
      updateSummary();
    }

    function updateSummary() {
      const seatsArr = Array.from(selectedSeats).sort();
      const count = seatsArr.length;
      const total = count * TICKET_PRICE;

      selectedSeatsLabel.innerText = count > 0 ? seatsArr.join(', ') : 'Ninguno';
      ticketCountLabel.innerText = count;
      totalPriceLabel.innerText = `$${total.toLocaleString('es-AR')} Pesos`;

      validateForm();
    }

    customerName.addEventListener('input', validateForm);
    customerEmail.addEventListener('input', validateForm);

    function validateForm() {
      const hasSeat = selectedSeats.size > 0;
      const hasName = customerName.value.trim().length > 0;
      const hasEmail = customerEmail.value.trim().length > 0;

      btnConfirmBooking.disabled = !(hasSeat && hasName && hasEmail);
    }

    // 5. TICKET MODAL HANDLERS
    const ticketModal = document.getElementById('ticketModal');

    function confirmTicketPurchase() {
      if (selectedSeats.size === 0) return;

      const randomRef = '#EGO-' + Math.floor(1000 + Math.random() * 9000);
      const seatsArr = Array.from(selectedSeats).sort().join(', ');
      const total = selectedSeats.size * TICKET_PRICE;

      document.getElementById('ticketRef').innerText = randomRef;
      document.getElementById('ticketModalName').innerText = customerName.value.trim();
      document.getElementById('ticketModalEmail').innerText = customerEmail.value.trim();
      document.getElementById('ticketModalSeats').innerText = seatsArr;
      document.getElementById('ticketModalTotal').innerText = `$${total.toLocaleString('es-AR')} Pesos`;

      ticketModal.classList.remove('opacity-0', 'pointer-events-none');
    }

    function closeTicketModal() {
      ticketModal.classList.add('opacity-0', 'pointer-events-none');

      selectedSeats.forEach(seatId => {
        preOccupiedSeats.add(seatId);
        const btn = seatMatrix.querySelector(`[data-id="${seatId}"]`);
        if (btn) {
          btn.disabled = true;
          btn.className = 'w-7 h-7 sm:w-9 sm:h-9 rounded-lg text-xs font-bold font-mono flex items-center justify-center border bg-zinc-900 border-zinc-800 text-slate-700 cursor-not-allowed opacity-40';
        }
      });

      selectedSeats.clear();
      customerName.value = '';
      customerEmail.value = '';
      updateSummary();
    }
  </script>
</body>
</html>
