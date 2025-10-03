# mom-birthday-card
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy 55th Birthday, Mom!</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Lora:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Lora', serif;
            background: linear-gradient(135deg, #f5e7e9 0%, #e8e4f1 100%);
        }
        .card {
            background: #fff9f9;
            border: 2px solid #d4af37;
            border-radius: 15px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        .sparkle {
            position: absolute;
            width: 8px;
            height: 8px;
            background: radial-gradient(circle, #d4af37, transparent);
            border-radius: 50%;
            animation: sparkle 2s ease-in-out infinite;
        }
        @keyframes sparkle {
            0% { transform: scale(0); opacity: 1; }
            100% { transform: scale(1.8); opacity: 0; }
        }
        .hidden { display: none; }
        .heading {
            font-family: 'Playfair Display', serif;
            color: #4a2c4a;
        }
        .subheading {
            font-family: 'Lora', serif;
            color: #6b4e71;
        }
        .quote {
            font-style: italic;
            color: #5c4033;
        }
        .mystery-box {
            background: linear-gradient(45deg, #6b4e71, #d4af37);
            transition: transform 0.3s ease;
        }
        .mystery-box:hover {
            transform: scale(1.05);
        }
        .bible-verse {
            background: #f8f1e9;
            border-left: 4px solid #d4af37;
        }
    </style>
</head>
<body class="flex items-center justify-center min-h-screen">
    <div id="card" class="card p-10 max-w-3xl text-center">
        <h1 class="heading text-5xl font-bold mb-6">HAPPY 55TH BIRTHDAY FOR THE WORLDS BEST MOM</h1>
        <h2 class="subheading text-2xl mb-8">~ From Lydia, David, Esther, Debbi & Pops</h2>
        <p class="text-lg text-gray-700 mb-6 leading-relaxed">
            Dear Mom, your love and care light up our lives every day. You are our rock, our joy, and the heart of our family. 
            Thank you for your endless sacrifices and unconditional love. We are so blessed to have you!
        </p>
        <div class="mb-8">
            <h3 class="subheading text-xl font-semibold mb-4">Quotes for the Best Mom in the World</h3>
            <p class="quote text-gray-600 mb-2">"A mother is she who can take the place of all others but whose place no one else can take." – Cardinal Mermillod</p>
            <p class="quote text-gray-600 mb-2">"The heart of a mother is a deep abyss at the bottom of which you will always find forgiveness." – Honoré de Balzac</p>
            <p class="quote text-gray-600">"A mother's love is the fuel that enables a normal human being to do the impossible." – Marion C. Garretty</p>
        </div>
        <div id="mystery-box" class="mystery-box relative p-8 rounded-lg cursor-pointer" onclick="revealSurprise()">
            <h3 class="text-2xl text-white font-bold">Mystery Box of Surprises!</h3>
            <div class="sparkle" style="top: 10px; left: 20px;"></div>
            <div class="sparkle" style="top: 30px; right: 30px;"></div>
            <div class="sparkle" style="bottom: 15px; left: 50px;"></div>
            <div class="sparkle" style="bottom: 20px; right: 20px;"></div>
        </div>
        <div id="surprise" class="hidden mt-8">
            <h3 class="subheading text-2xl font-semibold mb-6">Our Special Memories</h3>
            <div class="grid grid-cols-2 gap-6 mb-8">
                <!-- Replace these with your image URLs or file paths -->
                <img src="https://via.placeholder.com/150" alt="Family Photo 1" class="rounded-lg shadow-md">
                <img src="https://via.placeholder.com/150" alt="Family Photo 2" class="rounded-lg shadow-md">
                <img src="https://via.placeholder.com/150" alt="Family Photo 3" class="rounded-lg shadow-md">
                <img src="https://via.placeholder.com/150" alt="Family Photo 4" class="rounded-lg shadow-md">
            </div>
            <div class="mb-8">
                <h3 class="subheading text-xl font-semibold mb-4">A Message from Us</h3>
                <!-- Replace with your voice message file -->
                <audio controls class="mx-auto">
                    <source src="path/to/your/voice_message.mp3" type="audio/mpeg">
                    Your browser does not support the audio element.
                </audio>
            </div>
            <div class="bible-verse p-6 rounded-lg">
                <p class="text-xl font-bold text-gray-800">"She is clothed with strength and dignity; she can laugh at the days to come."</p>
                <p class="text-lg text-gray-600">Proverbs 31:26</p>
            </div>
        </div>
    </div>
    <script>
        function revealSurprise() {
            document.getElementById('mystery-box').classList.add('hidden');
            document.getElementById('surprise').classList.remove('hidden');
        }
    </script>
</body>
</html>
