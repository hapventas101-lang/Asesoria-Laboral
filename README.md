<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dra. Maria Lucila Toloza | Especialista en Derecho Laboral</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Inter', sans-serif; }
        .serif { font-family: 'Playfair Display', serif; }
        .step-inactive { display: none; }
        .btn-option:hover { border-color: #c5a059; background-color: #fcfaf2; }
        .btn-selected { border-color: #c5a059; background-color: #fcfaf2; box-shadow: 0 0 0 2px #c5a059; }
        .hero-overlay { background: linear-gradient(to right, rgba(15, 23, 42, 0.96), rgba(15, 23, 42, 0.75)); }
        .gold-accent { color: #c5a059; }
        .bg-gold { background-color: #c5a059; }
    </style>
</head>
<body class="bg-[#fcfcf9] text-slate-900 overflow-x-hidden">

    <nav class="bg-white/95 backdrop-blur-md border-b sticky top-0 z-[100] px-6 py-4">
        <div class="max-w-7xl mx-auto flex justify-between items-center">
            <div class="flex items-center gap-4">
                <div class="w-12 h-12 bg-slate-900 rounded-lg flex items-center justify-center text-white text-2xl shadow-lg">
                    <i class="fas fa-balance-scale"></i>
                </div>
                <div>
                    <span class="block font-bold text-slate-800 leading-none text-xl tracking-tight uppercase">Maria Lucila Toloza</span>
                    <span class="text-[10px] uppercase tracking-[0.3em] text-slate-500 font-bold mt-1 block">Abogada Especialista Laboral</span>
                </div>
            </div>
            <div class="hidden md:flex items-center gap-8 text-sm font-semibold text-slate-600 uppercase tracking-widest">
                <button onclick="scrollToConsult()" class="bg-slate-900 text-white px-6 py-3 rounded-full hover:bg-slate-800 transition shadow-xl">
                    Iniciar Consulta
                </button>
            </div>
        </div>
    </nav>

    <section class="relative min-h-[75vh] flex items-center bg-slate-900 text-white overflow-hidden">
        <div class="absolute inset-0 z-0">
            <img src="https://images.unsplash.com/photo-1505664194779-8beaceb93744?auto=format&fit=crop&q=80&w=2000" alt="Estudio Jurídico" class="w-full h-full object-cover opacity-40">
            <div class="absolute inset-0 hero-overlay"></div>
        </div>
        <div class="max-w-7xl mx-auto px-6 relative z-10">
            <div class="max-w-3xl">
                <span class="inline-block px-4 py-1 rounded-full bg-blue-500/20 border border-blue-400/30 text-blue-300 text-xs font-bold uppercase tracking-[0.2em] mb-6">Defensa del Trabajador</span>
                <h1 class="serif text-4xl md:text-6xl mb-8 leading-tight">Soluciones legales para <br><span class="gold-accent italic text-3xl md:text-5xl">conflictos laborales</span></h1>
                <p class="text-slate-300 text-lg mb-10 leading-relaxed max-w-xl">
                    Especialista en despidos, accidentes de trabajo y reclamos contra ART. Brindamos asesoramiento integral en Córdoba con un enfoque humano y profesional.
                </p>
                <div class="flex flex-wrap gap-5">
                    <button onclick="scrollToConsult()" class="bg-blue-600 hover:bg-blue-500 px-10 py-5 rounded-2xl font-bold transition shadow-2xl shadow-blue-900/40 flex items-center gap-3">
                        <i class="fab fa-whatsapp text-xl"></i> Consultar ahora
                    </button>
                </div>
            </div>
        </div>
    </section>

    <section id="consultar" class="bg-slate-100 py-24 px-6 border-y border-slate-200">
        <div class="max-w-3xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="serif text-3xl md:text-4xl mb-4 text-slate-800">Inicie su consulta</h2>
                <p class="text-slate-500">Complete los siguientes pasos para enviarme su caso directamente por WhatsApp.</p>
            </div>

            <div id="progress-bar" class="flex justify-between items-center mb-12 px-4">
                <div class="flex flex-col items-center">
                    <div id="p-1" class="w-10 h-10 rounded-full border-2 flex items-center justify-center bg-slate-900 text-white border-slate-900 font-bold">1</div>
                </div>
                <div class="h-[2px] bg-slate-300 flex-1 mx-4"></div>
                <div class="flex flex-col items-center">
                    <div id="p-2" class="w-10 h-10 rounded-full border-2 flex items-center justify-center bg-white border-slate-300 text-slate-400 font-bold">2</div>
                </div>
                <div class="h-[2px] bg-slate-300 flex-1 mx-4"></div>
                <div class="flex flex-col items-center">
                    <div id="p-3" class="w-10 h-10 rounded-full border-2 flex items-center justify-center bg-white border-slate-300 text-slate-400 font-bold">3</div>
                </div>
            </div>

            <div class="bg-white rounded-[2.5rem] shadow-2xl p-8 md:p-16 border border-white">
                <div id="step-1">
                    <h3 class="text-2xl font-bold mb-8 text-slate-800">¿Cuál es su nombre?</h3>
                    <div class="mb-8">
                        <label class="block text-xs font-bold uppercase text-slate-400 mb-3 tracking-widest">Nombre y Apellido</label>
                        <input type="text" id="nombre" class="w-full bg-slate-50 border-0 rounded-2xl p-5 outline-none focus:ring-2 focus:ring-blue-100 transition" placeholder="Ej: Juan Pérez">
                    </div>
                    <button onclick="nextStep(2)" class="w-full bg-slate-900 text-white py-6 rounded-2xl font-bold text-lg hover:shadow-xl transition-all">Siguiente paso</button>
                </div>

                <div id="step-2" class="step-inactive">
                    <h3 class="text-2xl font-bold mb-8 text-slate-800">Motivo de la consulta</h3>
                    <div class="grid grid-cols-1 gap-4 mb-10">
                        <div onclick="selectCase('Despido', this)" class="btn-option cursor-pointer p-6 border-2 rounded-3xl flex items-center gap-4 transition">
                            <i class="fas fa-user-slash text-red-600 text-xl"></i>
                            <span class="font-bold text-slate-700">Despido / Liquidación</span>
                        </div>
                        <div onclick="selectCase('Accidente', this)" class="btn-option cursor-pointer p-6 border-2 rounded-3xl flex items-center gap-4 transition">
                            <i class="fas fa-ambulance text-blue-600 text-xl"></i>
                            <span class="font-bold text-slate-700">Accidente Laboral / ART</span>
                        </div>
                        <div onclick="selectCase('Otro', this)" class="btn-option cursor-pointer p-6 border-2 rounded-3xl flex items-center gap-4 transition">
                            <i class="fas fa-folder-open text-slate-400 text-xl"></i>
                            <span class="font-bold text-slate-700">Otras consultas laborales</span>
                        </div>
                    </div>
                    <div class="flex gap-4">
                        <button onclick="prevStep(1)" class="flex-1 bg-slate-100 py-5 rounded-2xl font-bold text-slate-500">Atrás</button>
                        <button onclick="nextStep(3)" class="flex-[2] bg-slate-900 text-white py-5 rounded-2xl font-bold text-lg">Continuar</button>
                    </div>
                </div>

                <div id="step-3" class="step-inactive">
                    <h3 class="text-2xl font-bold mb-8 text-slate-800">Describa brevemente su situación</h3>
                    <textarea id="detalle" rows="6" class="w-full bg-slate-50 border-0 rounded-2xl p-6 mb-10 outline-none resize-none" placeholder="Cuénteme qué sucedió para brindarle un mejor asesoramiento..."></textarea>
                    <div class="flex gap-4">
                        <button onclick="prevStep(2)" class="flex-1 bg-slate-100 py-5 rounded-2xl font-bold text-slate-500">Atrás</button>
                        <button onclick="submitForm()" id="btn-submit" class="flex-[2] bg-green-600 text-white py-5 rounded-2xl font-bold text-lg hover:bg-green-700 transition flex items-center justify-center gap-3">
                            <i class="fab fa-whatsapp"></i> Enviar a la Dra. Toloza
                        </button>
                    </div>
                </div>

                <div id="step-success" class="step-inactive text-center py-12">
                    <div class="w-24 h-24 bg-green-100 text-green-600 rounded-full flex items-center justify-center mx-auto mb-8 text-4xl">
                        <i class="fas fa-check-circle"></i>
                    </div>
                    <h3 class="serif text-3xl font-bold mb-4">Consulta Lista</h3>
                    <p class="text-slate-500 mb-10">Si WhatsApp no se abrió automáticamente, presione el botón de abajo.</p>
                    <a id="retry-link" href="#" target="_blank" class="inline-block bg-slate-900 text-white px-8 py-4 rounded-full font-bold">Abrir chat ahora</a>
                </div>
            </div>
        </div>
    </section>

    <footer class="bg-white border-t py-16 px-6">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-10">
            <div>
                <div class="flex items-center gap-3 mb-4">
                    <i class="fas fa-balance-scale text-2xl text-slate-900"></i>
                    <span class="font-bold text-xl tracking-tight uppercase">Dra. Maria Lucila Toloza</span>
                </div>
                <p class="text-sm text-slate-400">Especialista en Derecho Laboral y Seguridad Social. Córdoba, Argentina.</p>
            </div>
            <div class="flex flex-col items-center md:items-end gap-4">
                <a href="https://wa.me/5493515116858" target="_blank" class="bg-green-50 text-green-700 px-8 py-4 rounded-2xl font-bold border border-green-100 flex items-center gap-3 hover:bg-green-600 hover:text-white transition group">
                    <i class="fab fa-whatsapp text-2xl"></i>
                    351 5116858
                </a>
                <p class="text-[10px] text-slate-300 uppercase">© 2024 Maria Lucila Toloza | Todos los derechos reservados</p>
            </div>
        </div>
    </footer>

    <script>
        let currentStep = 1;
        let selectedCaseType = '';

        function scrollToConsult() {
            document.getElementById('consultar').scrollIntoView({ behavior: 'smooth' });
        }

        function nextStep(step) {
            const currentEl = document.getElementById(`step-${currentStep}`);
            if (currentEl) currentEl.classList.add('step-inactive');

            const nextEl = document.getElementById(`step-${step}`);
            if (nextEl) nextEl.classList.remove('step-inactive');

            const progressCircle = document.getElementById(`p-${step}`);
            if (progressCircle) {
                progressCircle.classList.add('bg-slate-900', 'text-white', 'border-slate-900');
                progressCircle.classList.remove('text-slate-400', 'border-slate-300');
            }
            currentStep = step;
        }

        function prevStep(step) {
            document.getElementById(`step-${currentStep}`).classList.add('step-inactive');
            document.getElementById(`step-${step}`).classList.remove('step-inactive');
            currentStep = step;
        }

        function selectCase(type, el) {
            selectedCaseType = type;
            document.querySelectorAll('.btn-option').forEach(b => b.classList.remove('btn-selected'));
            el.classList.add('btn-selected');
        }

        async function submitForm() {
            const btn = document.getElementById('btn-submit');
            btn.disabled = true;
            btn.innerHTML = '<i class="fas fa-circle-notch fa-spin"></i> Enviando...';

            const nombre = document.getElementById('nombre').value || "Cliente";
            const detalle = document.getElementById('detalle').value || "Solicita asesoramiento laboral.";

            const message = `⚖️ *CONSULTA LABORAL*\n` +
                            `--------------------------\n` +
                            `👤 *Nombre:* ${nombre}\n` +
                            `📁 *Tipo:* ${selectedCaseType || "General"}\n\n` +
                            `📝 *Detalle:* ${detalle}\n` +
                            `--------------------------\n` +
                            `_Enviado desde el portal de la Dra. Toloza_`;

            const waUrl = `https://wa.me/5493515116958?text=${encodeURIComponent(message)}`;

            // Intentamos registro interno antes de redirigir
            try {
                await fetch(new URL('/api/generar-contenido', window.location.origin), {
                    method: 'POST',
                    headers: {'Content-Type': 'application/json'},
                    body: JSON.stringify({ nombre, tipo_caso: selectedCaseType, detalle })
                }).catch(() => console.log("Modo standalone activado."));
            } finally {
                window.open(waUrl, '_blank');
                document.getElementById('retry-link').href = waUrl;
                document.getElementById('progress-bar').style.display = 'none';
                nextStep('success');
            }
        }
    </script>
</body>
</html>
