Desde el fondo de mi corazón
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para El Amor de mi Vida 🩵</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #87CEEB, #B6E6FF);
            color: #333;
            min-height: 100vh;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            text-align: center;
        }
        
        .header {
            background: rgba(255, 255, 255, 0.95);
            padding: 40px;
            border-radius: 20px;
            margin-bottom: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }
        
        .main-title {
            font-size: 2.5em;
            color: #2c3e50;
            margin-bottom: 20px;
        }
        
        .personal-message {
            font-size: 1.3em;
            line-height: 1.6;
            margin-bottom: 30px;
            color: #2c3e50;
        }
        
        .counter-container {
            background: rgba(255, 255, 255, 0.9);
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .counter-title {
            font-size: 1.8em;
            color: #2c3e50;
            margin-bottom: 10px;
        }
        
        .counter-subtitle {
            font-size: 1.1em;
            color: #7f8c8d;
            margin-bottom: 20px;
            font-style: italic;
        }
        
        .time-counter {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
            margin: 20px 0;
        }
        
        .time-unit {
            background: linear-gradient(135deg, #4FC3F7, #81D4FA);
            color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(79, 195, 247, 0.3);
        }
        
        .time-number {
            font-size: 2.5em;
            font-weight: bold;
            display: block;
        }
        
        .time-label {
            font-size: 0.9em;
            opacity: 0.9;
        }
        
        .anniversary-date {
            background: #E3F2FD;
            padding: 15px;
            border-radius: 10px;
            margin: 15px 0;
            border: 2px dashed #4FC3F7;
            font-size: 1.1em;
        }
        
        .messages-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            margin: 30px 0;
        }
        
        .message-card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid #4FC3F7;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            text-align: left;
        }
        
        .reasons-section {
            background: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .reasons-list {
            text-align: left;
            display: inline-block;
            margin-top: 20px;
        }
        
        .reasons-list li {
            margin: 10px 0;
            font-size: 1.1em;
            line-height: 1.5;
        }
        
        .heart {
            color: #4FC3F7;
            font-size: 1.2em;
            margin: 0 5px;
        }
        
        /* NUBE DE PALABRAS */
        .wordcloud-section {
            background: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .wordcloud {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            margin: 25px 0;
            min-height: 200px;
            align-items: center;
        }
        
        .word {
            padding: 8px 16px;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s ease;
            background: #E3F2FD;
            border: 2px solid #4FC3F7;
        }
        
        .word:hover {
            transform: scale(1.1);
            background: #4FC3F7;
            color: white;
        }
        
        .word-size-1 { font-size: 1em; }
        .word-size-2 { font-size: 1.2em; }
        .word-size-3 { font-size: 1.4em; }
        .word-size-4 { font-size: 1.6em; }
        .word-size-5 { font-size: 1.8em; }
        
        /* MENSAJES SECRETOS */
        .secret-section {
            background: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .secret-container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin: 25px 0;
        }
        
        .secret-box {
            background: linear-gradient(135deg, #E3F2FD, #B3E5FC);
            padding: 25px 15px;
            border-radius: 12px;
            cursor: pointer;
            transition: all 0.3s ease;
            border: 2px solid #81D4FA;
            position: relative;
            overflow: hidden;
        }
        
        .secret-box:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(79, 195, 247, 0.3);
        }
        
        .secret-question {
            font-size: 2em;
            margin-bottom: 10px;
        }
        
        .secret-message {
            font-size: 0.9em;
            opacity: 0;
            max-height: 0;
            transition: all 0.5s ease;
            color: #1565C0;
            font-weight: 500;
        }
        
        .secret-box.active .secret-message {
            opacity: 1;
            max-height: 100px;
            margin-top: 10px;
        }
        
        .secret-box.active {
            background: linear-gradient(135deg, #B3E5FC, #81D4FA);
        }

        /* CARTA DE AMOR */
        .letter-section {
            background: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            position: relative;
        }
        
        .letter-envelope {
            background: linear-gradient(135deg, #E3F2FD, #B3E5FC);
            padding: 30px;
            border-radius: 10px;
            border: 2px solid #4FC3F7;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .letter-envelope:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(79, 195, 247, 0.4);
        }
        
        .letter-envelope h3 {
            margin: 0;
            color: #1565C0;
            font-size: 1.5em;
        }
        
        .letter-content {
            max-height: 0;
            opacity: 0;
            overflow: hidden;
            transition: all 0.8s ease;
            text-align: left;
            line-height: 1.8;
            padding: 0 20px;
            background: #fafafa;
            border-radius: 10px;
            margin-top: 0;
        }
        
        .letter-content.open {
            max-height: 2000px;
            opacity: 1;
            padding: 30px 20px;
            margin-top: 20px;
            overflow-y: auto;
        }
        
        .letter-text {
            font-size: 1.1em;
            color: #333;
            white-space: pre-line;
        }
        
        .letter-signature {
            text-align: right;
            font-style: italic;
            margin-top: 20px;
            color: #4FC3F7;
            font-weight: bold;
        }

        /* NUEVO: LIBRO INTERACTIVO */
        .book-section {
            background: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .book-container {
            background: #f5f5f5;
            padding: 25px;
            border-radius: 10px;
            border: 2px solid #4FC3F7;
            margin: 20px 0;
            min-height: 400px;
            position: relative;
        }
        
        .book-page {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            min-height: 350px;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        
        .book-cover {
            background: linear-gradient(135deg, #4FC3F7, #81D4FA);
            color: white;
            padding: 40px;
            border-radius: 10px;
            text-align: center;
        }
        
        .book-title {
            font-size: 2.5em;
            margin-bottom: 20px;
            font-weight: bold;
        }
        
        .book-subtitle {
            font-size: 1.2em;
            opacity: 0.9;
        }
        
        .dedication {
            text-align: center;
            font-style: italic;
            line-height: 1.8;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .book-controls {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }
        
        .book-btn {
            background: linear-gradient(135deg, #4FC3F7, #81D4FA);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 1em;
            transition: all 0.3s ease;
        }
        
        .book-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 10px rgba(79, 195, 247, 0.3);
        }
        
        .book-btn:disabled {
            background: #cccccc;
            cursor: not-allowed;
            transform: none;
            box-shadow: none;
        }
        
        .page-number {
            font-weight: bold;
            color: #4FC3F7;
            margin: 0 15px;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
        
        .floating-hearts {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .floating-heart {
            position: absolute;
            font-size: 24px;
            opacity: 0.4;
            animation: float 6s infinite linear;
        }
        
        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
            }
        }
        
        .section-title {
            font-size: 2em;
            color: #2c3e50;
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <!-- Corazones flotantes de fondo -->
    <div class="floating-hearts" id="heartsContainer"></div>
    
    <div class="container">
        <div class="header">
            <!-- TÍTULO PRINCIPAL -->
            <h1 class="main-title">Para África 🩵</h1>
            
            <!-- MENSAJE PERSONAL -->
            <div class="personal-message">
                Esto es para ti, así puedes ver siempre cuánto te amo y que eres lo mejor en mi vida.
            </div>
            
            <!-- CONTADOR DE TIEMPO -->
            <div class="counter-container">
                <h2 class="counter-title">Nuestro Tiempo Juntos</h2>
                <p class="counter-subtitle">Este tiempo llevas aguantándome y lo que te queda</p>
                
                <div class="anniversary-date">
                    <p>Desde aquel día especial: <strong>9 de Febrero</strong></p>
                </div>
                
                <div class="time-counter">
                    <div class="time-unit">
                        <span class="time-number" id="days">0</span>
                        <span class="time-label">Días</span>
                    </div>
                    <div class="time-unit">
                        <span class="time-number" id="hours">0</span>
                        <span class="time-label">Horas</span>
                    </div>
                    <div class="time-unit">
                        <span class="time-number" id="minutes">0</span>
                        <span class="time-label">Minutos</span>
                    </div>
                    <div class="time-unit">
                        <span class="time-number" id="seconds">0</span>
                        <span class="time-label">Segundos</span>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- 1. MENSAJES PARA TI (PRIMERO) -->
        <div class="messages-section">
            <h2 class="section-title">Mensajes para Ti 🩵</h2>
            <div class="messages-grid">
                <div class="message-card">
                    "Eres mi primer y último pensamiento en el día"
                </div>
                <div class="message-card">
                    "Contigo todo es más bonito"
                </div>
                <div class="message-card">
                    "Mi corazón se pone feliz cada vez que te veo"
                </div>
                <div class="message-card">
                    "Me encanta verte feliz"
                </div>
                <div class="message-card">
                    "Quiero que estes en mi vida por mucho mucho tiempo"
                </div>
                <div class="message-card">
                    "Eres la mujer más bella y hermosa de este universo"
                </div>
            </div>
        </div>
        
        <!-- 2. RAZONES POR LAS QUE TE AMO (SEGUNDO) -->
        <div class="reasons-section">
            <h2 class="section-title">Razones por las que Te Amo 🩵</h2>
            <ul class="reasons-list">
                <li><span class="heart">🩵</span> Por ti, por ser la mujer con la que quiero algo bonito</li>
                <li><span class="heart">🩵</span> Por tu forma de ser tan especial</li>
                <li><span class="heart">🩵</span> Por hacerme feliz cada vez que me das un beso</li>
                <li><span class="heart">🩵</span> Por aguantar mis tonterias</li>
                <li><span class="heart">🩵</span> Por la forma en que me conoces</li>
                <li><span class="heart">🩵</span> Por hacer que cada vez que salgamos sea un bonito recuerdo</li>
                <li><span class="heart">🩵</span> Por ser tan tan tan bonita y tener unos ojos que me hipnotizan</li>
                <li><span class="heart">🩵</span> Por ser mi mejor amiga (mi única amiga) y mi amor a la vez</li>
            </ul>
        </div>
        
        <!-- 3. NUBE DE AMOR (TERCERO) -->
        <div class="wordcloud-section">
            <h2 class="section-title">Nuestra Nube de Amor 🩵</h2>
            <p>Palabras que definen lo que somos</p>
            <div class="wordcloud" id="wordcloud">
                <!-- Las palabras se generan con JavaScript -->
            </div>
        </div>
        
        <!-- 4. MENSAJES SECRETOS (ÚLTIMO) -->
        <div class="secret-section">
            <h2 class="section-title">Mensajes Secretos 🩵</h2>
            <p>¡Toca las cajas para descubrir mensajes especiales!</p>
            <div class="secret-container">
                <div class="secret-box" onclick="toggleSecret(this)">
                    <div class="secret-question">✨</div>
                    <div class="secret-message">Un beso tuyo me da vida</div>
                </div>
                <div class="secret-box" onclick="toggleSecret(this)">
                    <div class="secret-question">💫</div>
                    <div class="secret-message">Tu ojos son mis favoritos en el mundo</div>
                </div>
                <div class="secret-box" onclick="toggleSecret(this)">
                    <div class="secret-question">🌟</div>
                    <div class="secret-message">Contigo quiero vivir muchas experiencias</div>
                </div>
                <div class="secret-box" onclick="toggleSecret(this)">
                    <div class="secret-question">🎀</div>
                    <div class="secret-message">Eres el mejor regalo que la vida me dio</div>
                </div>
                <div class="secret-box" onclick="toggleSecret(this)">
                    <div class="secret-question">🦋</div>
                    <div class="secret-message">Me haces sentir que todo es bonito</div>
                </div>
                <div class="secret-box" onclick="toggleSecret(this)">
                    <div class="secret-question">🌙</div>
                    <div class="secret-message">Te amo más cada dia</div>
                </div>
            </div>
        </div>

        <!-- 5. CARTA DE AMOR -->
        <div class="letter-section">
            <h2 class="section-title">Mi Carta para Ti 🩵</h2>
            <div class="letter-envelope" onclick="toggleLetter()">
                <h3>💌 Toca aquí para abrir mi carta</h3>
                <p>Desde el fondo de mi corazón...</p>
            </div>
            <div class="letter-content" id="letterContent">
                <div class="letter-text">
África,

No sabría como empezar esta carta, creo que todo lo que te pueda decir siempre va a demostrar todo el amor que te tengo, pero dicen que las palabras llegan al corazón, por eso quiero dedicarte algunas, que espero te gusten.

No puedes llegar a imaginarte lo que significas para mí, veía imposible poder estar contigo, poder conocerte más, por eso ahora quiero cuidarte y darte mucho amor para que nunca te vayas de mi lado. Es que lo veía como un sueño el día que me dijiste que si, no me lo creía, pero mira ahora, sigue siendo un sueño y espero no despertar nunca para seguir contigo.

Cada día pienso y me pregunto, ¿realmente merezco estar con ella?, porque eres una gran mujer y persona, hermosa por fuera y dentro, y yo siento que te merecerías mucho más, porque si yo sé que no soy el mejor, tampoco el más guapo ni nada de eso, muchas veces te hago enfadar y más cosas, en cambio tú, no tienes nada malo, eres una obra de arte, muy bella, tienes una carita perfecta y sobretodo unos ojos muy muy muy lindos y que decir de tu personalidad, única e inigualable, por eso me empezaste a gustar, me llamaba la atención tu forma de ser, resaltabas ante lás demás y lo sigues haciendo. Y ves, tu eres perfecta para mí, en cambio yo no, pero bueno yo solo quiero que tu seas feliz siempre e intentaré que sea así. No quiero que te canses de mí nunca, sería muy feito eso, y aunque no lo demuestre, me pongo muy mal siempre que nos enfadamos, no me gusta demostrarlo, pero es así, pero sabes que, eso se me pasa con solo ver un te amo tuyo, es como que me da vida, me da ánimos. Tengo miedo de perderte, espero nunca pase eso, quiero que nunca pase. porque enserio, no veo mís dias sin hablarte, sin decirte tonterías, sin picarte, sin decirte te amo, sin decirte porque cuando te pregunto si me amas, ves eres todo de mí, eres la pieza que encaja perfecta conmigo, eres mi persona ideal, mi persona favorita y el amor de mi vida. Eres la reina de mi corazón, por ti está feliz siempre, así que sigue haciendome feliz vale?, por mucho tiempo.

En mis días, estás presente siempre, me despierto y pienso en ti, estoy en el autobús yendo al instituto y pienso en ti, estoy en clases y pienso en ti, África pienso en ti cada segundo de mi vida, no se que me has hecho, nunca había estado así, tan enamorado, pero me encanta porque eres tú. Eres la primera persona de la cual me enamoro realmente, así que se podría decir que eres mi primer amor y si lo eres, yo digo que lo eres, y serás el primero y único gran amor de toda mi vida, porque quiero contigo una vida, y me la pela que tengamos poco tiempo de estar juntos, yo quiero que me acompañes toda mi vida.

Y te lo repito , me encanta como eres, cada parte de ti, tu forma de reír, tu manera de mirarme, tu forma de entenderme, todo toditito de ti, por eso prometo amarte cada día mucho más, apoyarte en todo y ser tu refugio cuando lo necesites, quiero tener una vida llena de momentos bonitos contigo, llena de risas, experiencias y amor.

Siempre serás mi mejor amiga, mi confidente y el amor de mi vida. No puedo imaginar un futuro sin ti.

Con todo mi amor,
                </div>
                <div class="letter-signature">
                    Te amo infinitamente más que infinitamente infinito🩵
                </div>
            </div>
        </div>

        <!-- 6. NUEVO: LIBRO INTERACTIVO -->
        <div class="book-section">
            <h2 class="section-title">Nuestro Libro del Amor 📖</h2>
            <p>La historia de nuestro amor página a página</p>
            
            <div class="book-container">
                <div class="book-page" id="bookPage">
                    <!-- El contenido del libro se actualiza aquí -->
                </div>
                
                <div class="book-controls">
                    <button class="book-btn" onclick="previousPage()" id="prevBtn">← Página Anterior</button>
                    <span class="page-number">Página <span id="currentPage">1</span> de <span id="totalPages">2</span></span>
                    <button class="book-btn" onclick="nextPage()" id="nextBtn">Página Siguiente →</button>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Fecha de inicio de la relación - 9 de febrero de 2025
        const startDate = new Date('2025-02-09T00:00:00');
        
        function updateCounter() {
            const now = new Date();
            const diff = now - startDate;
            
            // Cálculos del tiempo
            const seconds = Math.floor(diff / 1000);
            const minutes = Math.floor(seconds / 60);
            const hours = Math.floor(minutes / 60);
            const days = Math.floor(hours / 24);
            
            // Actualizar los displays
            document.getElementById('days').textContent = days;
            document.getElementById('hours').textContent = hours % 24;
            document.getElementById('minutes').textContent = minutes % 60;
            document.getElementById('seconds').textContent = seconds % 60;
        }
        
        // FUNCIÓN: Mensajes secretos
        function toggleSecret(element) {
            element.classList.toggle('active');
        }

        // FUNCIÓN: Carta de amor
        function toggleLetter() {
            const letterContent = document.getElementById('letterContent');
            letterContent.classList.toggle('open');
        }
        
        // FUNCIÓN: Nube de palabras CON TUS PALABRAS
        function createWordCloud() {
            const words = [
                {text: "Amor", size: 5},
                {text: "Abrazos", size: 4},
                {text: "Besos", size: 4},
                {text: "Confianza", size: 4},
                {text: "Felicidad", size: 5},
                {text: "Diversión", size: 3},
                {text: "Picarnos", size: 3},
                {text: "Compañía", size: 4},
                {text: "Química", size: 3},
                {text: "Encanto", size: 3},
                {text: "Recuerdos", size: 4},
                {text: "Tranquilidad", size: 3},
                {text: "Honestidad", size: 3},
                {text: "Infinito", size: 4},
                {text: "Conexión", size: 4}
            ];
            
            const wordcloud = document.getElementById('wordcloud');
            
            // Mezclar palabras para orden aleatorio
            words.sort(() => Math.random() - 0.5);
            
            words.forEach(word => {
                const wordElement = document.createElement('div');
                wordElement.className = `word word-size-${word.size}`;
                wordElement.textContent = word.text;
                wordElement.onclick = function() {
                    this.style.background = '#4FC3F7';
                    this.style.color = 'white';
                    setTimeout(() => {
                        this.style.background = '#E3F2FD';
                        this.style.color = '#333';
                    }, 1000);
                };
                wordcloud.appendChild(wordElement);
            });
        }
        
        // NUEVO: LIBRO INTERACTIVO (SOLO PORTADA Y PRIMERA PÁGINA)
        const bookPages = [
            {
                type: "cover",
                content: `
                    <div class="book-cover">
                        <div class="book-title">Un amor infinito</div>
                        <div class="book-subtitle">Para África</div>
                    </div>
                `
            },
            {
                type: "dedication",
                content: `
                    <div class="dedication">
                        <p>Nunca se sabe cuando puedes amar tanto a alguien, en mi caso, no pensaba que llegaría a amarte de esta manera.</p>
                        <br>
                        <p>Nunca se sabe cuánto es lo que puedes llegar a amar a alguien, en mi caso, tampoco quisiera saberlo, porque así mi amor por ti no tendría un límite</p>
                        <br>
                        <p>Muchas veces cuesta expresar los sentimientos, en mi caso, tengo un sentimiento tan profundo y especial, que hasta me faltarían palabras para describirlo.</p>
                        <br>
                        <p>En un libro puedo expresar e ir, con el tiempo, contando nuestra historia, que espero nunca tenga un final. A lo mejor pensarás que no es un gran detalle o que es muy repentino o anticipado, pero solamente quiero expresar mis sentimientos y que puedas tener un espacio bonito para ti.</p>
                        <br>
                        <p>Espero te guste, mi amor.</p>
                    </div>
                `
            }
        ];

        let currentPage = 0;

        function updateBook() {
            const page = bookPages[currentPage];
            document.getElementById('bookPage').innerHTML = page.content;
            
            document.getElementById('currentPage').textContent = currentPage + 1;
            document.getElementById('totalPages').textContent = bookPages.length;
            
            document.getElementById('prevBtn').disabled = currentPage === 0;
            document.getElementById('nextBtn').disabled = currentPage === bookPages.length - 1;
        }

        function nextPage() {
            if (currentPage < bookPages.length - 1) {
                currentPage++;
                updateBook();
            }
        }

        function previousPage() {
            if (currentPage > 0) {
                currentPage--;
                updateBook();
            }
        }
        
        // Crear corazones flotantes
        function createHearts() {
            const heartsContainer = document.getElementById('heartsContainer');
            const hearts = ['🩵', '💙', '🩵', '💙', '🩵', '💙'];
            
            for (let i = 0; i < 15; i++) {
                const heart = document.createElement('div');
                heart.className = 'floating-heart';
                heart.textContent = hearts[Math.floor(Math.random() * hearts.length)];
                heart.style.left = Math.random() * 100 + 'vw';
                heart.style.animationDelay = Math.random() * 6 + 's';
                heart.style.fontSize = (Math.random() * 20 + 20) + 'px';
                heartsContainer.appendChild(heart);
            }
        }
        
        // Efectos especiales al cargar
        document.addEventListener('DOMContentLoaded', function() {
            // Iniciar contador
            updateCounter();
            setInterval(updateCounter, 1000);
            
            // Crear corazones flotantes
            createHearts();
            
            // Crear nube de palabras
            createWordCloud();
            
            // Inicializar libro
            updateBook();
            
            // Efecto de aparición suave
            const elements = document.querySelectorAll('.header, .messages-section, .reasons-section, .wordcloud-section, .secret-section, .letter-section, .book-section');
            elements.forEach((element, index) => {
                element.style.opacity = '0';
                element.style.transform = 'translateY(20px)';
                setTimeout(() => {
                    element.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
                    element.style.opacity = '1';
                    element.style.transform = 'translateY(0)';
                }, index * 200);
            });
        });
    </script>
</body>
</html>
