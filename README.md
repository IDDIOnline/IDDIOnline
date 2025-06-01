<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>La Iglesia de Dios Israelita</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Base Styles */
        :root {
            --color-primary: #2b6cb0; /* Stronger primary blue */
            --color-primary-dark: #2c5282; /* Darker primary for hover */
            --color-secondary-light: #ebf8ff; /* Light secondary blue */
            --color-secondary-dark: #bfdbfe; /* Darker secondary for hover */
            --color-text-dark: #1f2937; /* Very dark gray for main text */
            --color-text-medium: #374151; /* Medium gray */
            --color-text-light: #4b5563; /* Light gray */
            --color-background-light: #fdfdfe; /* Almost white background */
            --color-border-light: #e2e8f0; /* Light gray border */

            /* Sidebar Colors - Updated to match provided snippet */
            --color-sidebar-bg: #1a365d; /* Darker blue for sidebar */
            --color-sidebar-border: #2a4365; /* Slightly lighter sidebar border */
            --color-sidebar-text: #c3dae8; /* Lighter blue for sidebar text */
            --color-sidebar-icon: #90cdf4; /* Lighter blue for sidebar icons */

            --color-focus-ring: rgba(66, 153, 225, 0.5); /* Blue focus ring */
        }

        *, *::before, *::after {
            box-sizing: border-box; /* Global box-sizing */
        }

        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            background-color: var(--color-background-light);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
            color: var(--color-text-medium);
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
            line-height: 1.6; /* Improved readability */
            font-size: 1rem; /* Base font size */
        }

        /* Utility Classes (mimicking Tailwind where needed) */
        .flex { display: flex; }
        .flex-col { flex-direction: column; }
        .items-center { align-items: center; }
        .justify-between { justify-content: space-between; }
        .justify-center { justify-content: center; }
        .text-center { text-align: center; }
        .p-4 { padding: 1rem; }
        .p-6 { padding: 1.5rem; }
        .pb-4 { padding-bottom: 1rem; }
        .px-4 { padding-left: 1rem; padding-right: 1rem; }
        .py-2 { padding-top: 0.5rem; padding-bottom: 0.5rem; }
        .py-3 { padding-top: 0.75rem; padding-bottom: 0.75rem; }
        .px-6 { padding-left: 1.5rem; padding-right: 1.5rem; }
        .mt-1 { margin-top: 0.25rem; }
        .mt-4 { margin-top: 1rem; }
        .mt-5 { margin-top: 1.25rem; }
        .mt-6 { margin-top: 1.5rem; }
        .mb-4 { margin-bottom: 1rem; }
        .mb-6 { margin-bottom: 1.5rem; }
        .mr-2 { margin-right: 0.5rem; }
        .mr-3 { margin-right: 0.75rem; }
        .ml-auto { margin-left: auto; }
        .space-x-2 > *:not(:first-child) { margin-left: 0.5rem; }
        .space-y-2 > *:not(:first-child) { margin-top: 0.5rem; }
        .space-y-3 > *:not(:first-child) { margin-top: 0.75rem; }
        .space-y-4 > *:not(:first-child) { margin-top: 1rem; }
        .w-full { width: 100%; }
        .h-6 { height: 1.5rem; }
        .h-5 { height: 1.25rem; }
        .h-10 { height: 2.5rem; }
        .h-8 { height: 2rem; }
        .h-12 { height: 3rem; }
        .w-6 { width: 1.5rem; }
        .w-5 { width: 1.25rem; }
        .w-10 { width: 2.5rem; }
        .w-64 { width: 16rem; }
        .max-w-2xl { max-width: 42rem; }
        .mx-auto { margin-left: auto; margin-right: auto; }
        .rounded-md { border-radius: 0.375rem; }
        .rounded-lg { border-radius: 0.5rem; }
        .rounded-xl { border-radius: 0.75rem; } /* New rounded value */
        .rounded-full { border-radius: 9999px; }
        .block { display: block; } /* Added for explicit block display */
        
        /* Softer, more modern shadows */
        .shadow-sm { box-shadow: 0 1px 3px rgba(0, 0, 0, 0.06), 0 1px 2px rgba(0, 0, 0, 0.04); }
        .shadow-md { box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08), 0 2px 6px rgba(0, 0, 0, 0.05); }
        .shadow-lg { box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1), 0 6px 6px rgba(0, 0, 0, 0.06); } /* New stronger shadow for cards */

        .border { border-width: 1px; border-style: solid; }
        .border-b { border-bottom-width: 1px; }
        .border-gray-200 { border-color: var(--color-border-light); }
        .border-gray-300 { border-color: #d1d5db; }
        .border-blue-100 { border-color: #dbeafe; }
        .border-blue-700 { border-color: var(--color-primary); }
        .bg-white { background-color: #fff; }
        .bg-blue-50 { background-color: var(--color-background-light); }
        .bg-blue-100 { background-color: var(--color-secondary-light); }
        .bg-blue-800 { background-color: var(--color-sidebar-bg); }
        .bg-black { background-color: #000; }
        .bg-opacity-50 { background-color: rgba(0, 0, 0, 0.5); }
        .text-white { color: #fff; }
        .text-gray-600 { color: var(--color-text-light); }
        .text-gray-700 { color: var(--color-text-medium); }
        .text-gray-800 { color: var(--color-text-dark); }
        .text-blue-200 { color: var(--color-sidebar-text); }
        .text-blue-300 { color: var(--color-sidebar-icon); } /* Now explicitly using sidebar icon color */
        .text-blue-400 { color: var(--color-sidebar-icon); } /* Now explicitly using sidebar icon color */
        .text-blue-700 { color: var(--color-primary); }
        .text-blue-800 { color: var(--color-text-dark); }
        .text-sm { font-size: 0.875rem; }
        .text-base { font-size: 1rem; }
        .text-lg { font-size: 1.125rem; }
        .text-xl { font-size: 1.25rem; }
        .text-2xl { font-size: 1.5rem; }
        .text-3xl { font-size: 1.875rem; }
        .font-medium { font-weight: 500; }
        .font-semibold { font-weight: 600; }
        .font-bold { font-weight: 700; }
        
        .transition-colors { transition-property: color, background-color, border-color, text-decoration-color, fill, stroke; transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1); transition-duration: 150ms; }
        .transition-transform { transition-property: transform; transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1); transition-duration: 300ms; }
        .duration-200 { transition-duration: 200ms; }
        .duration-300 { transition-duration: 300ms; }
        .ease-in-out { transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1); }

        .hover\:bg-blue-800:hover { background-color: var(--color-primary-dark); }
        .hover\:bg-blue-700:hover { background-color: var(--color-sidebar-border); } /* Darker for sidebar links */
        .hover\:bg-blue-200:hover { background-color: var(--color-secondary-dark); }
        .hover\:bg-blue-50:hover { background-color: #e0f2f7; }
        .hover\:text-white:hover { color: #fff; }
        .hover\:underline:hover { text-decoration: underline; }
        
        .focus\:outline-none:focus { outline: 2px solid transparent; outline-offset: 2px; }
        .focus\:ring-2:focus { box-shadow: 0 0 0 2px; }
        .focus\:ring-offset-2:focus { box-shadow: 0 0 0 2px #fff, 0 0 0 4px; }
        .focus\:ring-blue-500:focus { box-shadow: 0 0 0 2px #fff, 0 0 0 4px var(--color-focus-ring); }
        .focus\:ring-blue-300:focus { box-shadow: 0 0 0 2px #fff, 0 0 0 4px #93c5fd; }
        .focus\:ring-blue-200:focus { box-shadow: 0 0 0 2px #fff, 0 0 0 4px #bfdbfe; }
        .focus\:border-blue-500:focus { border-color: var(--color-primary); }
        .sticky { position: sticky; }
        .top-0 { top: 0; }
        .z-20 { z-index: 20; }
        .z-30 { z-index: 30; }
        .z-40 { z-index: 40; }
        .fixed { position: fixed; }
        .inset-0 { top: 0; right: 0; bottom: 0; left: 0; }
        .right-0 { right: 0; }
        .overflow-y-auto { overflow-y: auto; }
        .flex-1 { flex: 1 1 0%; }
        .transform { transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y)); }
        .translate-x-full { transform: translateX(100%); }
        .translate-x-0 { transform: translateX(0); }
        .hidden { display: none; }
        .block { display: block; }
        .underline { text-decoration: underline; }
        .line-through { text-decoration: line-through; }
        .cursor-pointer { cursor: pointer; }

        /* Page Transition CSS */
        .page-content {
            opacity: 0;
            transform: translateY(10px);
            transition: opacity 0.4s ease-out, transform 0.4s ease-out;
            will-change: opacity, transform; /* Optimize for animation */
        }
        .page-content.active {
            opacity: 1;
            transform: translateY(0);
        }

        /* Specific Component Styles */
        header {
            border-bottom: 1px solid var(--color-border-light);
            background-color: #fff;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05); /* Softer shadow */
        }

        .header-button {
            background-color: transparent;
            border: none;
            padding: 0;
        }
        .header-button .lucide-icon {
            color: var(--color-primary);
        }

        .sidebar {
            background-color: var(--color-sidebar-bg);
            box-shadow: -4px 0 10px rgba(0, 0, 0, 0.2); /* Shadow for sidebar */
        }
        .sidebar-header {
            border-color: var(--color-sidebar-border);
        }
        .sidebar-title {
            color: var(--color-sidebar-icon); /* Uses sidebar icon color */
        }
        .sidebar-close-button {
            background-color: transparent;
            border: none;
        }
        .sidebar-close-button .lucide-icon {
            color: var(--color-sidebar-icon); /* Uses sidebar icon color */
        }
        .sidebar-close-button:hover {
            background-color: var(--color-sidebar-border);
        }

        .sidebar-nav-link {
            color: var(--color-sidebar-text);
        }
        .sidebar-nav-link:hover {
            background-color: var(--color-sidebar-border);
            color: #fff;
        }
        .sidebar-nav-link .lucide-icon {
            color: var(--color-sidebar-icon); /* Uses sidebar icon color */
        }

        .card {
            background-color: #fff;
            border: 1px solid var(--color-border-light);
            border-radius: 0.75rem; /* More rounded */
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08), 0 4px 8px rgba(0, 0, 0, 0.04); /* Deeper, softer shadow */
        }
        .card img {
            border-radius: 0.625rem; /* Match card radius */
        }

        .primary-button {
            background-color: var(--color-primary);
            color: #fff;
            padding: 0.75rem 1.5rem;
            border-radius: 0.5rem;
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.1); /* Subtle shadow */
            transition: background-color 0.2s ease, transform 0.2s ease, box-shadow 0.2s ease;
        }
        .primary-button:hover {
            background-color: var(--color-primary-dark);
            transform: translateY(-2px); /* Slight lift */
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15); /* Enhanced shadow */
        }
        .primary-button:active {
            transform: translateY(0); /* Press effect */
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
        }
        .primary-button:focus {
            box-shadow: 0 0 0 3px var(--color-focus-ring);
        }

        .secondary-button {
            background-color: var(--color-secondary-light);
            color: var(--color-primary);
            border: 1px solid var(--color-secondary-dark);
            padding: 0.75rem 1.5rem;
            border-radius: 0.5rem;
            transition: background-color 0.2s ease, transform 0.2s ease, box-shadow 0.2s ease;
        }
        .secondary-button:hover {
            background-color: var(--color-secondary-dark);
            transform: translateY(-1px);
            box-shadow: 0 2px 5px rgba(0,0,0,0.08);
        }
        .secondary-button:active {
            transform: translateY(0);
        }
        .secondary-button:focus {
            box-shadow: 0 0 0 3px var(--color-focus-ring);
        }

        .ghost-button {
            color: var(--color-primary);
            transition: background-color 0.2s ease;
        }
        .ghost-button:hover {
            background-color: #f0f8ff;
        }
        .ghost-button:focus {
            box-shadow: 0 0 0 3px var(--color-focus-ring);
        }

        .input-field, .textarea-field {
            border: 1px solid var(--color-border-light);
            border-radius: 0.5rem;
            padding: 0.75rem 1rem;
            box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.03); /* Softer inner shadow */
            transition: border-color 0.2s ease, box-shadow 0.2s ease;
        }
        .input-field:focus, .textarea-field:focus {
            border-color: var(--color-primary);
            box-shadow: 0 0 0 3px var(--color-focus-ring);
            outline: none; /* Remove default outline */
        }

        .sermon-item {
            border: 1px solid var(--color-border-light);
            background-color: #fff;
            border-radius: 0.625rem;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }
        .sermon-item:hover {
            transform: translateY(-3px); /* More pronounced lift */
            box-shadow: 0 6px 16px rgba(0, 0, 0, 0.1); /* Enhanced shadow */
        }

        /* Responsive Design (Mobile-first) */
        @media (min-width: 768px) { /* md breakpoint */
            .md\:hidden { display: none; }
            .md\:ml-64 { margin-left: 16rem; }
            .md\:translate-x-0 { transform: translateX(0); }
        }
    </style>
</head>
<body>
    <div class="flex flex-col min-h-screen bg-blue-50 font-inter">
        <header class="bg-white shadow-sm border-b border-blue-100 p-4 flex items-center justify-between sticky top-0 z-20">
            <h1 class="text-xl font-bold text-blue-800">La Iglesia de Dios Israelita</h1>
            <button id="menu-toggle-button" class="ghost-button h-10 w-10 flex items-center justify-center rounded-md focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-200 cursor-pointer">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-6 w-6 text-blue-700">
                    <line x1="4" x2="20" y1="12" y2="12"></line>
                    <line x1="4" x2="20" y1="6" y2="6"></line>
                    <line x1="4" x2="20" y1="18" y2="18"></line>
                </svg>
            </button>
        </header>

        <main id="main-content" class="flex-1 p-4 overflow-y-auto">
            <div id="home-page" class="page-content">
                <div class="text-center p-6 bg-white rounded-xl shadow-lg card">
                    <img src="https://placehold.co/600x300/e0f2f7/01579b?text=Bienvenido" alt="Welcome Banner" class="w-full rounded-lg mb-6 shadow-sm" />
                    <h2 class="text-3xl font-bold text-blue-800 mb-4">¡Bienvenidos a Nuestra Iglesia!</h2>
                    <p class="text-gray-700 text-lg mb-4">
                        Nos complace que nos visite. Aquí encontrará un lugar de paz, fe y comunidad.
                    </p>
                    <p class="text-gray-600 text-base">
                        Nuestra misión es difundir la palabra de Dios y servir a nuestra comunidad con amor y dedicación.
                    </p>
                    <div class="flex justify-center mt-6">
                        <button class="primary-button flex items-center justify-center cursor-pointer">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-4 w-4 mr-2">
                                <circle cx="12" cy="12" r="10"></circle>
                                <polygon points="10 8 16 12 10 16 10 8"></polygon>
                            </svg>
                            Ver Servicio en Vivo
                        </button>
                    </div>
                </div>
            </div>

            <div id="about-page" class="page-content hidden">
                <div class="p-6 bg-white rounded-xl shadow-lg card">
                    <h2 class="text-2xl font-bold text-blue-800 mb-4">Acerca de Nosotros</h2>
                    <p class="text-gray-700 mb-4">
                        La Iglesia de Dios Israelita tiene una rica historia de fe y servicio. Fundada en principios bíblicos,
                        nuestra congregación se ha dedicado a la enseñanza de la palabra de Dios y al apoyo mutuo entre sus miembros.
                    </p>
                    <p class="text-gray-700 mb-4">
                        Creemos firmemente en el poder de la oración, la importancia de la comunidad y la guía de las escrituras.
                        Nuestros valores fundamentales incluyen el amor, la compasión, la justicia y la humildad.
                    </p>
                    <p class="text-gray-700">
                        Invitamos a todos a unirse a nosotros en el camino de la fe y a experimentar la gracia de Dios.
                    </p>
                    HELLO
<body class="center">
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Photo Slider</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom styles for the Inter font */
        body {
            font-family: 'Inter', sans-serif;
        }
        /* Ensure images take full width within the flex container */
        .slider-images img {
            width: 100%;
            flex-shrink: 0; /* Prevents images from shrinking */
            object-fit: cover; /* Ensures images cover the area without distortion */
        }
    </style>
</head>
<body class="min-h-screen flex items-center justify-center">
    <div
        id="slider-container"
        class="relative w-1/3 max-w-full bg-white rounded-xl shadow-lg overflow-hidden
               hover:shadow-xl transition-shadow duration-300 ease-in-out"
    >
        <div id="slider-images" class="flex transition-transform duration-500 ease-in-out">
            <img src="https://scontent-ord5-3.xx.fbcdn.net/v/t39.30808-6/482068061_681783227846233_6505843607583388327_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=127cfc&_nc_ohc=A0rPSA7zuC8Q7kNvwFAx3vT&_nc_oc=Adm5FFjF9PUL3wWNz2k2yEQ4a4wajDmfMNMkFT0e78S_hcB1Ma81ZceKzv4GLOoa8DA&_nc_zt=23&_nc_ht=scontent-ord5-3.xx&_nc_gid=2n9Xt068BIU0_j9uSy5aQA&oh=00_AfJJVSGmtM5kGisCbXwI6l586kiP04u2eu42ImiudfDw1Q&oe=6841D467" alt="Slide 1"
                 class="w-full flex-shrink-0 object-cover rounded-xl"
                 onerror="this.onerror=null;this.src='https://placehold.co/800x450/CCCCCC/666666?text=Image+Error';" />
            <img src="https://scontent-ord5-3.xx.fbcdn.net/v/t39.30808-6/485145768_1092813809547352_1485650446715542739_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=f727a1&_nc_ohc=fxvxN6-ufH0Q7kNvwFhEgr-&_nc_oc=AdkWMS7a4aJ25XMV6CI8Ub01Wx9a1cdPfpO4Ka-UXhH3jjwqP-4Xl-VOOCpyZiSBj7o&_nc_zt=23&_nc_ht=scontent-ord5-3.xx&_nc_gid=Cdgh411RXto8fYeUE6Iwzg&oh=00_AfJkGawyosOuBoDIQLwmRzUD-p8pfcMPyJ6dAJEe2RldqA&oe=6841F122" alt="Slide 2"
                 class="w-full flex-shrink-0 object-cover rounded-xl"
                 onerror="this.onerror=null;this.src='https://placehold.co/800x450/CCCCCC/666666?text=Image+Error';" />
            <img src="https://scontent-ord5-2.xx.fbcdn.net/v/t39.30808-6/465450171_9311590395546266_4699851194046170707_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=cf85f3&_nc_ohc=Nv9prDhmH8sQ7kNvwFlvZsg&_nc_oc=AdlzokcDSKeUG2wHjnAP6uaVxczxuwy0-yq6Sk2oXjosXh7T0YumEcUToIRA0Q9Zo2c&_nc_zt=23&_nc_ht=scontent-ord5-2.xx&_nc_gid=9qE6JRF422_z-d1nCaDETg&oh=00_AfKu22zTx-kvYXnvVqy4AjVZmXG2AH3uJJbEJm314YlFpw&oe=6841EB4C" alt="Slide 3"
                 class="w-full flex-shrink-0 object-cover rounded-xl"
                 onerror="this.onerror=null;this.src='https://placehold.co/800x450/CCCCCC/666666?text=Image+Error';" />
            <img src="https://scontent-ord5-1.xx.fbcdn.net/v/t39.30808-6/465231298_9311453955559910_3484166220115580374_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=cf85f3&_nc_ohc=2BhE6w2-Ij4Q7kNvwGyq4Ks&_nc_oc=AdmUPgoA7hh97x-uMzybdob5ANLFoiWGqYCL_hdCGlFp_TFRgim6nQbuMu9ixfHqB4I&_nc_zt=23&_nc_ht=scontent-ord5-1.xx&_nc_gid=WUUPBts8E7xnBi-oKAamTQ&oh=00_AfIyOtb7WW-AdhkuvSIPBgWyNEuEYTcjKvUYmkLbcU6c2A&oe=6841EC49" alt="Slide 4"
                 class="w-full flex-shrink-0 object-cover rounded-xl"
                 onerror="this.onerror=null;this.src='https://placehold.co/800x450/CCCCCC/666666?text=Image+Error';" />
            <img src="https://scontent-ord5-3.xx.fbcdn.net/v/t1.6435-9/42465233_1884903408261109_2868740314925891584_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=833d8c&_nc_ohc=r5U1nAUYLFUQ7kNvwEfmMNa&_nc_oc=AdmmBUR7sBjYsRuuc2Et5_gZqnGZXHGqwwk1kFJffi5pt8IvWEG_M6Ad_tV5JNo6V6Q&_nc_zt=23&_nc_ht=scontent-ord5-3.xx&_nc_gid=jowMo4knkqFHYaopkoXG8A&oh=00_AfKRwIX2m_ZiiYGCvzcaJgOlXAnRbvXhmyhKzh4j75hPFQ&oe=68639A5D" alt="Slide 5"
                 class="w-full flex-shrink-0 object-cover rounded-xl"
                 onerror="this.onerror=null;this.src='https://placehold.co/800x450/CCCCCC/666666?text=Image+Error';" />
            <img src="https://scontent-ord5-3.xx.fbcdn.net/v/t39.30808-6/500780163_1148456883983044_5268337824696854206_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=127cfc&_nc_ohc=ZLhs54C_ucIQ7kNvwHB9w7o&_nc_oc=AdmFgxHiW6u5RnFnt_K-jxHE38MLv2mrVLFoKdfaQ0ZgxIUKiIp4Txix0zY1JCOplxQ&_nc_zt=23&_nc_ht=scontent-ord5-3.xx&_nc_gid=_JAbu9Es1Iqwb-gw7BYTZw&oh=00_AfJqAW9KsYZhLQUfrqzeQWYM99VQvQD_uK173HP6raP1zQ&oe=6841CED7" alt="Slide 6"
                 class="w-full flex-shrink-0 object-cover rounded-xl"
                 onerror="this.onerror=null;this.src='https://placehold.co/800x450/CCCCCC/666666?text=Image+Error';" />
            <img src="https://scontent-ord5-3.xx.fbcdn.net/v/t39.30808-6/485833912_1098559985639401_2614873029103859240_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=f727a1&_nc_ohc=Ucy2zCc4ikEQ7kNvwFWxIpr&_nc_oc=AdkjjGJ-Dxg6k2VJP6oNBsCpje9V5l2XYCJh4AdIrGEUtUVnmmy2JbYOAdcQOv8Zmv0&_nc_zt=23&_nc_ht=scontent-ord5-3.xx&_nc_gid=XVGHQ5Xco1nDc7jl5wI2sw&oh=00_AfK-SCcbUWI1nBOdV6RfxcfhVzWCM4sh_T0wnP9nP7NQpQ&oe=6841FB72" alt="Slide 7"
                 class="w-full flex-shrink-0 object-cover rounded-xl"
                 onerror="this.onerror=null;this.src='https://placehold.co/800x450/CCCCCC/666666?text=Image+Error';" />
            <img src="https://scontent-ord5-3.xx.fbcdn.net/v/t39.30808-6/486743692_1098559635639436_3472729707717691457_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=f727a1&_nc_ohc=CrFa0Yd8k-gQ7kNvwEvLicK&_nc_oc=Adkeg0Qc5U6ZITpPXBqcvrM2hp-ZOEX11tY62f2tQu4PPTTQd84ZT0pSJNK-5B-_Ty4&_nc_zt=23&_nc_ht=scontent-ord5-3.xx&_nc_gid=dPGjgIMCM_7zVDMEVqmAvw&oh=00_AfJah8uUIbiVMiEJe8S45ThVF5I530XrsSVG1O_42LH3zw&oe=6841E9B1" alt="Slide 8"
                 class="w-full flex-shrink-0 object-cover rounded-xl"
                 onerror="this.onerror=null;this.src='https://placehold.co/800x450/CCCCCC/666666?text=Image+Error';" />
        </div>

        <button
            id="prev-btn"
            class="absolute top-1/2 left-4 transform -translate-y-1/2
                   bg-black bg-opacity-50 text-white p-3 rounded-full
                   hover:bg-opacity-75 focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-75
                   transition-colors duration-200 ease-in-out shadow-md"
            aria-label="Previous slide"
        >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M15 19l-7-7 7-7" />
            </svg>
        </button>

        <button
            id="next-btn"
            class="absolute top-1/2 right-4 transform -translate-y-1/2
                   bg-black bg-opacity-50 text-white p-3 rounded-full
                   hover:bg-opacity-75 focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-75
                   transition-colors duration-200 ease-in-out shadow-md"
            aria-label="Next slide"
        >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7" />
            </svg>
        </button>

        <div id="dots-container" class="absolute bottom-4 left-1/2 transform -translate-x-1/2 flex space-x-2">
            </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const sliderContainer = document.getElementById('slider-container');
            const sliderImages = document.getElementById('slider-images');
            const images = sliderImages.querySelectorAll('img');
            const prevBtn = document.getElementById('prev-btn');
            const nextBtn = document.getElementById('next-btn');
            const dotsContainer = document.getElementById('dots-container');

            let currentIndex = 0;
            const totalImages = images.length;
            let autoSlideInterval; // Variable to hold the interval ID for auto-sliding

            // Dynamically create navigation dots based on the number of images
            // Clear existing dots first to prevent duplicates on updates
            dotsContainer.innerHTML = '';
            for (let i = 0; i < totalImages; i++) {
                const dot = document.createElement('button'); // Using button for better accessibility
                dot.classList.add('h-3', 'w-3', 'rounded-full', 'transition-colors', 'duration-200', 'ease-in-out',
                                  'focus:outline-none', 'focus:ring-2', 'focus:ring-white', 'focus:ring-opacity-75');
                dot.setAttribute('data-index', i);
                dot.setAttribute('aria-label', `Go to slide ${i + 1}`);
                dotsContainer.appendChild(dot);
            }

            const dots = dotsContainer.querySelectorAll('button'); // Get all created dot buttons

            // Function to update the slider's position and active dot
            function updateSlider() {
                // Adjust the transform property to show the current image
                sliderImages.style.transform = `translateX(-${currentIndex * 100}%)`;

                // Update the active state of navigation dots
                dots.forEach((dot, index) => {
                    if (index === currentIndex) {
                        dot.classList.add('bg-white');
                        dot.classList.remove('bg-gray-400', 'bg-opacity-75');
                    } else {
                        dot.classList.remove('bg-white');
                        dot.classList.add('bg-gray-400', 'bg-opacity-75');
                    }
                });
            }

            // Function to move to the next slide
            function goToNextSlide() {
                currentIndex = (currentIndex + 1) % totalImages;
                updateSlider();
            }

            // Function to move to the previous slide
            function goToPrevSlide() {
                currentIndex = (currentIndex - 1 + totalImages) % totalImages; // Ensures index wraps correctly for negative values
                updateSlider();
            }

            // Function to start the automatic slide show
            function startAutoSlide() {
                stopAutoSlide(); // Clear any existing interval before starting a new one
                autoSlideInterval = setInterval(goToNextSlide, 3000); // Change slide every 3 seconds
            }

            // Function to stop the automatic slide show
            function stopAutoSlide() {
                if (autoSlideInterval) {
                    clearInterval(autoSlideInterval);
                    autoSlideInterval = null; // Reset the interval ID
                }
            }

            // Event listener for the "Next" button
            nextBtn.addEventListener('click', () => {
                stopAutoSlide(); // Pause auto-slide on manual interaction
                goToNextSlide();
                startAutoSlide(); // Resume auto-slide after interaction
            });

            // Event listener for the "Previous" button
            prevBtn.addEventListener('click', () => {
                stopAutoSlide(); // Pause auto-slide on manual interaction
                goToPrevSlide();
                startAutoSlide(); // Resume auto-slide after interaction
            });

            // Event listeners for navigation dots
            dots.forEach(dot => {
                dot.addEventListener('click', (event) => {
                    stopAutoSlide(); // Pause auto-slide on manual interaction
                    const index = parseInt(event.target.getAttribute('data-index'));
                    currentIndex = index;
                    updateSlider();
                    startAutoSlide(); // Resume auto-slide after interaction
                });
            });

            // Event listeners to pause/resume auto-slide on mouse hover
            sliderContainer.addEventListener('mouseenter', stopAutoSlide);
            sliderContainer.addEventListener('mouseleave', startAutoSlide);

            // Initial setup: display the first image and start auto-sliding
            updateSlider();
            startAutoSlide();
        });
    </script>
