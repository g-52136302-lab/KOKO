<!DOCTYPE html>
<html lang="ms">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>e-Pencapaian - SMKA Tun Ahmadshah</title>
    
    <!-- SDK & Frameworks -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf-autotable/3.5.28/jspdf.plugin.autotable.min.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;700&family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
 
    <style>
        :root {
            --neon-cyan: #06b6d4;
            --neon-blue: #3b82f6;
            --neon-purple: #a855f7;
            --glass-bg: rgba(15, 23, 42, 0.45);
            --glass-border: rgba(255, 255, 255, 0.1);
        }
        
        body { 
            font-family: 'Plus Jakarta Sans', sans-serif; 
            background-color: #020617;
            color: #f8fafc;
            overflow: hidden;
            height: 100vh;
        }
 
        .font-header { font-family: 'Space Grotesk', sans-serif; }
        
        .bg-cyber {
            background: 
                radial-gradient(circle at 20% 30%, rgba(6, 182, 212, 0.15) 0%, transparent 40%),
                radial-gradient(circle at 80% 70%, rgba(99, 102, 241, 0.15) 0%, transparent 40%),
                linear-gradient(to bottom, #020617, #0f172a);
        }
        
        .dot-grid {
            background-image: radial-gradient(rgba(255,255,255,0.05) 1px, transparent 1px);
            background-size: 30px 30px;
        }
        
        .silhouette {
            position: absolute;
            left: 50%; top: 50%;
            transform: translate(-50%, -50%);
            width: 700px;
            opacity: 0.4;
            mask-image: radial-gradient(circle, black 55%, transparent 95%);
            pointer-events: none;
            z-index: 0;
            filter: drop-shadow(0 0 40px rgba(6, 182, 212, 0.4)) saturate(1.5);
        }
 
        .glass {
            background: var(--glass-bg);
            backdrop-filter: blur(25px);
            -webkit-backdrop-filter: blur(25px);
            border: 1px solid var(--glass-border);
            box-shadow: 0 10px 30px -10px rgba(0, 0, 0, 0.7);
        }
 
        .
