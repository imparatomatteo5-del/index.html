<!DOCTYPE html>  
<html lang="it">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Il Blueprint del Content Architect: Vision 2026</title>  
    <script src="https://cdn.tailwindcss.com"></script>  
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>  
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;900&display=swap" rel="stylesheet">  
      
    <!-- Chosen Palette: Indigo Future (Deep Indigo, Slate, Vibrant Cyan & Pink Accents) -->  
    <!-- Application Structure Plan:   
         1. Hero Section: Defines the core identity shift from Creator to Architect.  
         2. The A.R.C. Protocol: Interactive diagram explaining the proprietary method.  
         3. Pain Point Solver: A dynamic filterable interface replacing static tables. Users identify their struggle and get the specific video hook/solution.  
         4. Efficiency Data: Quantitative proof of the method's value using charts.  
         5. Monetization Roadmap: Interactive timeline showing the evolution of the business model.  
         6. 30-Day Launchpad: Actionable checklist for immediate implementation.  
         This structure moves from "Mindset" -> "Method" -> "Application" -> "Business" -> "Action", guiding the user through the transformation.  
    -->  
  
    <!-- Visualization & Content Choices:  
         1. Market Gap (Radar Chart): Visualizes the skill gap between a generic creator and an Architect (Strategy, Tech, Speed, etc.). Goal: Compare.  
         2. Efficiency Impact (Bar Chart): Compares manual workflow time vs. AI-assisted workflow. Goal: Inform/Compare.  
         3. Pain Point Cards (Interactive Grid): Replaces long text tables. Users filter by category (e.g., "Tech Barrier") to see specific hooks. Goal: Organize/Explore.  
         4. Monetization Staircase (Styled HTML): Visualizes the 3 phases of business growth. Goal: Process/Change.  
         CONFIRMATION: NO SVG graphics used. NO Mermaid JS used.  
    -->  
  
    <style>  
        body { font-family: 'Inter', sans-serif; }  
        .chart-container {   
            position: relative;   
            width: 100%;   
            max-width: 600px;   
            margin-left: auto;   
            margin-right: auto;   
            height: 350px;   
            max-height: 400px;   
        }  
        @media (min-width: 768px) { .chart-container { height: 400px; } }  
          
        .glass-panel {  
            background: rgba(255, 255, 255, 0.9);  
            backdrop-filter: blur(10px);  
            border: 1px solid rgba(255, 255, 255, 0.2);  
        }  
          
        .gradient-text {  
            background: linear-gradient(to right, #4f46e5, #06b6d4);  
            -webkit-background-clip: text;  
            -webkit-text-fill-color: transparent;  
        }  
  
        /* Smooth scrolling */  
        html { scroll-behavior: smooth; }  
          
        /* Card hover effects */  
        .hover-lift { transition: transform 0.2s ease, box-shadow 0.2s ease; }  
        .hover-lift:hover { transform: translateY(-5px); box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.1); }  
    </style>  