</body>
</html>

                    HELLO
                </div>
            </div>

            <div id="sermons-page" class="page-content hidden">
                <div class="p-6 bg-white rounded-xl shadow-lg card">
                    <h2 class="text-2xl font-bold text-blue-800 mb-4">Sermones</h2>
                    <p class="text-gray-700 mb-6">Escuche y aprenda de nuestros sermones pasados.</p>
                    <ul class="space-y-4" id="sermons-list">
                        </ul>
                </div>
            </div>

            <div id="bible-page" class="page-content hidden">
                <div class="p-6 bg-white rounded-xl shadow-lg card">
                <!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>La Santa Biblia</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom font for the entire page */
        body {
            font-family: 'Inter', sans-serif;
        }
    </style>
</head>
<body class="bg-gradient-to-br from-blue-50 to-indigo-100 min-h-screen flex flex-col text-gray-800">

    <header class="bg-white shadow-md py-4 px-6 md:px-8 lg:px-12 rounded-b-xl">
        <div class="container mx-auto flex flex-col md:flex-row items-center justify-between">
            <h1 class="text-3xl font-extrabold text-blue-700 mb-2 md:mb-0">
                La Santa Biblia
            </h1>
            <nav class="space-x-4">
                </nav>
        </div>
    </header>

    <main class="flex-grow container mx-auto p-6 md:p-8 lg:p-10 flex flex-col items-center">

        <div class="bg-white p-6 md:p-8 rounded-xl shadow-lg w-full max-w-2xl mb-8 border border-blue-200">
            <label for="bibleVersionSelect" class="block text-sm font-medium text-gray-700 mb-2">Seleccionar Versión de la Biblia:</label>
            <select id="bibleVersionSelect" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-200">
                <option value="">Cargando versiones...</option>
            </select>
        </div>

        <div class="bg-white p-6 md:p-8 rounded-xl shadow-lg w-full max-w-2xl mb-8 border border-blue-200">
            <h2 class="text-2xl font-semibold text-blue-700 mb-4 text-center">Cargar Capítulo Completo</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-4">
                <div>
                    <label for="bookSelectChapter" class="block text-sm font-medium text-gray-700 mb-2">Seleccionar Libro:</label>
                    <select id="bookSelectChapter" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-200">
                        <option value="">Seleccionar un libro</option>
                    </select>
                </div>
                <div>
                    <label for="chapterSelectChapter" class="block text-sm font-medium text-gray-700 mb-2">Seleccionar Capítulo:</label>
                    <select id="chapterSelectChapter" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-200" disabled>
                        <option value="">Seleccionar un libro primero</option>
                    </select>
                </div>
            </div>
            <button id="loadChapterBtn" class="w-full bg-blue-600 text-white py-3 rounded-lg font-bold hover:bg-blue-700 transition duration-300 shadow-md">
                Cargar Capítulo
            </button>
        </div>

        <div class="bg-white p-6 md:p-8 rounded-xl shadow-lg w-full max-w-2xl mb-8 border border-blue-200">
            <h2 class="text-2xl font-semibold text-blue-700 mb-4 text-center">Buscar Versículo(s)</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4 mb-4">
                <div>
                    <label for="bookInputVerse" class="block text-sm font-medium text-gray-700 mb-2">Libro:</label>
                    <input type="text" id="bookInputVerse" placeholder="ej., Juan" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-200">
                </div>
                <div>
                    <label for="chapterInputVerse" class="block text-sm font-medium text-gray-700 mb-2">Capítulo:</label>
                    <input type="number" id="chapterInputVerse" placeholder="ej., 3" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-200">
                </div>
                <div>
                    <label for="startVerseInput" class="block text-sm font-medium text-gray-700 mb-2">Versículo Inicial:</label>
                    <input type="number" id="startVerseInput" placeholder="ej., 16" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-200">
                </div>
                <div>
                    <label for="endVerseInput" class="block text-sm font-medium text-gray-700 mb-2">Versículo Final (Opcional):</label>
                    <input type="number" id="endVerseInput" placeholder="ej., 17" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-200">
                </div>
            </div>
            <button id="lookupVersesBtn" class="w-full bg-blue-600 text-white py-3 rounded-lg font-bold hover:bg-blue-700 transition duration-300 shadow-md">
                Buscar Versículo(s)
            </button>
        </div>

        <div id="chapterDisplay" class="bg-white p-6 md:p-8 rounded-xl shadow-lg w-full max-w-3xl mb-8 border border-blue-200">
            <h2 class="text-2xl font-semibold text-blue-700 mb-4 text-center" id="chapterReference">Bienvenido a La Santa Biblia</h2>
            <div class="text-lg leading-relaxed text-gray-700 text-center" id="chapterContent">
                <p>Selecciona una versión de la Biblia, libro y capítulo arriba para empezar a leer.</p>
                <p>Por ejemplo, prueba "Juan" capítulo "3" con la "Versión Reina-Valera".</p>
            </div>
        </div>

        <div id="verseLookupDisplay" class="bg-white p-6 md:p-8 rounded-xl shadow-lg w-full max-w-3xl border border-blue-200 hidden">
            <h2 class="text-2xl font-semibold text-blue-700 mb-4 text-center" id="verseLookupReference"></h2>
            <div class="text-lg leading-relaxed text-gray-700 text-center" id="verseLookupContent"></div>
        </div>

        <div id="messageBox" class="fixed bottom-4 right-4 bg-red-500 text-white p-4 rounded-lg shadow-xl hidden z-50">
            <p id="messageText"></p>
            <button class="absolute top-1 right-2 text-white font-bold" onclick="document.getElementById('messageBox').classList.add('hidden')">&times;</button>
        </div>

    </main>

    <footer class="bg-white shadow-inner py-4 px-6 md:px-8 lg:px-12 mt-8 rounded-t-xl">
        <div class="container mx-auto text-center text-gray-600">
            &copy; 2025 Sitio Web La Santa Biblia. Todos los derechos reservados.
        </div>
    </footer>

    <script type="module">
        function showMessageBox(message) {
            const messageBox = document.getElementById('messageBox');
            const messageText = document.getElementById('messageText');
            messageText.textContent = message;
            messageBox.classList.remove('hidden');
            setTimeout(() => {
                messageBox.classList.add('hidden');
            }, 3000);
        }

        const SCRIPTURE_API_KEY = '77d6e18f041437e25b504841f8850bb2';
        let currentBooks = [];
        let currentChapters = [];

        async function fetchBibleVersions() {
            const bibleVersionSelect = document.getElementById('bibleVersionSelect');
            const apiUrl = 'https://api.scripture.api.bible/v1/bibles';

            try {
                const response = await fetch(apiUrl, {
                    method: 'GET',
                    headers: {
                        'api-key': SCRIPTURE_API_KEY,
                        'Accept': 'application/json'
                    }
                });

                if (!response.ok) {
                    const errorData = await response.json();
                    throw new Error(errorData.message || `API error: ${response.status}`);
                }

                const result = await response.json();
                const bibles = result.data;

                bibleVersionSelect.innerHTML = '';

                if (bibles && bibles.length > 0) {
                    bibles.sort((a, b) => a.name.localeCompare(b.name));

                    bibles.forEach(bible => {
                        const option = document.createElement('option');
                        option.value = bible.id;
                        option.textContent = bible.name;
                        if (bible.id === 'de4e12af7f28f599-01') { // KJV Bible ID
                            option.selected = true;
                        }
                        bibleVersionSelect.appendChild(option);
                    });
                    fetchBooksForBible(bibleVersionSelect.value, 'chapter');
                    fetchBooksForBible(bibleVersionSelect.value, 'verse');
                } else {
                    const option = document.createElement('option');
                    option.value = '';
                    option.textContent = 'No se encontraron versiones';
                    bibleVersionSelect.appendChild(option);
                    showMessageBox("No se pudieron cargar versiones de la Biblia.");
                }
            } catch (error) {
                console.error("Error al cargar versiones de la Biblia:", error);
                const option = document.createElement('option');
                option.value = '';
                option.textContent = 'Error al cargar versiones';
                bibleVersionSelect.innerHTML = '';
                bibleVersionSelect.appendChild(option);
                showMessageBox(`Error al cargar versiones de la Biblia: ${error.message}`);
            }
        }

        async function fetchBooksForBible(bibleId, section) {
            const bookSelectChapter = document.getElementById('bookSelectChapter');
            const chapterSelectChapter = document.getElementById('chapterSelectChapter');

            if (section === 'chapter') {
                bookSelectChapter.innerHTML = '<option value="">Cargando libros...</option>';
                bookSelectChapter.disabled = true;
                chapterSelectChapter.innerHTML = '<option value="">Seleccionar un libro primero</option>';
                chapterSelectChapter.disabled = true;
            }

            if (!bibleId) return;

            const apiUrl = `https://api.scripture.api.bible/v1/bibles/${bibleId}/books`;
            try {
                const response = await fetch(apiUrl, {
                    method: 'GET',
                    headers: {
                        'api-key': SCRIPTURE_API_KEY,
                        'Accept': 'application/json'
                    }
                });

                if (!response.ok) {
                    const errorData = await response.json();
                    throw new Error(errorData.message || `Error de API al buscar libros: ${response.status}`);
                }

                const result = await response.json();
                currentBooks = result.data;

                if (section === 'chapter') {
                    bookSelectChapter.innerHTML = '<option value="">Seleccionar un libro</option>';
                    if (currentBooks && currentBooks.length > 0) {
                        currentBooks.forEach(book => {
                            const option = document.createElement('option');
                            option.value = book.id;
                            option.textContent = book.name;
                            bookSelectChapter.appendChild(option);
                        });
                        bookSelectChapter.disabled = false;
                    } else {
                        bookSelectChapter.innerHTML = '<option value="">No se encontraron libros</option>';
                        showMessageBox("No se encontraron libros para la versión de la Biblia seleccionada.");
                    }
                }
            } catch (error) {
                console.error("Error al cargar libros para la Biblia:", error);
                if (section === 'chapter') {
                    bookSelectChapter.innerHTML = '<option value="">Error al cargar libros</option>';
                }
                showMessageBox(`Error al cargar libros para esta versión: ${error.message}`);
            }
        }

        async function fetchChaptersForBook(bibleId, bookId, section) {
            const chapterSelectChapter = document.getElementById('chapterSelectChapter');

            if (section === 'chapter') {
                chapterSelectChapter.innerHTML = '<option value="">Cargando capítulos...</option>';
                chapterSelectChapter.disabled = true;
            }

            if (!bibleId || !bookId) return;

            const apiUrl = `https://api.scripture.api.bible/v1/bibles/${bibleId}/books/${bookId}/chapters`;
            try {
                const response = await fetch(apiUrl, {
                    method: 'GET',
                    headers: {
                        'api-key': SCRIPTURE_API_KEY,
                        'Accept': 'application/json'
                    }
                });

                if (!response.ok) {
                    const errorData = await response.json();
                    throw new Error(errorData.message || `Error de API al buscar capítulos: ${response.status}`);
                }

                const result = await response.json();
                currentChapters = result.data;

                if (section === 'chapter') {
                    chapterSelectChapter.innerHTML = '<option value="">Seleccionar un capítulo</option>';
                    if (currentChapters && currentChapters.length > 0) {
                        currentChapters.forEach(chapter => {
                            if (chapter.number && chapter.number !== "0") {
                                const option = document.createElement('option');
                                option.value = chapter.id;
                                option.textContent = `Capítulo ${chapter.number}`;
                                chapterSelectChapter.appendChild(option);
                            }
                        });
                        chapterSelectChapter.disabled = false;
                    } else {
                        chapterSelectChapter.innerHTML = '<option value="">No se encontraron capítulos</option>';
                        showMessageBox("No se encontraron capítulos para el libro seleccionado.");
                    }
                }
            } catch (error) {
                console.error("Error al cargar capítulos para el libro:", error);
                if (section === 'chapter') {
                    chapterSelectChapter.innerHTML = '<option value="">Error al cargar capítulos</option>';
                }
                showMessageBox(`Error al cargar capítulos para este libro: ${error.message}`);
            }
        }

        window.onload = fetchBibleVersions;

        document.getElementById('bibleVersionSelect').addEventListener('change', (event) => {
            const selectedBibleId = event.target.value;
            fetchBooksForBible(selectedBibleId, 'chapter');
            fetchBooksForBible(selectedBibleId, 'verse');
        });

        document.getElementById('bookSelectChapter').addEventListener('change', (event) => {
            const selectedBibleId = document.getElementById('bibleVersionSelect').value;
            const selectedBookId = event.target.value;
            fetchChaptersForBook(selectedBibleId, selectedBookId, 'chapter');
        });

        document.getElementById('loadChapterBtn').addEventListener('click', async () => {
            const bibleVersionSelect = document.getElementById('bibleVersionSelect');
            const bookSelect = document.getElementById('bookSelectChapter');
            const chapterSelect = document.getElementById('chapterSelectChapter');

            const selectedBibleId = bibleVersionSelect.value;
            const selectedBookId = bookSelect.value;
            const selectedChapterId = chapterSelect.value;

            const chapterReferenceElement = document.getElementById('chapterReference');
            const chapterContentElement = document.getElementById('chapterContent');
            const verseLookupDisplay = document.getElementById('verseLookupDisplay');

            verseLookupDisplay.classList.add('hidden');
            document.getElementById('chapterDisplay').classList.remove('hidden');

            if (!selectedBibleId || !selectedBookId || !selectedChapterId) {
                showMessageBox("Por favor, selecciona una versión de la Biblia, libro y capítulo para cargar un capítulo completo.");
                return;
            }

            const selectedBookName = bookSelect.options[bookSelect.selectedIndex].textContent;
            const selectedChapterNumber = chapterSelect.options[chapterSelect.selectedIndex].textContent.replace('Capítulo ', '');
            const selectedBibleName = bibleVersionSelect.options[bibleVersionSelect.selectedIndex].textContent;

            chapterReferenceElement.textContent = `Cargando ${selectedBookName} Capítulo ${selectedChapterNumber} (${selectedBibleName})...`;
            chapterContentElement.innerHTML = "<p>Por favor espera...</p>";

            try {
                const chapterContentApiUrl = `https://api.scripture.api.bible/v1/bibles/${selectedBibleId}/chapters/${selectedChapterId}`;
                const chapterContentResponse = await fetch(chapterContentApiUrl, {
                    method: 'GET',
                    headers: {
                        'api-key': SCRIPTURE_API_KEY,
                        'Accept': 'application/json'
                    }
                });

                if (!chapterContentResponse.ok) {
                    const errorData = await chapterContentResponse.json();
                    throw new Error(errorData.message || `Error de API al cargar el contenido del capítulo: ${chapterContentResponse.status}`);
                }

                const chapterResult = await chapterContentResponse.json();

                if (chapterResult.data && chapterResult.data.content) {
                    const parser = new DOMParser();
                    const doc = parser.parseFromString(chapterResult.data.content, 'text/html');

                    doc.querySelectorAll('.footnote, .crossreference, .chapternum').forEach(el => el.remove());

                    doc.querySelectorAll('.versenum').forEach(el => {
                        el.outerHTML = `<span class="font-bold text-blue-700 mr-1">${el.textContent}</span>`;
                    });

                    chapterReferenceElement.textContent = `${chapterResult.data.reference}`;
                    chapterContentElement.innerHTML = doc.body.innerHTML;

                } else {
                    chapterReferenceElement.textContent = "Capítulo No Encontrado";
                    chapterContentElement.innerHTML = "<p>El capítulo solicitado no pudo ser encontrado. Por favor, verifica tu entrada.</p>";
                    showMessageBox("Capítulo no encontrado. Por favor, verifica el libro y el capítulo.");
                }
            } catch (error) {
                console.error("Error al cargar capítulo:", error);
                chapterReferenceElement.textContent = "Error al Cargar Capítulo";
                chapterContentElement.innerHTML = "<p>Hubo un error al cargar el capítulo. Por favor, verifica tu entrada o inténtalo de nuevo más tarde.</p>";
                showMessageBox(`Error: ${error.message}. Consulta la consola para más detalles.`);
            }
        });

        document.getElementById('lookupVersesBtn').addEventListener('click', async () => {
            const bibleVersionSelect = document.getElementById('bibleVersionSelect');
            const bookInputVerse = document.getElementById('bookInputVerse').value.trim();
            const chapterInputVerse = document.getElementById('chapterInputVerse').value.trim();
            const startVerseInput = document.getElementById('startVerseInput').value.trim();
            const endVerseInput = document.getElementById('endVerseInput').value.trim();

            const selectedBibleId = bibleVersionSelect.value;

            const verseLookupReferenceElement = document.getElementById('verseLookupReference');
            const verseLookupContentElement = document.getElementById('verseLookupContent');
            const verseLookupDisplay = document.getElementById('verseLookupDisplay');
            const chapterDisplay = document.getElementById('chapterDisplay');

            chapterDisplay.classList.add('hidden');
            verseLookupDisplay.classList.remove('hidden');

            if (!selectedBibleId || !bookInputVerse || !chapterInputVerse || !startVerseInput) {
                showMessageBox("Por favor, selecciona una versión de la Biblia e introduce un libro, capítulo y versículo inicial para la búsqueda de versículos.");
                return;
            }

            const apiBookId = currentBooks.find(b => b.name.toLowerCase() === bookInputVerse.toLowerCase() || b.abbreviation?.toLowerCase() === bookInputVerse.toLowerCase())?.id;

            if (!apiBookId) {
                showMessageBox(`Libro "${bookInputVerse}" no encontrado o reconocido para la versión de la Biblia seleccionada.`);
                verseLookupReferenceElement.textContent = "Libro No Encontrado";
                verseLookupContentElement.innerHTML = "<p>Por favor, introduce un nombre de libro o abreviatura válido.</p>";
                return;
            }

            let verseIdString = `${apiBookId}.${chapterInputVerse}.${startVerseInput}`;
            if (endVerseInput && parseInt(endVerseInput) > parseInt(startVerseInput)) {
                verseIdString += `-${apiBookId}.${chapterInputVerse}.${endVerseInput}`;
            }

            verseLookupReferenceElement.textContent = `Cargando ${bookInputVerse} ${chapterInputVerse}:${startVerseInput}${endVerseInput ? '-' + endVerseInput : ''} (${bibleVersionSelect.options[bibleVersionSelect.selectedIndex].text})...`;
            verseLookupContentElement.innerHTML = "<p>Por favor espera...</p>";

            try {
                const verseApiUrl = `https://api.scripture.api.bible/v1/bibles/${selectedBibleId}/verses/${verseIdString}`;
                const verseResponse = await fetch(verseApiUrl, {
                    method: 'GET',
                    headers: {
                        'api-key': SCRIPTURE_API_KEY,
                        'Accept': 'application/json'
                    }
                });

                if (!verseResponse.ok) {
                    const errorData = await verseResponse.json();
                    throw new Error(errorData.message || `Error de API al buscar versículo(s): ${verseResponse.status}`);
                }

                const verseResult = await verseResponse.json();

                if (verseResult.data && verseResult.data.content) {
                    const parser = new DOMParser();
                    const doc = parser.parseFromString(verseResult.data.content, 'text/html');

                    doc.querySelectorAll('.footnote, .crossreference, .chapternum').forEach(el => el.remove());
                     doc.querySelectorAll('.versenum').forEach(el => {
                        el.outerHTML = `<span class="font-bold text-blue-700 mr-1">${el.textContent}</span>`;
                    });

                    verseLookupReferenceElement.textContent = `${verseResult.data.reference}`;
                    verseLookupContentElement.innerHTML = doc.body.innerHTML;
                } else {
                    verseLookupReferenceElement.textContent = "Versículo(s) No Encontrado(s)";
                    verseLookupContentElement.innerHTML = "<p>El/los versículo(s) solicitado(s) no pudo(pudieron) ser encontrado(s). Por favor, verifica tu entrada.</p>";
                    showMessageBox("Versículo(s) no encontrado(s). Por favor, verifica el libro, capítulo y versículo(s).");
                }
            } catch (error) {
                console.error("Error al cargar versículo(s):", error);
                verseLookupReferenceElement.textContent = "Error al Cargar Versículo(s)";
                verseLookupContentElement.innerHTML = "<p>Hubo un error al cargar el/los versículo(s). Por favor, verifica tu entrada o inténtalo de nuevo más tarde.</p>";
                showMessageBox(`Error: ${error.message}. Consulta la consola para más detalles.`);
            }
        });
    </script>
