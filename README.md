<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Asesoría Legal Laboral | Dra. Maria Lucila Toloza - Especialista en Derecho Laboral</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Inter', sans-serif; }
        .serif { font-family: 'Playfair Display', serif; }
        .step-inactive { display: none; }
        .progress-circle { transition: all 0.3s ease; }
        .btn-option:hover { border-color: #1e40af; background-color: #f0f9ff; }
        .btn-selected { border-color: #1e40af; background-color: #eff6ff; box-shadow: 0 0 0 2px #1e40af; }
        .gradient-gold { background: linear-gradient(135deg, #c5a059 0%, #9e7e43 100%); }
        .hero-overlay { background: linear-gradient(to right, rgba(15, 23, 42, 0.95), rgba(15, 23, 42, 0.7)); }
    </style>
</head>
<body class="bg-[#fcfcf9] text-slate-900 overflow-x-hidden">

    <nav class="bg-white/90 backdrop-blur-md border-b sticky top-0 z-[100] px-6 py-3">
        <div class="max-w-7xl mx-auto flex justify-between items-center">
            <div class="flex items-center gap-4">
                <div class="w-12 h-12 bg-slate-900 rounded-xl flex items-center justify-center text-white text-2xl">
                    <i class="fas fa-balance-scale"></i>
                </div>
                <div class="hidden sm:block border-l-2 border-slate-100 pl-4">
                    <span class="block font-bold text-slate-800 leading-tight tracking-tight text-lg uppercase">Asesoría Laboral</span>
                    <span class="text-[10px] uppercase tracking-[0.2em] text-slate-500 font-bold">Defensa del Trabajador</span>
                </div>
            </div>
            <div class="hidden md:flex items-center gap-8 text-sm font-semibold text-slate-600">
                <a href="#especialidades" class="hover:text-blue-700 transition">Especialidades</a>
                <button onclick="scrollToConsult()" class="bg-slate-900 text-white px-6 py-3 rounded-full hover:bg-blue-800 transition shadow-lg">
                    Iniciar Consulta
                </button>
            </div>
        </div>
    </nav>

    <section class="relative min-h-[75vh] flex items-center bg-slate-900 text-white overflow-hidden">
        <div class="absolute inset-0 z-0">
            <img src="https://images.unsplash.com/photo-1589829545856-d10d557cf95f?auto=format&fit=crop&q=80&w=2000" alt="Legal Background" class="w-full h-full object-cover opacity-30">
            <div class="absolute inset-0 hero-overlay"></div>
        </div>
        <div class="max-w-7xl mx-auto px-6 relative z-10 grid md:grid-cols-2 gap-12 items-center">
            <div>
                <span class="inline-block px-4 py-1 rounded-full bg-blue-500/20 border border-blue-400/30 text-blue-300 text-xs font-bold uppercase tracking-widest mb-6">Expertos en Derecho Laboral</span>
                <h1 class="serif text-4xl md:text-6xl mb-6 leading-tight">Tu trabajo es tu dignidad. <br><span class="text-blue-400">Defendemos tus derechos.</span></h1>
                <p class="text-slate-300 text-lg mb-8 max-w-lg leading-relaxed">
                    Bajo la dirección de la Dra. Maria Lucila Toloza, brindamos soluciones legales efectivas en despidos, accidentes laborales y reclamos contra ART.
                </p>
                <div class="flex flex-wrap gap-4">
                    <button onclick="scrollToConsult()" class="bg-blue-600 hover:bg-blue-500 px-8 py-4 rounded-xl font-bold transition shadow-xl shadow-blue-900/20">Consulta Gratis por WhatsApp</button>
                </div>
            </div>
        </div>
    </section>

    <section id="especialidades" class="py-24 max-w-7xl mx-auto px-6">
        <div class="text-center mb-16">
            <h2 class="serif text-3xl md:text-4xl mb-4">Áreas de Especialización</h2>
            <div class="w-20 h-1 gradient-gold mx-auto rounded-full"></div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 hover:shadow-xl transition-all">
                <div class="w-14 h-14 bg-blue-50 rounded-2xl flex items-center justify-center text-blue-600 mb-6">
                    <i class="fas fa-briefcase-medical text-2xl"></i>
                </div>
                <h3 class="font-bold text-xl mb-3">Accidentes Laborales</h3>
                <p class="text-sm text-slate-500 leading-relaxed">Representación integral ante accidentes de trabajo o enfermedades profesionales.</p>
            </div>
            <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 hover:shadow-xl transition-all">
                <div class="w-14 h-14 bg-amber-50 rounded-2xl flex items-center justify-center text-amber-600 mb-6">
                    <i class="fas fa-building-shield text-2xl"></i>
                </div>
                <h3 class="font-bold text-xl mb-3">Reclamos ART</h3>
                <p class="text-sm text-slate-500 leading-relaxed">Gestión de divergencias médicas y determinación de incapacidades laborales.</p>
            </div>
            <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 hover:shadow-xl transition-all">
                <div class="w-14 h-14 bg-red-50 rounded-2xl flex items-center justify-center text-red-600 mb-6">
                    <i class="fas fa-user-minus text-2xl"></i>
                </div>
                <h3 class="font-bold text-xl mb-3">Despidos e Indemnizaciones</h3>
                <p class="text-sm text-slate-500 leading-relaxed">Cálculo y reclamo de indemnizaciones por despido directo, indirecto o falta de registro.</p>
            </div>
        </div>
    </section>

    <section id="consultar" class="bg-slate-50 py-24 px-6 border-y border-slate-200">
        <div id="client-ui" class="max-w-3xl mx-auto">
            <div class="text-center mb-12">
                <h2 class="serif text-3xl md:text-4xl mb-4">Iniciá tu Consulta</h2>
                <p class="text-slate-500">Completá el formulario para un análisis preliminar de tu caso.</p>
            </div>

            <div class="bg-white rounded-[2.5rem] shadow-2xl p-8 md:p-12">
                <div id="step-1">
                    <h3 class="text-2xl font-bold mb-8">Información de Contacto</h3>
                    <div class="grid md:grid-cols-2 gap-6 mb-8">
                        <div>
                            <label class="block text-xs font-bold uppercase text-slate-400 mb-2">Nombre y Apellido *</label>
                            <input type="text" id="nombre" class="w-full bg-slate-50 border-0 rounded-2xl p-4 outline-none focus:ring-2 focus:ring-blue-100" placeholder="Ej: Juan Pérez">
                        </div>
                        <div>
                            <label class="block text-xs font-bold uppercase text-slate-400 mb-2">WhatsApp *</label>
                            <input type="text" id="tel" class="w-full bg-slate-50 border-0 rounded-2xl p-4 outline-none focus:ring-2 focus:ring-blue-100" placeholder="Ej: +54 9 351...">
                        </div>
                    </div>
                    <div class="mb-8">
                        <label class="block text-xs font-bold uppercase text-slate-400 mb-2">Contanos qué pasó *</label>
                        <textarea id="detalle" rows="4" class="w-full bg-slate-50 border-0 rounded-2xl p-4 outline-none resize-none" placeholder="Describe brevemente tu situación laboral..."></textarea>
                    </div>
                    <button onclick="submitForm()" id="btn-submit" class="w-full bg-green-600 text-white py-6 rounded-2xl font-bold text-xl hover:bg-green-700 transition shadow-xl flex items-center justify-center gap-3">
                        <i class="fab fa-whatsapp text-2xl"></i> Enviar Consulta
                    </button>
                </div>

                <div id="step-6" class="step-inactive text-center py-8">
                    <div class="w-20 h-20 bg-green-100 text-green-600 rounded-full flex items-center justify-center mx-auto mb-6 text-3xl">
                        <i class="fas fa-check"></i>
                    </div>
                    <h3 class="serif text-3xl font-bold mb-4">¡Consulta Enviada!</h3>
                    <p class="text-slate-500 mb-8">Se ha abierto WhatsApp para iniciar la conversación. Si no ocurrió, hacé clic abajo.</p>
                    <a id="retry-wa" href="#" target="_blank" class="bg-slate-900 text-white px-8 py-4 rounded-full font-bold">Abrir Chat Manualmente</a>
                </div>
            </div>
        </div>
    </section>

    <footer class="bg-white border-t border-slate-100 py-16 px-6">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-12">
            <div class="flex flex-col items-center md:items-start gap-4">
                <div class="w-16 h-16 bg-slate-900 rounded-2xl flex items-center justify-center text-white text-3xl">
                    <i class="fas fa-balance-scale"></i>
                </div>
                <div class="text-center md:text-left">
                    <p class="font-bold text-slate-900 text-lg serif italic">Asesoría Legal Laboral</p>
                    <p class="text-[10px] tracking-[0.2em] uppercase text-blue-600 font-bold mt-1">Dra. Maria Lucila Toloza - Especialista</p>
                </div>
            </div>
            
            <div class="flex flex-col items-center md:items-end gap-6">
                <p class="text-sm font-bold text-slate-400 uppercase tracking-widest">Contacto Directo</p>
                <a href="https://wa.me/message/6TW3IKTVAFXDP1" target="_blank" class="flex items-center gap-3 bg-green-50 text-green-700 px-8 py-4 rounded-2xl font-bold border border-green-100 hover:bg-green-100 transition">
                    <i class="fab fa-whatsapp text-2xl"></i>
                    <span>Hablar por WhatsApp</span>
                </a>
                <p class="text-[10px] text-slate-300">© 2024 · Córdoba, Argentina · Asesoría Legal Laboral</p>
            </div>
        </div>
    </footer>

    <script>
        const TELEFONO_ESTUDIO = "5493515116958"; 

        function scrollToConsult() {
            document.getElementById('consultar').scrollIntoView({ behavior: 'smooth' });
        }

        async function submitForm() {
            const nombre = document.getElementById('nombre').value;
            const tel = document.getElementById('tel').value;
            const detalle = document.getElementById('detalle').value;

            if(!nombre || !tel || !detalle) {
                const errorMsg = "Por favor completa los campos obligatorios.";
                alert(errorMsg);
                return;
            }

            const btn = document.getElementById('btn-submit');
            btn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> Procesando...';

            const textWA = `⚖️ *CONSULTA WEB - ASESORÍA LABORAL*\n` +
                           `----------------------------------\n` +
                           `👤 *CLIENTE:* ${nombre}\n` +
                           `📱 *WHATSAPP:* ${tel}\n\n` +
                           `📝 *SITUACIÓN:* ${detalle}\n` +
                           `----------------------------------`;
            
            const waLink = `https://wa.me/${TELEFONO_ESTUDIO}?text=${encodeURIComponent(textWA)}`;

            setTimeout(() => {
                window.open(waLink, '_blank');
                document.getElementById('step-1').classList.add('step-inactive');
                document.getElementById('step-6').classList.remove('step-inactive');
                document.getElementById('retry-wa').href = waLink;
            }, 800);
        }
    </script>
</body>
</html>