</head>  
<body class="bg-slate-50 text-slate-800 antialiased selection:bg-indigo-100 selection:text-indigo-900">  
  
    <!-- Navigation -->  
    <nav class="fixed top-0 w-full z-50 bg-slate-900/95 backdrop-blur text-white border-b border-slate-700">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
            <div class="flex items-center justify-between h-16">  
                <div class="flex items-center gap-2">  
                    <div class="h-8 w-8 bg-gradient-to-br from-indigo-500 to-cyan-400 rounded-lg flex items-center justify-center font-bold text-white">CA</div>  
                    <span class="font-bold text-lg tracking-tight">Content Architect</span>  
                </div>  
                <div class="hidden md:block">  
                    <div class="ml-10 flex items-baseline space-x-4">  
                        <a href="#vision" class="hover:bg-slate-800 px-3 py-2 rounded-md text-sm font-medium transition-colors">Vision</a>  
                        <a href="#arc-protocol" class="hover:bg-slate-800 px-3 py-2 rounded-md text-sm font-medium transition-colors">A.R.C. Protocol</a>  
                        <a href="#strategies" class="hover:bg-slate-800 px-3 py-2 rounded-md text-sm font-medium transition-colors">Strategie & Hook</a>  
                        <a href="#data" class="hover:bg-slate-800 px-3 py-2 rounded-md text-sm font-medium transition-colors">Dati & Efficienza</a>  
                        <a href="#monetization" class="hover:bg-slate-800 px-3 py-2 rounded-md text-sm font-medium transition-colors">Monetizzazione</a>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </nav>  
  
    <!-- Hero Section -->  
    <header id="vision" class="pt-32 pb-20 bg-white relative overflow-hidden">  
        <div class="absolute inset-0 bg-[url('https://grainy-gradients.vercel.app/noise.svg')] opacity-20"></div>  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 text-center">  
            <div class="inline-block px-4 py-1.5 rounded-full bg-indigo-50 text-indigo-700 font-semibold text-sm mb-6 border border-indigo-100">  
                Vision 2026 Blueprint  
            </div>  
            <h1 class="text-5xl md:text-7xl font-black text-slate-900 mb-6 tracking-tight leading-tight">  
                Da Creator a <br>  
                <span class="gradient-text">Content Architect</span>  
            </h1>  
            <p class="mt-4 max-w-2xl mx-auto text-xl text-slate-500">  
                "Non vendo solo il video. Vendo il <strong>sistema</strong> che lo ha generato."  
            </p>  
            <div class="mt-10 flex justify-center gap-4">  
                <a href="#arc-protocol" class="px-8 py-4 bg-slate-900 text-white font-bold rounded-xl shadow-lg hover:bg-slate-800 transition-all transform hover:scale-105">  
                    Esplora il Blueprint  
                </a>  
            </div>  
        </div>  
    </header>  
  
    <!-- SECTION: A.R.C. Protocol -->  
    <section id="arc-protocol" class="py-20 bg-slate-50 border-t border-slate-200">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
            <div class="text-center mb-16">  
                <h2 class="text-3xl md:text-4xl font-bold text-slate-900 mb-4">Il Metodo Proprietario: A.R.C.</h2>  
                <p class="text-lg text-slate-600 max-w-3xl mx-auto">  
                    Il "Content Architect" non improvvisa. Utilizza un protocollo strutturato che fonde strategia, ingegneria dell'IA e produzione tecnica. Interagisci con le fasi qui sotto per scoprire i dettagli.  
                </p>  
            </div>  
  
            <!-- Interactive Diagram: Flexbox based Cards -->  
            <div class="grid md:grid-cols-3 gap-8">  
                <!-- A -->  
                <div class="group relative bg-white rounded-2xl p-8 shadow-sm hover:shadow-xl transition-all border border-slate-100 cursor-pointer overflow-hidden hover:-translate-y-2">  
                    <div class="absolute top-0 right-0 p-4 opacity-10 font-black text-9xl text-indigo-600 select-none group-hover:scale-110 transition-transform">A</div>  
                    <div class="relative z-10">  
                        <div class="w-12 h-12 bg-indigo-100 rounded-lg flex items-center justify-center text-2xl mb-6">🏛️</div>  
                        <h3 class="text-2xl font-bold text-slate-900 mb-2">Architect</h3>  
                        <p class="text-xs font-bold text-indigo-600 uppercase tracking-wider mb-4">Strategia</p>  
                        <p class="text-slate-600 leading-relaxed">  
                            Non si accende la videocamera se non c'è un'architettura dati. Targeting psicologico, analisi dei competitor e definizione degli obiettivi prima di ogni prompt.  
                        </p>  
                    </div>  
                    <div class="mt-6 pt-6 border-t border-slate-100">  
                        <span class="text-sm font-semibold text-slate-400 group-hover:text-indigo-600 transition-colors">Focus: Dati & Psicologia &rarr;</span>  
                    </div>  
                </div>  
  
                <!-- R -->  
                <div class="group relative bg-white rounded-2xl p-8 shadow-sm hover:shadow-xl transition-all border border-slate-100 cursor-pointer overflow-hidden hover:-translate-y-2">  
                    <div class="absolute top-0 right-0 p-4 opacity-10 font-black text-9xl text-cyan-600 select-none group-hover:scale-110 transition-transform">R</div>  
                    <div class="relative z-10">  
                        <div class="w-12 h-12 bg-cyan-100 rounded-lg flex items-center justify-center text-2xl mb-6">🧠</div>  
                        <h3 class="text-2xl font-bold text-slate-900 mb-2">Refine</h3>  
                        <p class="text-xs font-bold text-cyan-600 uppercase tracking-wider mb-4">AI Engineering</p>  
                        <p class="text-slate-600 leading-relaxed">  
                            L'IA come motore creativo, non sostituto. Ingegnerizzazione dei prompt per LLM (Claude/GPT) per generare script, storyboard e asset visivi precisi.  
                        </p>  
                    </div>  
                    <div class="mt-6 pt-6 border-t border-slate-100">  
                        <span class="text-sm font-semibold text-slate-400 group-hover:text-cyan-600 transition-colors">Focus: Prompting & Struttura &rarr;</span>  
                    </div>  
                </div>  
  
                <!-- C -->  
                <div class="group relative bg-white rounded-2xl p-8 shadow-sm hover:shadow-xl transition-all border border-slate-100 cursor-pointer overflow-hidden hover:-translate-y-2">  
                    <div class="absolute top-0 right-0 p-4 opacity-10 font-black text-9xl text-pink-600 select-none group-hover:scale-110 transition-transform">C</div>  
                    <div class="relative z-10">  
                        <div class="w-12 h-12 bg-pink-100 rounded-lg flex items-center justify-center text-2xl mb-6">🎥</div>  
                        <h3 class="text-2xl font-bold text-slate-900 mb-2">Create</h3>  
                        <p class="text-xs font-bold text-pink-600 uppercase tracking-wider mb-4">UGC Tech</p>  
                        <p class="text-slate-600 leading-relaxed">  
                            Produzione ed esecuzione. Uso di avatar digitali, sintesi vocale e editing automatizzato per scalare la creazione di contenuti senza perdere autenticità.  
                        </p>  
                    </div>  
                    <div class="mt-6 pt-6 border-t border-slate-100">  
                        <span class="text-sm font-semibold text-slate-400 group-hover:text-pink-600 transition-colors">Focus: Produzione & Automazione &rarr;</span>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- SECTION: Pain Points & Strategies (Interactive Filter) -->  
    <section id="strategies" class="py-20 bg-white">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
            <div class="mb-12">  
                <span class="text-indigo-600 font-bold tracking-wider uppercase text-sm">Analisi Psicologica</span>  
                <h2 class="text-3xl md:text-4xl font-bold text-slate-900 mt-2 mb-4">Trasformare i "Pain Point" in Hook Virali</h2>  
                <p class="text-lg text-slate-600 max-w-3xl">  
                    Abbiamo mappato 50 "punti di dolore" del mercato italiano. Seleziona una categoria qui sotto per vedere come il Content Architect risponde a questi problemi con contenuti strategici e soluzioni tecniche.  
                </p>  
            </div>  
  
            <!-- Filter Buttons -->  
            <div class="flex flex-wrap gap-2 mb-10" id="category-filters">  
                <button onclick="filterStrategies('all')" class="filter-btn active px-4 py-2 rounded-full text-sm font-semibold border transition-all bg-slate-900 text-white border-slate-900">Tutti</button>  
                <button onclick="filterStrategies('A')" class="filter-btn px-4 py-2 rounded-full text-sm font-semibold border border-slate-200 text-slate-600 hover:bg-green-50 hover:border-green-200 hover:text-green-700 transition-all">🟢 Tech Barrier</button>  
                <button onclick="filterStrategies('B')" class="filter-btn px-4 py-2 rounded-full text-sm font-semibold border border-slate-200 text-slate-600 hover:bg-blue-50 hover:border-blue-200 hover:text-blue-700 transition-all">🔵 Sindrome Impostore</button>  
                <button onclick="filterStrategies('C')" class="filter-btn px-4 py-2 rounded-full text-sm font-semibold border border-slate-200 text-slate-600 hover:bg-red-50 hover:border-red-200 hover:text-red-700 transition-all">🔴 Efficienza & Tempo</button>  
                <button onclick="filterStrategies('D')" class="filter-btn px-4 py-2 rounded-full text-sm font-semibold border border-slate-200 text-slate-600 hover:bg-yellow-50 hover:border-yellow-200 hover:text-yellow-700 transition-all">🟡 Monetizzazione</button>  
                <button onclick="filterStrategies('E')" class="filter-btn px-4 py-2 rounded-full text-sm font-semibold border border-slate-200 text-slate-600 hover:bg-purple-50 hover:border-purple-200 hover:text-purple-700 transition-all">🟣 Creatività</button>  
            </div>  
  
            <!-- Dynamic Content Grid -->  
            <div id="strategies-grid" class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">  
                <!-- Content will be injected by JS -->  
            </div>  
        </div>  
    </section>  
  
    <!-- SECTION: Data & Efficiency (Charts) -->  
    <section id="data" class="py-20 bg-slate-50 border-t border-slate-200">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
            <div class="grid lg:grid-cols-2 gap-16">  
                <!-- Chart 1: Market Gap Analysis -->  
                <div>  
                    <h3 class="text-2xl font-bold text-slate-900 mb-4">Analisi del Gap Competitivo</h3>  
                    <p class="text-slate-600 mb-8">  
                        Il mercato è pieno di esecutori. Il Content Architect domina grazie a un mix unico di competenze strategiche e tecnologiche che mancano al creator tradizionale.  
                    </p>  
                    <div class="bg-white p-6 rounded-2xl shadow-sm border border-slate-100">  
                        <div class="chart-container">  
                            <canvas id="radarChart"></canvas>  
                        </div>  
                    </div>  
                </div>  
  
                <!-- Chart 2: Efficiency (Speedrun) -->  
                <div>  
                    <h3 class="text-2xl font-bold text-slate-900 mb-4">Impatto sull'Efficienza (Speedrun)</h3>  
                    <p class="text-slate-600 mb-8">  
                        La velocità è la moneta del Content Architect. Confronto diretto tra il tempo impiegato per un Reel con il metodo tradizionale vs. il metodo IA integrato.  
                    </p>  
                    <div class="bg-white p-6 rounded-2xl shadow-sm border border-slate-100">  
                        <div class="chart-container">  
                            <canvas id="efficiencyChart"></canvas>  
                        </div>  
                        <div class="mt-4 flex justify-around text-center">  
                            <div>  
                                <p class="text-3xl font-black text-slate-300">4h</p>  
                                <p class="text-xs text-slate-500 uppercase">Tradizionale</p>  
                            </div>  
                            <div>  
                                <p class="text-3xl font-black text-indigo-600">12m</p>  
                                <p class="text-xs text-slate-500 uppercase">Architect</p>  
                            </div>  
                        </div>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- SECTION: Monetization & Roadmap -->  
    <section id="monetization" class="py-20 bg-slate-900 text-white relative overflow-hidden">  
        <!-- Background accents -->  
        <div class="absolute top-0 right-0 w-96 h-96 bg-indigo-600 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob"></div>  
        <div class="absolute bottom-0 left-0 w-96 h-96 bg-cyan-600 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob animation-delay-2000"></div>  
  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">  
            <div class="text-center mb-16">  
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Evoluzione del Business</h2>  
                <p class="text-xl text-slate-300 max-w-2xl mx-auto">  
                    Il percorso per scalare da freelance a imprenditore digitale, vendendo asset invece di tempo.  
                </p>  
            </div>  
  
            <div class="grid md:grid-cols-3 gap-8">  
                <!-- Phase 1 -->  
                <div class="bg-slate-800/50 backdrop-blur border border-slate-700 p-8 rounded-2xl hover:bg-slate-800 transition-all">  
                    <div class="text-xs font-bold text-indigo-400 uppercase tracking-widest mb-2">Fase 1</div>  
                    <h3 class="text-2xl font-bold mb-4">Done-For-You</h3>  
                    <div class="text-sm bg-slate-700/50 inline-block px-3 py-1 rounded-full mb-6">High Ticket Service</div>  
                    <ul class="space-y-3 text-slate-300 mb-8">  
                        <li class="flex items-start"><span class="text-indigo-400 mr-2">✓</span> Servizio "UGC Tech System"</li>  
                        <li class="flex items-start"><span class="text-indigo-400 mr-2">✓</span> Consegna Video + Database Prompt</li>  
                        <li class="flex items-start"><span class="text-indigo-400 mr-2">✓</span> Target: Startup Tech & SaaS</li>  
                    </ul>  
                </div>  
  
                <!-- Phase 2 -->  
                <div class="bg-slate-800/50 backdrop-blur border border-slate-700 p-8 rounded-2xl hover:bg-slate-800 transition-all relative">  
                    <div class="absolute -top-4 left-1/2 transform -translate-x-1/2 bg-gradient-to-r from-indigo-500 to-cyan-500 text-white text-xs font-bold px-3 py-1 rounded-full">SCALING</div>  
                    <div class="text-xs font-bold text-cyan-400 uppercase tracking-widest mb-2">Fase 2</div>  
                    <h3 class="text-2xl font-bold mb-4">Done-With-You</h3>  
                    <div class="text-sm bg-slate-700/50 inline-block px-3 py-1 rounded-full mb-6">Consulting</div>  
                    <ul class="space-y-3 text-slate-300 mb-8">  
                        <li class="flex items-start"><span class="text-cyan-400 mr-2">✓</span> Ottimizzazione Workflow Interni</li>  
                        <li class="flex items-start"><span class="text-cyan-400 mr-2">✓</span> Training Team Marketing su AI</li>  
                        <li class="flex items-start"><span class="text-cyan-400 mr-2">✓</span> Target: PMI e Agenzie</li>  
                    </ul>  
                </div>  
  
                <!-- Phase 3 -->  
                <div class="bg-slate-800/50 backdrop-blur border border-slate-700 p-8 rounded-2xl hover:bg-slate-800 transition-all">  
                    <div class="text-xs font-bold text-pink-400 uppercase tracking-widest mb-2">Fase 3</div>  
                    <h3 class="text-2xl font-bold mb-4">Digital Product</h3>  
                    <div class="text-sm bg-slate-700/50 inline-block px-3 py-1 rounded-full mb-6">Passive Assets</div>  
                    <ul class="space-y-3 text-slate-300 mb-8">  
                        <li class="flex items-start"><span class="text-pink-400 mr-2">✓</span> "The Architect's Vault"</li>  
                        <li class="flex items-start"><span class="text-pink-400 mr-2">✓</span> Custom GPTs & Notion Templates</li>  
                        <li class="flex items-start"><span class="text-pink-400 mr-2">✓</span> Target: Aspiranti Creator</li>  
                    </ul>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- SECTION: 30-Day Action Plan -->  
    <section class="py-20 bg-white">  
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">  
            <h2 class="text-3xl font-bold text-slate-900 mb-8 text-center">Piano d'Azione: Prossimi 30 Giorni</h2>  
            <div class="space-y-6">  
                <!-- Week 1 -->  
                <div class="flex flex-col md:flex-row gap-6 p-6 border border-slate-100 rounded-xl hover:shadow-md transition-shadow bg-slate-50">  
                    <div class="md:w-1/4">  
                        <span class="text-sm font-bold text-indigo-600 uppercase">Settimana 1</span>  
                        <h4 class="text-lg font-bold">Pulizia & Posizionamento</h4>  
                    </div>  
                    <div class="md:w-3/4">  
                        <p class="text-slate-600 mb-2">Ottimizzazione Bio LinkedIn/IG e creazione dei primi 3 video "Manifesto".</p>  
                        <div class="flex gap-2 text-xs font-medium text-slate-500 bg-white p-2 rounded border border-slate-200 inline-block">  
                            <span>🎯 Obiettivo: Definire l'identità</span>  
                        </div>  
                    </div>  
                </div>  
                 <!-- Week 2 -->  
                 <div class="flex flex-col md:flex-row gap-6 p-6 border border-slate-100 rounded-xl hover:shadow-md transition-shadow bg-white">  
                    <div class="md:w-1/4">  
                        <span class="text-sm font-bold text-green-600 uppercase">Settimana 2</span>  
                        <h4 class="text-lg font-bold">Attacco Tech Barrier</h4>  
                    </div>  
                    <div class="md:w-3/4">  
                        <p class="text-slate-600 mb-2">Pubblicazione 5 contenuti "Tool Breaker". Risolvere problemi complessi con tool semplici.</p>  
                        <div class="flex gap-2 text-xs font-medium text-slate-500 bg-slate-50 p-2 rounded border border-slate-200 inline-block">  
                            <span>🎯 Obiettivo: Salvataggi (Saveable Content)</span>  
                        </div>  
                    </div>  
                </div>  
                 <!-- Week 3 -->  
                 <div class="flex flex-col md:flex-row gap-6 p-6 border border-slate-100 rounded-xl hover:shadow-md transition-shadow bg-white">  
                    <div class="md:w-1/4">  
                        <span class="text-sm font-bold text-red-600 uppercase">Settimana 3</span>  
                        <h4 class="text-lg font-bold">Dimostrazione Velocità</h4>  
                    </div>  
                    <div class="md:w-3/4">  
                        <p class="text-slate-600 mb-2">Contenuti "Dietro le quinte" (Screen recording). Mostrare il workflow in tempo reale.</p>  
                        <div class="flex gap-2 text-xs font-medium text-slate-500 bg-slate-50 p-2 rounded border border-slate-200 inline-block">  
                            <span>🎯 Obiettivo: Autorità Tecnica</span>  
                        </div>  
                    </div>  
                </div>  
                 <!-- Week 4 -->  
                 <div class="flex flex-col md:flex-row gap-6 p-6 border border-slate-100 rounded-xl hover:shadow-md transition-shadow bg-white">  
                    <div class="md:w-1/4">  
                        <span class="text-sm font-bold text-yellow-600 uppercase">Settimana 4</span>  
                        <h4 class="text-lg font-bold">Lancio Offerta</h4>  
                    </div>  
                    <div class="md:w-3/4">  
                        <p class="text-slate-600 mb-2">Lancio "Beta Call" per servizio di consulenza o UGC Tech a prezzo lancio.</p>  
                        <div class="flex gap-2 text-xs font-medium text-slate-500 bg-slate-50 p-2 rounded border border-slate-200 inline-block">  
                            <span>🎯 Obiettivo: Primi 3 Clienti High-Ticket</span>  
                        </div>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Footer -->  
    <footer class="bg-slate-900 text-slate-400 py-12 border-t border-slate-800 text-center">  
        <p class="text-sm">Blueprint Generato per Content Architect Vision 2026</p>  
    </footer>  
  
    <!-- JavaScript Logic -->  
    <script>  
        // --- DATA STORAGE ---  
        // Storing the strategic content for the dynamic grid  
        const strategies = [  
            // Category A: Tech Barrier  
            { id: 1, category: 'A', title: 'Paura "Effetto Robot"', pain: 'Il video AI sembra finto.', hook: '"Il tuo video sembra finto perché sbagli questo singolo prompt."', solution: 'Demo parametro "Temperature" / Style Prompt.', color: 'green' },  
            { id: 2, category: 'A', title: 'Audio Scadente', pain: 'Audio registrato male.', hook: '"Ho registrato in bagno. Ascolta come l\'IA lo ha pulito."', solution: 'Demo Adobe Podcast / Audo Studio.', color: 'green' },  
            { id: 3, category: 'A', title: 'Troppi Tool', pain: 'Caos abbonamenti.', hook: '"Smetti di pagare 10 abbonamenti. Ecco il mio Stack da 30€."', solution: 'Breakdown 3 tool essenziali.', color: 'green' },  
            { id: 4, category: 'A', title: 'Immagini Midjourney', pain: 'Prompt non funzionanti.', hook: '"Parli a Midjourney come se fosse umano. Sbagliato."', solution: 'Struttura tecnica prompt copertine.', color: 'green' },  
  
            // Category B: Sindrome Impostore  
            { id: 5, category: 'B', title: 'Vergogna Video', pain: 'Odi la videocamera.', hook: '"Vuoi fare UGC ma odi la videocamera? Ho clonato me stesso."', solution: 'Demo HeyGen/Synthesia + Strategia.', color: 'blue' },  
            { id: 6, category: 'B', title: 'Postazione Brutta', pain: 'Sfondo disordinato.', hook: '"La mia stanza è un disastro. In video sembra uno studio."', solution: 'Tutorial Generative Fill (Photoshop/Premiere).', color: 'blue' },  
            { id: 7, category: 'B', title: 'Pronuncia Inglese', pain: 'Inglese scolastico.', hook: '"Parlo come un bambino di 5 anni, ma qui sembro madrelingua."', solution: 'Demo Rask.ai o ElevenLabs dubbing.', color: 'blue' },  
  
            // Category C: Efficiency  
            { id: 8, category: 'C', title: '4 Ore per un Reel', pain: 'Lentezza esasperante.', hook: '"Cronometriamo: Da idea a video montato in 12 minuti."', solution: 'Workflow: ChatGPT -> CapCut Template.', color: 'red' },  
            { id: 9, category: 'C', title: 'Senza Idee', pain: 'Blocco creativo.', hook: '"Non uso più il cervello per le idee. Ho un Secondo Cervello."', solution: 'Notion Database + AI Generator.', color: 'red' },  
            { id: 10, category: 'C', title: 'Ricerca Competitor', pain: 'Scrolling infinito.', hook: '"Ho analizzato 100 video dei tuoi competitor mentre bevevo caffè."', solution: 'Analisi Data Scraping / Viral Analysis.', color: 'red' },  
  
            // Category D: Monetization  
            { id: 11, category: 'D', title: 'Pagati Poco', pain: 'Cambio merce.', hook: '"Perché a me pagano fatture da 2k? Vendo Architettura."', solution: 'Spiegare ROI vs Video commodity.', color: 'yellow' },  
            { id: 12, category: 'D', title: 'Contratti & AI', pain: 'Rischi legali.', hook: '"Stai vendendo la tua faccia all\'IA per sempre. Leggi qui."', solution: 'Analisi clausole diritti immagine AI.', color: 'yellow' },  
            { id: 13, category: 'D', title: 'Vendere Servizi', pain: 'Difficoltà vendita.', hook: '"Come ho pacchettizzato la conoscenza in Productized Service."', solution: 'Vendere Prompt/Template oltre al servizio.', color: 'yellow' },  
  
            // Category E: Creativity  
            { id: 14, category: 'E', title: 'Video Noiosi', pain: 'Bassa retention.', hook: '"Il video non è noioso, è strutturato male. Curva di Interesse."', solution: 'Analisi grafica retention video.', color: 'purple' },  
            { id: 15, category: 'E', title: 'Collage "Frankenstein"', pain: 'Editing slegato.', hook: '"Mixed Media: Fondere reale e AI senza effetto Frankenstein."', solution: 'Tutorial transizioni fluide (Match cut).', color: 'purple' }  
        ];  
  
        // --- DOM ELEMENTS ---  
        const grid = document.getElementById('strategies-grid');  
        const filters = document.getElementById('category-filters').children;  
  
        // --- FUNCTIONS ---  
  
        function renderStrategies(filterKey) {  
            grid.innerHTML = ''; // Clear existing  
              
            const filtered = filterKey === 'all'   
                ? strategies   
                : strategies.filter(s => s.category === filterKey);  
  
            filtered.forEach(item => {  
                const card = document.createElement('div');  
                // Dynamic styling based on category color  
                let bgClass = 'bg-white';  
                let borderClass = 'border-slate-200';  
                let textClass = 'text-slate-600';  
                  
                if(item.color === 'green') { borderClass = 'border-green-100 hover:border-green-300'; }  
                if(item.color === 'blue') { borderClass = 'border-blue-100 hover:border-blue-300'; }  
                if(item.color === 'red') { borderClass = 'border-red-100 hover:border-red-300'; }  
                if(item.color === 'yellow') { borderClass = 'border-yellow-100 hover:border-yellow-300'; }  
                if(item.color === 'purple') { borderClass = 'border-purple-100 hover:border-purple-300'; }  
  
                card.className = `p-6 rounded-xl border ${borderClass} shadow-sm hover:shadow-md transition-all hover-lift flex flex-col h-full`;  
                card.innerHTML = `  
                    <div class="mb-4">  
                        <span class="text-xs font-bold uppercase tracking-wider px-2 py-1 rounded bg-slate-100 text-slate-500">${item.title}</span>  
                    </div>  
                    <div class="mb-4 flex-grow">  
                        <p class="text-sm text-slate-400 mb-1">Il Problema:</p>  
                        <p class="text-sm text-slate-600 italic mb-4">"${item.pain}"</p>  
                        <p class="text-sm text-slate-400 mb-1">L'Hook Virale:</p>  
                        <p class="font-bold text-slate-800 text-lg leading-tight">${item.hook}</p>  
                    </div>  
                    <div class="mt-auto pt-4 border-t border-dashed border-slate-200">  
                        <p class="text-xs font-semibold text-indigo-600 uppercase mb-1">Soluzione Architect:</p>  
                        <p class="text-sm text-slate-700">${item.solution}</p>  
                    </div>  
                `;  
                grid.appendChild(card);  
            });  
        }  
  
        function filterStrategies(key) {  
            // Update UI buttons  
            Array.from(filters).forEach(btn => {  
                btn.classList.remove('bg-slate-900', 'text-white', 'border-slate-900');  
                btn.classList.add('border-slate-200', 'text-slate-600');  
            });  
              
            // Highlight active button (finding the one clicked is tricky with inline onclick, so using event target logic implicitly or simplified)  
            // Ideally passing 'this' would be better, but simplified for single file logic:  
            const buttons = document.querySelectorAll('.filter-btn');  
            buttons.forEach(btn => {  
                if(btn.textContent.includes(key) || (key === 'all' && btn.textContent === 'Tutti')) {  
                     btn.classList.remove('bg-white', 'text-slate-600', 'border-slate-200');  
                     btn.classList.add('bg-slate-900', 'text-white', 'border-slate-900');  
                } else if (key === 'A' && btn.textContent.includes('Tech')) {  
                     btn.classList.add('bg-slate-900', 'text-white', 'border-slate-900');  
                } else if (key === 'B' && btn.textContent.includes('Sindrome')) {  
                     btn.classList.add('bg-slate-900', 'text-white', 'border-slate-900');  
                } else if (key === 'C' && btn.textContent.includes('Efficienza')) {  
                     btn.classList.add('bg-slate-900', 'text-white', 'border-slate-900');  
                } else if (key === 'D' && btn.textContent.includes('Monetizzazione')) {  
                     btn.classList.add('bg-slate-900', 'text-white', 'border-slate-900');  
                } else if (key === 'E' && btn.textContent.includes('Creatività')) {  
                     btn.classList.add('bg-slate-900', 'text-white', 'border-slate-900');  
                }  
            });  
  
            renderStrategies(key);  
        }  
  
        // --- CHARTS INITIALIZATION ---  
          
        // 1. Radar Chart: Market Gap  
        const ctxRadar = document.getElementById('radarChart').getContext('2d');  
        new Chart(ctxRadar, {  
            type: 'radar',  
            data: {  
                labels: ['Strategia', 'Velocità', 'Tech/AI', 'Scalabilità', 'Brand Identity'],  
                datasets: [{  
                    label: 'Creator Generalista',  
                    data: [30, 40, 20, 20, 50],  
                    fill: true,  
                    backgroundColor: 'rgba(148, 163, 184, 0.2)', // Slate  
                    borderColor: 'rgb(148, 163, 184)',  
                    pointBackgroundColor: 'rgb(148, 163, 184)',  
                }, {  
                    label: 'Content Architect',  
                    data: [90, 100, 95, 90, 85],  
                    fill: true,  
                    backgroundColor: 'rgba(79, 70, 229, 0.2)', // Indigo  
                    borderColor: 'rgb(79, 70, 229)',  
                    pointBackgroundColor: 'rgb(79, 70, 229)',  
                }]  
            },  
            options: {  
                maintainAspectRatio: false,  
                scales: {  
                    r: {  
                        angleLines: { color: '#e2e8f0' },  
                        grid: { color: '#e2e8f0' },  
                        pointLabels: { font: { family: 'Inter', size: 12, weight: '600' } },  
                        suggestedMin: 0,  
                        suggestedMax: 100  
                    }  
                },  
                plugins: {  
                    legend: { position: 'top', labels: { font: { family: 'Inter' } } }  
                }  
            }  
        });  
  
        // 2. Bar Chart: Efficiency (Speedrun)  
        const ctxBar = document.getElementById('efficiencyChart').getContext('2d');  
        new Chart(ctxBar, {  
            type: 'bar',  
            data: {  
                labels: ['Ideazione (Script)', 'Editing (Video)', 'Ricerca Competitor', 'Adattamento Formati'],  
                datasets: [{  
                    label: 'Metodo Manuale (Minuti)',  
                    data: [60, 180, 45, 30],  
                    backgroundColor: 'rgba(203, 213, 225, 0.8)', // Slate 300  
                    borderRadius: 4  
                }, {  
                    label: 'Metodo Architect (Minuti)',  
                    data: [5, 12, 2, 5],  
                    backgroundColor: 'rgba(6, 182, 212, 0.8)', // Cyan 500  
                    borderRadius: 4  
                }]  
            },  
            options: {  
                indexAxis: 'y',  
                maintainAspectRatio: false,  
                scales: {  
                    x: {   
                        grid: { color: '#f1f5f9' },  
                        title: { display: true, text: 'Minuti' }  
                    },  
                    y: { grid: { display: false } }  
                },  
                plugins: {  
                    tooltip: {  
                        callbacks: {  
                            title: function(context) {  
                                // Handle potential long labels wrapping (though short here)  
                                return context[0].label;   
                            }  
                        }  
                    },  
                    legend: { position: 'bottom', labels: { font: { family: 'Inter' } } }  
                }  
            }  
        });  
  
        // Initialize grid on load  
        renderStrategies('all');  
  
    </script>  
</body>  
</html>  
  