</body>
                </div>
            </div>

            <div id="contact-page" class="page-content hidden">
                <div class="p-6 bg-white rounded-xl shadow-lg card">
                    <h2 class="text-2xl font-bold text-blue-800 mb-4">Contacto</h2>
                    <p class="text-gray-700 mb-4">
                        Estamos aquí para servirle. No dude en ponerse en contacto con nosotros para cualquier pregunta o necesidad.
                    </p>
                    <div class="space-y-4">
                        <div class="flex items-center text-gray-700">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 mr-3 text-blue-700">
                                <rect width="20" height="16" x="2" y="4" rx="2"></rect>
                                <path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"></path>
                            </svg>
                            <span>info@laiglesiadediosisraelita.online</span>
                        </div>
                        <div class="flex items-center text-gray-700">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 mr-3 text-blue-700">
                                <path d="m3 9 9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"></path>
                                <polyline points="9 22 9 12 15 12 15 22"></polyline>
                            </svg>
                            <span>[Dirección de la Iglesia, Ciudad, País]</span>
                        </div>
                    </div>
                    <form id="contact-form" class="mt-6 space-y-4">
                        <div>
                            <label for="name" class="block text-sm font-medium text-gray-700">Nombre</label>
                            <input type="text" id="name" class="input-field mt-1 block w-full shadow-sm" />
                        </div>
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-700">Correo Electrónico</label>
                            <input type="email" id="email" class="input-field mt-1 block w-full shadow-sm" />
                        </div>
                        <div>
                            <label for="message" class="block text-sm font-medium text-gray-700">Mensaje</label>
                            <textarea id="message" rows="4" class="textarea-field mt-1 block w-full shadow-sm"></textarea>
                        </div>
                        <button type="submit" class="primary-button flex items-center justify-center cursor-pointer">
                            Enviar Mensaje
                        </button>
                    </form>
                </div>
            </div>
        </main>

        <aside id="sidebar" class="fixed inset-y-0 right-0 z-40 w-64 bg-blue-800 text-white transform translate-x-full transition-transform duration-300 ease-in-out">
            <div class="p-4 border-b border-blue-700 flex items-center justify-between sidebar-header">
                <h2 class="text-xl font-semibold text-blue-300 sidebar-title">Menú</h2>
                <button id="sidebar-close-button" class="ghost-button h-10 w-10 flex items-center justify-center rounded-md text-blue-300 hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-200 cursor-pointer">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-6 w-6">
                        <line x1="18" x2="6" y1="6" y2="18"></line>
                        <line x1="6" x2="18" y1="6" y2="18"></line>
                    </svg>
                </button>
            </div>
            <nav class="mt-5">
                <ul>
                    <li>
                        <a href="#" class="sidebar-nav-link flex items-center py-3 px-4 transition-colors duration-200" data-page="home">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 mr-3 text-blue-400">
                                <path d="m3 9 9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"></path>
                                <polyline points="9 22 9 12 15 12 15 22"></polyline>
                            </svg>
                            <span>Inicio</span>
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 ml-auto text-blue-400">
                                <polyline points="9 18 15 12 9 6"></polyline>
                            </svg>
                        </a>
                    </li>
                    <li>
                        <a href="#" class="sidebar-nav-link flex items-center py-3 px-4 transition-colors duration-200" data-page="about">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-6 w-6 mr-3 text-blue-400">
                                <circle cx="12" cy="12" r="10"></circle>
                                <path d="M12 16v-4"></path>
                                <path d="M12 8h.01"></path>
                            </svg>
                            <span>Acerca de Nosotros</span>
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 ml-auto text-blue-400">
                                <polyline points="9 18 15 12 9 6"></polyline>
                            </svg>
                        </a>
                    </li>
                    <li>
                        <a href="#" class="sidebar-nav-link flex items-center py-3 px-4 transition-colors duration-200" data-page="sermons">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 mr-3 text-blue-400">
                                <path d="M4 19.5v-15A2.5 2.5 0 0 1 6.5 2H20v20H6.5a2.5 2.5 0 0 1 0-5H20"></path>
                            </svg>
                            <span>Sermones</span>
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 ml-auto text-blue-400">
                                <polyline points="9 18 15 12 9 6"></polyline>
                            </svg>
                        </a>
                    </li>
                    <li>
                        <a href="#" class="sidebar-nav-link flex items-center py-3 px-4 transition-colors duration-200" data-page="bible">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 mr-3 text-blue-400">
                                <path d="M4 19.5v-15A2.5 2.5 0 0 1 6.5 2H20v20H6.5a2.5 2.5 0 0 1 0-5H20"></path>
                            </svg>
                            <span>Biblia</span>
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 ml-auto text-blue-400">
                                <polyline points="9 18 15 12 9 6"></polyline>
                            </svg>
                        </a>
                    </li>
                    <li>
                        <a href="#" class="sidebar-nav-link flex items-center py-3 px-4 transition-colors duration-200" data-page="contact">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 mr-3 text-blue-400">
                                <rect width="20" height="16" x="2" y="4" rx="2"></rect>
                                <path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"></path>
                            </svg>
                            <span>Contacto</span>
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-5 w-5 ml-auto text-blue-400">
                                <polyline points="9 18 15 12 9 6"></polyline>
                            </svg>
                        </a>
                    </li>
                </ul>
            </nav>
        </aside>

        <div id="sidebar-overlay" class="fixed inset-0 bg-black bg-opacity-50 z-30 hidden"></div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const menuToggleButton = document.getElementById('menu-toggle-button');
            const sidebar = document.getElementById('sidebar');
            const sidebarCloseButton = document.getElementById('sidebar-close-button');
            const sidebarOverlay = document.getElementById('sidebar-overlay');
            const navLinks = document.querySelectorAll('.sidebar-nav-link');
            const pageContents = document.querySelectorAll('.page-content');
            const mainContent = document.getElementById('main-content');

            // Mock Sermons Data
            const sermonsData = [
                { id: 1, title: 'La Importancia de la Fe', speaker: 'Pastor Juan Pérez', date: '2023-10-29' },
                { id: 2, title: 'El Amor Incondicional de Dios', speaker: 'Hermana María García', date: '2023-10-22' },
                { id: 3, title: 'Viviendo en Gracia', speaker: 'Pastor Juan Pérez', date: '2023-10-15' },
            ];

            let isSidebarOpen = false;
            let currentPageElement = null; // To keep track of the currently active page element

            // Function to toggle sidebar visibility
            function toggleSidebar() {
                isSidebarOpen = !isSidebarOpen;
                if (isSidebarOpen) {
                    sidebar.classList.remove('translate-x-full');
                    sidebar.classList.add('translate-x-0');
                    sidebarOverlay.classList.remove('hidden');
                } else {
                    sidebar.classList.remove('translate-x-0');
                    sidebar.classList.add('translate-x-full');
                    sidebarOverlay.classList.add('hidden');
                }
            }

            // Function to show a specific page with transition
            function showPage(pageId) {
                const targetPageElement = document.getElementById(`${pageId}-page`);

                if (currentPageElement === targetPageElement) {
                    // Already on this page, just close sidebar if open
                    if (isSidebarOpen) toggleSidebar();
                    return;
                }

                if (currentPageElement) {
                    // Start fade-out for current page
                    currentPageElement.classList.remove('active');
                    currentPageElement.classList.add('hidden'); // Hide after transition
                }

                // Wait for the current page to fade out (or immediately if no current page)
                setTimeout(() => {
                    if (targetPageElement) {
                        pageContents.forEach(page => {
                            page.classList.add('hidden'); // Ensure all others are hidden
                            page.classList.remove('active'); // Ensure others don't have active
                        });
                        targetPageElement.classList.remove('hidden');
                        // Trigger reflow to ensure transition runs
                        void targetPageElement.offsetWidth;
                        targetPageElement.classList.add('active');
                        currentPageElement = targetPageElement;
                    }
                    mainContent.scrollTo({ top: 0, behavior: 'smooth' }); // Scroll to top
                }, currentPageElement ? 300 : 0); // Delay matches CSS transition duration
            }


            // Function to render sermons
            function renderSermons() {
                const sermonsList = document.getElementById('sermons-list');
                if (sermonsList) {
                    sermonsList.innerHTML = ''; // Clear existing sermons
                    sermonsData.forEach(sermon => {
                        const li = document.createElement('li');
                        li.className = 'border border-blue-100 rounded-xl p-4 flex items-center justify-between bg-white sermon-item'; /* Added sermon-item class */
                        li.innerHTML = `
                            <div>
                                <h3 class="text-lg font-semibold text-blue-800">${sermon.title}</h3>
                                <p class="text-sm text-gray-600">Por: ${sermon.speaker} | ${sermon.date}</p>
                            </div>
                            <button class="primary-button h-8 px-3 text-sm flex items-center justify-center cursor-pointer">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide-icon h-4 w-4 mr-2">
                                    <circle cx="12" cy="12" r="10"></circle>
                                    <polygon points="10 8 16 12 10 16 10 8"></polygon>
                                </svg>
                                Escuchar
                            </button>
                        `;
                        sermonsList.appendChild(li);
                    });
                }
            }

            // Event Listeners
            menuToggleButton.addEventListener('click', toggleSidebar);
            sidebarCloseButton.addEventListener('click', toggleSidebar);
            sidebarOverlay.addEventListener('click', toggleSidebar);

            navLinks.forEach(link => {
                link.addEventListener('click', (event) => {
                    event.preventDefault();
                    const page = event.currentTarget.dataset.page;
                    showPage(page);
                    if (isSidebarOpen) {
                        toggleSidebar(); // Close sidebar after clicking a link
                    }
                });
            });

            // Handle contact form submission (example)
            const contactForm = document.getElementById('contact-form');
            if (contactForm) {
                contactForm.addEventListener('submit', (event) => {
                    event.preventDefault();
                    const name = document.getElementById('name').value;
                    const email = document.getElementById('email').value;
                    const message = document.getElementById('message').value;

                    // In a real application, you would send this data to a server
                    console.log('Contact Form Submitted:', { name, email, message });
                    alert('Mensaje enviado. ¡Gracias por contactarnos!'); // Using alert for demonstration
                    contactForm.reset();
                });
            }

            // Initial page load
            showPage('home');
            renderSermons(); // Render sermons on initial load
        });
    </script>
</body>
</html>
