<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moss Frame</title>

    <!-- 1. External Imports -->
    <link rel="preconnect" href="https://googleapis.com">
    <link rel="preconnect" href="https://gstatic.com" crossorigin>
    <link href="https://googleapis.com/css2?family=Lora:ital,wght@0,400..700;1,400..700&display=swap" rel="stylesheet">
    
    <!-- Sirv Application Core Engine Script -->
    <script src="https://scripts.sirv.com/sirvjs/v3/sirv.js"></script>

    <!-- 2. UI & Hotspot CSS Engine Overrides -->
    <style>
        /* Base page cleanup to make asset visible */
        body {
            margin: 0;
            padding: 40px;
            background-color: #1c2321;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        /* Root Theme Token Variables */
        :root {
            --accent-cream: #FDFCE8;
            --dark-bg: #1c2321;
        }

        /* Responsive Frame Wrapper */
        .spin-container {
            width: 100%;
            max-width: 600px;
            aspect-ratio: 1 / 1;
        }

        /* Hotspot Node Customization */
        .sirv-hotspot-pointer.pulsating-point::before {
            background-color: var(--accent-cream) !important;
            transform: scale(1.1);
        }
        .sirv-hotspot-pointer.pulsating-point::after {
            border: 2px solid var(--accent-cream) !important;
        }

        /* Text Box Content Overrides */
        .sirv-hotspot-tooltip {
            font-family: 'Lora', serif !important;
            font-size: 12px !important;
            background: var(--dark-bg) !important;
            color: var(--accent-cream) !important;
            border: 1px solid var(--accent-cream) !important;
        }

        /* Navigation UI Overlay Styles */
        .sirv-spin-arrows {
            color: var(--accent-cream) !important;
        }
    </style>
</head>
<body>

    <!-- 3. Configured Application Entry Point Wrapped inside a Layout Container -->
    <div class="spin-container">
        <div class="Sirv" data-src="https://sirv.com" data-options="arrows: always; hint: false;"></div>
    </div>

</body>
</html>
