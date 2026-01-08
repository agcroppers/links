:root {
    /* Paleta de Cores baseada na marca */
    --primary-green: #2E7D32; /* Verde Agro Sólido */
    --hover-green: #1B5E20;
    --text-white: #ffffff;
    --text-gray: #e0e0e0;
    
    /* Variáveis de Layout */
    --max-width: 480px; /* Largura padrão "Linktree" */
    --border-radius: 12px;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Inter', sans-serif;
    color: var(--text-white);
    min-height: 100vh;
    display: flex;
    justify-content: center;
    overflow-x: hidden;
    background-color: #0f1c10; /* Fallback color */
}

/* Fundo com Imagem e Blur */
.background-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    /* Imagem genérica de Agro de alta qualidade do Unsplash */
    background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.7)), 
                url('https://images.unsplash.com/photo-1625246333195-78d9c38ad449?q=80&w=1770&auto=format&fit=crop');
    background-size: cover;
    background-position: center;
    filter: blur(5px);
    transform: scale(1.05); /* Evita bordas brancas pelo blur */
}

.container {
    width: 100%;
    max-width: var(--max-width);
    padding: 40px 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100vh;
}

/* --- Cabeçalho --- */
header.profile {
    text-align: center;
    margin-bottom: 40px;
}

.logo {
    max-width: 180px;
    height: auto;
    margin-bottom: 15px;
}

header h1 {
    font-size: 1.8rem;
    font-weight: 600;
    margin-bottom: 8px;
    letter-spacing: -0.5px;
}

header p {
    font-size: 0.95rem;
    color: var(--text-gray);
    font-weight: 300;
    line-height: 1.4;
}

/* --- Links / Botões --- */
.links-list {
    width: 100%;
    display: flex;
    flex-direction: column;
    gap: 16px;
    flex-grow: 1; /* Empurra o footer para baixo */
}

.link-card {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 16px 24px;
    text-decoration: none;
    color: var(--text-white);
    border-radius: var(--border-radius);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    
    /* Efeito Glassmorphism Padrão */
    background: rgba(255, 255, 255, 0.05);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.2);
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.card-title {
    font-weight: 500;
    font-size: 1rem;
}

/* Estilo do Botão Principal (Featured) */
.link-card.featured {
    background-color: var(--primary-green);
    border-color: var(--primary-green);
    font-weight: 600;
}

/* Interações / Hover */
.link-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
}

.link-card:active {
    transform: scale(0.98);
}

.link-card:not(.featured):hover {
    background: rgba(255, 255, 255, 0.15);
    border-color: rgba(255, 255, 255, 0.4);
}

.link-card.featured:hover {
    background-color: var(--hover-green);
}

/* Ícone de seta (apenas no destaque se quiser, ou em todos) */
.icon-arrow svg {
    transition: transform 0.3s ease;
}
.link-card:hover .icon-arrow svg {
    transform: translateX(4px);
}

/* --- Rodapé --- */
.footer {
    width: 100%;
    margin-top: 40px;
    display: flex;
    flex-direction: column;
    align-items: center; /* Centralizado no mobile por padrão */
    gap: 15px;
    font-size: 0.85rem;
    color: rgba(255, 255, 255, 0.6);
}

.social-links a {
    display: flex;
    align-items: center;
    gap: 8px;
    color: var(--text-white);
    text-decoration: none;
    transition: opacity 0.3s;
    font-weight: 500;
}

.social-links a:hover {
    opacity: 0.8;
}

/* --- Desktop Layout (Adaptação) --- */
@media (min-width: 768px) {
    /* No Desktop, podemos fixar o social no canto inferior esquerdo conforme referência */
    .footer {
        flex-direction: row;
        justify-content: space-between;
        position: fixed;
        bottom: 20px;
        left: 20px;
        right: 20px;
        width: auto;
        /* O conteúdo do copyright vai para a direita, social para a esquerda */
    }
    
    .copyright {
        margin-left: auto; /* Empurra para direita */
    }

    .container {
        justify-content: center; /* Centraliza verticalmente no desktop */
    }
}

/* --- Animações de Entrada --- */
.animate-up {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 0.8s ease forwards;
}

.delay-1 { animation-delay: 0.1s; }
.delay-2 { animation-delay: 0.2s; }
.delay-3 { animation-delay: 0.3s; }
.delay-4 { animation-delay: 0.4s; }

@keyframes fadeInUp {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}