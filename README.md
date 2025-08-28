# Teste2<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rede de Computadores - Portal Informativo</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }
        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
        }
        .network-pattern {
            background-image: radial-gradient(circle, rgba(255,255,255,0.1) 2px, transparent 2px);
            background-size: 30px 30px;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="bg-white bg-opacity-90 backdrop-blur-md fixed w-full z-50 shadow-lg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <span class="text-2xl font-bold text-indigo-600">NETWORK</span>
                    <span class="text-gray-700 ml-1">Academy</span>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-4">
                        <a href="#sobre" class="text-gray-700 hover:text-indigo-600 px-3 py-2 rounded-md text-sm font-medium transition duration-300">Sobre</a>
                        <a href="#tipos" class="text-gray-700 hover:text-indigo-600 px-3 py-2 rounded-md text-sm font-medium transition duration-300">Tipos</a>
                        <a href="#componentes" class="text-gray-700 hover:text-indigo-600 px-3 py-2 rounded-md text-sm font-medium transition duration-300">Componentes</a>
                        <a href="#protocolos" class="text-gray-700 hover:text-indigo-600 px-3 py-2 rounded-md text-sm font-medium transition duration-300">Protocolos</a>
                    </div>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative min-h-screen flex items-center justify-center network-pattern pt-16">
        <div class="absolute inset-0 bg-black opacity-40"></div>
        <div class="relative z-10 max-w-6xl mx-auto px-4 text-center">
            <h1 class="text-5xl md:text-7xl font-bold text-white mb-6 leading-tight">
                Domine o Mundo das
                <span class="text-indigo-300">Redes de Computadores</span>
            </h1>
            <p class="text-xl md:text-2xl text-gray-200 mb-8 max-w-3xl mx-auto">
                Descubra os fundamentos, tecnologias e protocolos que conectam o mundo digital
            </p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <button onclick="scrollToSection('sobre')" class="bg-indigo-600 hover:bg-indigo-700 text-white px-8 py-4 rounded-lg font-semibold text-lg transition duration-300 transform hover:scale-105">
                    Começar a Explorar
                </button>
                <button onclick="scrollToSection('protocolos')" class="border-2 border-white text-white hover:bg-white hover:text-indigo-600 px-8 py-4 rounded-lg font-semibold text-lg transition duration-300">
                    Ver Protocolos
                </button>
            </div>
        </div>
    </section>

    <!-- Sobre Redes -->
    <section id="sobre" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">O que é uma Rede de Computadores?</h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">
                    Uma rede de computadores é um sistema que permite a comunicação e compartilhamento de recursos entre dispositivos interconectados.
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/399ff373-e1ad-4484-9505-4e28b71b3699.png" alt="Diagrama de rede mostrando múltiplos dispositivos conectados através de um roteador central com linhas representando conexões de dados" class="rounded-xl shadow-2xl w-full" />
                </div>
                <div>
                    <h3 class="text-2xl font-semibold text-gray-800 mb-4">Fundamentos das Redes</h3>
                    <p class="text-gray-600 mb-6 leading-relaxed">
                        As redes de computadores revolucionaram a forma como nos comunicamos e compartilhamos informações. Elas permitem que dispositivos como computadores, servidores, smartphones e outros equipamentos troquem dados de forma eficiente através de protocolos padronizados.
                    </p>
                    <div class="grid grid-cols-2 gap-4">
                        <div class="bg-gray-50 p-4 rounded-lg">
                            <h4 class="font-semibold text-indigo-600 mb-2">Comunicação</h4>
                            <p class="text-sm text-gray-600">Troca eficiente de informações entre dispositivos</p>
                        </div>
                        <div class="bg-gray-50 p-4 rounded-lg">
                            <h4 class="font-semibold text-indigo-600 mb-2">Compartilhamento</h4>
                            <p class="text-sm text-gray-600">Recursos compartilhados como impressoras e arquivos</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Tipos de Redes -->
    <section id="tipos" class="py-20 bg-gray-50">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Tipos de Redes</h2>
                <p class="text-xl text-gray-600">Diferentes escalas e propósitos para diferentes necessidades</p>
            </div>

            <div class="grid md:grid-cols-3 gap-8">
                <!-- LAN -->
                <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                    <div class="w-16 h-16 bg-indigo-100 rounded-lg flex items-center justify-center mb-4">
                        <svg class="w-8 h-8 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-16m16 0h2M7 21h10M7 21v-4a2 2 0 012-2h4a2 2 0 012 2v4"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">LAN (Local Area Network)</h3>
                    <p class="text-gray-600 mb-4">
                        Redes locais que conectam dispositivos em uma área geográfica limitada, como escritórios, casas ou edifícios.
                    </p>
                    <div class="aspect-w-16 aspect-h-9 mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/0b6f1096-e24e-49de-b829-6de1160c3710.png" alt="Diagrama de rede local LAN mostrando computadores conectados a um switch em um ambiente de escritório moderno" class="rounded-lg" />
                    </div>
                </div>

                <!-- WAN -->
                <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                    <div class="w-16 h-16 bg-indigo-100 rounded-lg flex items-center justify-center mb-4">
                        <svg class="w-8 h-8 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 15a4 4 0 004 4h9a5 5 0 10-.1-9.999 5.002 5.002 0 10-9.78 2.096A4.001 4.001 0 003 15z"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">WAN (Wide Area Network)</h3>
                    <p class="text-gray-600 mb-4">
                        Redes que abrangem grandes áreas geográficas, conectando cidades, países ou continentes. A internet é a maior WAN.
                    </p>
                    <div class="aspect-w-16 aspect-h-9 mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/a8ede490-f015-47ec-b4bc-c4a08df73a70.png" alt="Mapa mundial mostrando conexões de rede WAN entre continentes com linhas representando cabos submarinos e conexões internacionais" class="rounded-lg" />
                    </div>
                </div>

                <!-- MAN -->
                <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                    <div class="w-16 h-16 bg-indigo-100 rounded-lg flex items-center justify-center mb-4">
                        <svg class="w-8 h-8 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-16m16 0h2M7 21h10M7 21v-4a2 2 0 012-2h4a2 2 0 012 2v4"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">MAN (Metropolitan Area Network)</h3>
                    <p class="text-gray-600 mb-4">
                        Redes que cobrem uma área metropolitana, como uma cidade ou campus universitário, maior que LAN mas menor que WAN.
                    </p>
                    <div class="aspect-w-16 aspect-h-9 mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/290b583a-36e6-4426-89c2-36aa4c120190.png" alt="Vista aérea de uma cidade mostrando conexões de rede MAN entre edifícios e infraestrutura urbana" class="rounded-lg" />
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Componentes Principais -->
    <section id="componentes" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Componentes Essenciais</h2>
                <p class="text-xl text-gray-600">Os elementos que tornam a comunicação em rede possível</p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="text-center">
                    <div class="bg-indigo-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <svg class="w-10 h-10 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7h12m0 0l-4-4m4 4l-4 4m0 6H4m0 0l4 4m-4-4l4-4"></path>
                        </svg>
                    </div>
                    <h3 class="font-semibold text-gray-800 mb-2">Roteadores</h3>
                    <p class="text-gray-600 text-sm">Encaminham pacotes entre redes diferentes</p>
                </div>

                <div class="text-center">
                    <div class="bg-indigo-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <svg class="w-10 h-10 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11a7 7 0 01-7 7m0 0a7 7 0 01-7-7m7 7v4m0 0H8m4 0h4m-4-8a3 3 0 01-3-3V5a3 3 0 116 0v6a3 3 0 01-3 3z"></path>
                        </svg>
                    </div>
                    <h3 class="font-semibold text-gray-800 mb-2">Switches</h3>
                    <p class="text-gray-600 text-sm">Conectam dispositivos na mesma rede local</p>
                </div>

                <div class="text-center">
                    <div class="bg-indigo-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <svg class="w-10 h-10 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"></path>
                        </svg>
                    </div>
                    <h3 class="font-semibold text-gray-800 mb-2">Firewalls</h3>
                    <p class="text-gray-600 text-sm">Protegem a rede contra acessos não autorizados</p>
                </div>

                <div class="text-center">
                    <div class="bg-indigo-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <svg class="w-10 h-10 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-16m16 0h2M7 21h10M7 21v-4a2 2 0 012-2h4a2 2 0 012 2v4"></path>
                        </svg>
                    </div>
                    <h3 class="font-semibold text-gray-800 mb-2">Servidores</h3>
                    <p class="text-gray-600 text-sm">Fornecem serviços e recursos para a rede</p>
                </div>
            </div>

            <div class="mt-16 text-center">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/a336b38f-4448-4ab6-9a6d-8503e8fc4cf0.png" alt="Diagrama detalhado de infraestrutura de rede mostrando roteadores, switches, servidores e firewalls interconectados em um data center moderno" class="rounded-xl shadow-lg mx-auto w-full max-w-4xl" />
            </div>
        </div>
    </section>

    <!-- Protocolos -->
    <section id="protocolos" class="py-20 bg-gray-900 text-white">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-white mb-4">Protocolos de Rede</h2>
                <p class="text-xl text-gray-300">As regras que governam a comunicação digital</p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-gray-800 rounded-xl p-6 card-hover">
                    <h3 class="text-xl font-semibold text-indigo-300 mb-3">TCP/IP</h3>
                    <p class="text-gray-300 mb-4">
                        O protocolo fundamental da internet, responsável pelo endereçamento e roteamento de pacotes.
                    </p>
                    <div class="bg-gray-700 rounded-lg p-3">
                        <span class="text-sm text-indigo-200">Camadas: Aplicação, Transporte, Internet, Rede</span>
                    </div>
                </div>

                <div class="bg-gray-800 rounded-xl p-6 card-hover">
                    <h3 class="text-xl font-semibold text-indigo-300 mb-3">HTTP/HTTPS</h3>
                    <p class="text-gray-300 mb-4">
                        Protocolos para transferência de hipertexto, base da World Wide Web. HTTPS adiciona segurança.
                    </p>
                    <div class="bg-gray-700 rounded-lg p-3">
                        <span class="text-sm text-indigo-200">Portas: 80 (HTTP), 443 (HTTPS)</span>
                    </div>
                </div>

                <div class="bg-gray-800 rounded-xl p-6 card-hover">
                    <h3 class="text-xl font-semibold text-indigo-300 mb-3">DNS</h3>
                    <p class="text-gray-300 mb-4">
                        Sistema de Nomes de Domínio, traduz nomes de domínio para endereços IP.
                    </p>
                    <div class="bg-gray-700 rounded-lg p-3">
                        <span class="text-sm text-indigo-200">Porta: 53</span>
                    </div>
                </div>

                <div class="bg-gray-800 rounded-xl p-6 card-hover">
                    <h3 class="text-xl font-semibold text-indigo-300 mb-3">FTP/SFTP</h3>
                    <p class="text-gray-300 mb-4">
                        Protocolo de Transferência de Arquivos, com versão segura (SFTP) para transmissões criptografadas.
                    </p>
                    <div class="bg-gray-700 rounded-lg p-3">
                        <span class="text-sm text-indigo-200">Porta: 21 (FTP), 22 (SFTP)</span>
                    </div>
                </div>

                <div class="bg-gray-800 rounded-xl p-6 card-hover">
                    <h3 class="text-xl font-semibold text-indigo-300 mb-3">SMTP</h3>
                    <p class="text-gray-300 mb-4">
                        Protocolo Simples de Transferência de Correio, usado para envio de emails.
                    </p>
                    <div class="bg-gray-700 rounded-lg p-3">
                        <span class="text-sm text-indigo-200">Porta: 25, 587</span>
                    </div>
                </div>

                <div class="bg-gray-800 rounded-xl p-6 card-hover">
                    <h3 class="text-xl font-semibold text-indigo-300 mb-3">SSH</h3>
                    <p class="text-gray-300 mb-4">
                        Secure Shell, protocolo para acesso remoto seguro a sistemas.
                    </p>
                    <div class="bg-gray-700 rounded-lg p-3">
                        <span class="text-sm text-indigo-200">Porta: 22</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="max-w-6xl mx-auto px-4">
            <div class="grid md:grid-cols-3 gap-8">
                <div>
                    <h3 class="text-xl font-semibold mb-4">Network Academy</h3>
                    <p class="text-gray-300">
                        Seu portal definitivo para aprender sobre redes de computadores e tecnologias de comunicação.
                    </p>
                </div>
                <div>
                    <h3 class="text-xl font-semibold mb-4">Navegação</h3>
                    <ul class="space-y-2">
                        <li><a href="#sobre" class="text-gray-300 hover:text-indigo-300 transition duration-300">Sobre Redes</a></li>
                        <li><a href="#tipos" class="text-gray-300 hover:text-indigo-300 transition duration-300">Tipos de Rede</a></li>
                        <li><a href="#componentes" class="text-gray-300 hover:text-indigo-300 transition duration-300">Componentes</a></li>
                        <li><a href="#protocolos" class="text-gray-300 hover:text-indigo-300 transition duration-300">Protocolos</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="text-xl font-semibold mb-4">Contato</h3>
                    <p class="text-gray-300 mb-4">Entre em contato para mais informações</p>
                    <button class="bg-indigo-600 hover:bg-indigo-700 text-white px-6 py-2 rounded-lg transition duration-300">
                        Enviar Mensagem
                    </button>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 text-center">
                <p class="text-gray-400">© 2024 Network Academy. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <script>
        function scrollToSection(sectionId) {
            document.getElementById(sectionId).scrollIntoView({
                behavior: 'smooth'
            });
        }

        // Adiciona classe ativa na navegação ao scroll
        window.addEventListener('scroll', function() {
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('nav a');
            
            let current = '';
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                
                if (pageYOffset >= (sectionTop - 200)) {
                    current = section.getAttribute('id');
                }
            });
            
            navLinks.forEach(link => {
                link.classList.remove('text-indigo-600');
                link.classList.add('text-gray-700');
                if (link.getAttribute('href').substring(1) === current) {
                    link.classList.add('text-indigo-600');
                    link.classList.remove('text-gray-700');
                }
            });
        });
    </script>
</body>
</html>

