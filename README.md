<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vaquinha - Instituto Patinhas Solidárias | Resgate e Cuidado Animal</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Inter', sans-serif;
        }
        
        .progress-bar {
            transition: width 1s ease-in-out;
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }
        
        .donation-button {
            transition: all 0.2s ease;
        }
        
        .donation-button:hover {
            transform: translateY(-1px);
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }
        
        .hero-image {
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%234ade80" width="1200" height="600"/><circle fill="%23ffffff" opacity="0.1" cx="200" cy="150" r="80"/><circle fill="%23ffffff" opacity="0.1" cx="800" cy="300" r="120"/><circle fill="%23ffffff" opacity="0.1" cx="1000" cy="100" r="60"/></svg>');
            background-size: cover;
            background-position: center;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Header Principal -->
    <header class="hero-image text-white py-20">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto text-center">
                <div class="mb-8">
                    <div class="inline-flex items-center bg-white bg-opacity-20 backdrop-blur-sm rounded-full px-6 py-3 mb-4">
                        <span class="text-2xl mr-3">🐾</span>
                        <span class="font-semibold text-lg">Instituto Patinhas Solidárias</span>
                    </div>
                </div>
                
                <h1 class="text-4xl md:text-5xl font-bold mb-6 leading-tight">
                    Ajude-nos a Resgatar e Cuidar de Animais Abandonados
                </h1>
                
                <p class="text-xl md:text-2xl mb-8 opacity-90 leading-relaxed">
                    Há 8 anos salvando vidas. Mais de 2.500 animais resgatados, tratados e encaminhados para adoção responsável.
                </p>
                
                <div class="flex flex-wrap justify-center gap-6 text-sm opacity-90">
                    <div class="flex items-center">
                        <span class="mr-2">✅</span>
                        <span>ONG Registrada</span>
                    </div>
                    <div class="flex items-center">
                        <span class="mr-2">🏥</span>
                        <span>Parceria com 12 Veterinários</span>
                    </div>
                    <div class="flex items-center">
                        <span class="mr-2">📋</span>
                        <span>Transparência Total</span>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- Barra de Progresso Principal -->
    <section class="py-12 bg-white shadow-sm">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto">
                <div class="grid md:grid-cols-3 gap-8 mb-12">
                    <div class="text-center">
                        <div class="text-4xl font-bold text-green-600 mb-2" id="current-amount">R$ 0</div>
                        <div class="text-gray-600 font-medium">Arrecadado</div>
                    </div>
                    <div class="text-center">
                        <div class="text-4xl font-bold text-gray-800 mb-2">R$ 1.000.000</div>
                        <div class="text-gray-600 font-medium">Meta</div>
                    </div>
                    <div class="text-center">
                        <div class="text-4xl font-bold text-blue-600 mb-2" id="donor-count">0</div>
                        <div class="text-gray-600 font-medium">Doadores</div>
                    </div>
                </div>
                
                <div class="mb-8">
                    <div class="flex justify-between items-center mb-3">
                        <span class="text-sm font-medium text-gray-700">Progresso da Campanha</span>
                        <span class="text-sm font-medium text-gray-700" id="progress-percentage">0%</span>
                    </div>
                    <div class="bg-gray-200 rounded-full h-4 overflow-hidden">
                        <div id="progress-bar" class="progress-bar bg-green-500 h-full rounded-full" style="width: 0%"></div>
                    </div>
                </div>
                
                <div class="bg-gray-50 rounded-lg p-6">
                    <h3 class="font-semibold text-gray-800 mb-4">Metas da Campanha</h3>
                    <div class="space-y-3">
                        <div class="flex items-center">
                            <span class="text-gray-400 mr-3">⏳</span>
                            <span class="text-gray-700">R$ 100.000 - Medicamentos e equipamentos básicos</span>
                        </div>
                        <div class="flex items-center">
                            <span class="text-gray-400 mr-3">⏳</span>
                            <span class="text-gray-700">R$ 500.000 - Construção do novo abrigo</span>
                        </div>
                        <div class="flex items-center">
                            <span class="text-gray-400 mr-3">⏳</span>
                            <span class="text-gray-700">R$ 1.000.000 - Centro veterinário completo</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Valores de Doação -->
    <section class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="max-w-6xl mx-auto">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold text-gray-800 mb-4">Como Você Pode Ajudar</h2>
                    <p class="text-lg text-gray-600 max-w-2xl mx-auto">
                        Cada contribuição faz a diferença na vida de um animal. Escolha o valor que cabe no seu orçamento.
                    </p>
                </div>
                
                <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6 mb-12">
                    <!-- Doações -->
                    <div class="bg-white p-6 rounded-lg shadow-sm card-hover border border-gray-200">
                        <div class="text-center">
                            <div class="text-3xl mb-4">🥛</div>
                            <h3 class="text-xl font-semibold text-gray-800 mb-2">R$ 25</h3>
                            <p class="text-gray-600 mb-6 text-sm">Alimentação para 1 animal por 1 semana</p>
                            <button onclick="donate(25)" class="w-full bg-blue-500 text-white py-3 rounded-lg hover:bg-blue-600 transition-colors font-medium donation-button">
                                Doar R$ 25
                            </button>
                        </div>
                    </div>
                    
                    <div class="bg-white p-6 rounded-lg shadow-sm card-hover border-2 border-green-400 relative">
                        <div class="absolute -top-3 left-1/2 transform -translate-x-1/2">
                            <span class="bg-green-500 text-white text-xs px-3 py-1 rounded-full font-medium">POPULAR</span>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl mb-4">💊</div>
                            <h3 class="text-xl font-semibold text-gray-800 mb-2">R$ 75</h3>
                            <p class="text-gray-600 mb-6 text-sm">Medicamentos básicos e vermífugos</p>
                            <button onclick="donate(75)" class="w-full bg-green-500 text-white py-3 rounded-lg hover:bg-green-600 transition-colors font-medium donation-button">
                                Doar R$ 75
                            </button>
                        </div>
                    </div>
                    
                    <div class="bg-white p-6 rounded-lg shadow-sm card-hover border border-gray-200">
                        <div class="text-center">
                            <div class="text-3xl mb-4">🏥</div>
                            <h3 class="text-xl font-semibold text-gray-800 mb-2">R$ 150</h3>
                            <p class="text-gray-600 mb-6 text-sm">Consulta veterinária completa</p>
                            <button onclick="donate(150)" class="w-full bg-purple-500 text-white py-3 rounded-lg hover:bg-purple-600 transition-colors font-medium donation-button">
                                Doar R$ 150
                            </button>
                        </div>
                    </div>
                    
                    <div class="bg-white p-6 rounded-lg shadow-sm card-hover border border-gray-200">
                        <div class="text-center">
                            <div class="text-3xl mb-4">⚕️</div>
                            <h3 class="text-xl font-semibold text-gray-800 mb-2">R$ 400</h3>
                            <p class="text-gray-600 mb-6 text-sm">Castração + pós-operatório</p>
                            <button onclick="donate(400)" class="w-full bg-orange-500 text-white py-3 rounded-lg hover:bg-orange-600 transition-colors font-medium donation-button">
                                Doar R$ 400
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Script de Pagamento -->
    <script>
    function donate(amount) {
        // Substitua os links abaixo pelos links reais do seu PIX ou gateway
        const paymentLinks = {
            25: "https://pay.finaliza.shop/pl/772e490731",
            75: "https://pay.finaliza.shop/pl/d5ae2d095f",
            150: "https://pay.finaliza.shop/pl/8a85c1b208",
            400: "https://pay.finaliza.shop/pl/166db5188a"
        };

        if(paymentLinks[amount]){
            window.open(paymentLinks[amount], "_blank");
        } else {
            alert("Link de pagamento não encontrado!");
        }
    }
    </script>
</body>
</html>
