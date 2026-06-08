# PP72034
Testing
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ASESMEN SUMATIF PP 7 GENAP 2025/2026</title>
    <style>
        /* Google Forms Design System Tokens */
        :root {
            --bg-color: #f3eefc;
            --primary-color: #673ab7;
            --primary-dark: #512da8;
            --text-color: #202124;
            --text-secondary: #70757a;
            --text-error: #d93025;
            --card-bg: #ffffff;
            --border-color: #dadce0;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Roboto', 'Google Sans', Arial, sans-serif;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            display: flex;
            justify-content: center;
            padding: 12px 10px 36px 10px;
            font-size: 14px;
            line-height: 1.5;
        }

        .container {
            width: 100%;
            max-width: 640px;
        }

        /* Forms Card Layout */
        .card {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 8px;
            margin-bottom: 12px;
            padding: 24px;
            position: relative;
            word-wrap: break-word;
        }

        /* Header Card specific styling */
        .card.header-card {
            border-top: 10px solid var(--primary-color);
            padding-top: 16px;
        }

        .card.question-header {
            background-color: var(--primary-color);
            color: white;
            padding: 12px 16px;
            font-size: 14px;
            font-weight: 500;
            border-radius: 4px;
            margin-bottom: 12px;
            border: none;
            letter-spacing: 0.8px;
        }

        h1 {
            font-size: 24px;
            font-weight: 400;
            line-height: 1.35;
            margin-bottom: 12px;
            color: var(--text-color);
        }

        .meta-info {
            font-size: 13px;
            color: var(--text-color);
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 12px;
            margin-bottom: 12px;
        }

        .meta-line {
            display: flex;
            align-items: center;
            margin-bottom: 6px;
        }

        .meta-email {
            font-weight: normal;
        }

        .meta-link {
            color: #1a73e8;
            text-decoration: none;
            margin-left: 8px;
            font-size: 13px;
        }

        .meta-icon-text {
            color: var(--text-secondary);
            display: flex;
            align-items: center;
            gap: 6px;
            font-size: 12px;
            margin-top: 8px;
        }

        .required-notice {
            color: var(--text-error);
            font-size: 12px;
            margin-top: 12px;
        }

        /* Form Inputs */
        .form-group {
            margin-bottom: 4px;
        }

        .label {
            font-size: 15px;
            font-weight: 400;
            color: var(--text-color);
            margin-bottom: 16px;
            display: block;
        }

        .label .required-star {
            color: var(--text-error);
            margin-left: 3px;
        }

        .input-underline-container {
            position: relative;
            margin-top: 12px;
            width: 100%;
        }

        .input-underline {
            width: 100%;
            border: none;
            border-bottom: 1px solid #c4c7c5;
            padding: 6px 0;
            font-size: 14px;
            outline: none;
            background: transparent;
            color: var(--text-color);
            transition: border-bottom-color 0.2s;
        }

        .input-underline:focus {
            border-bottom: 2px solid var(--primary-color);
            padding-bottom: 5px;
        }

        /* Radio Options */
        .radio-group {
            display: flex;
            flex-direction: column;
            gap: 16px;
            margin-top: 16px;
        }

        .radio-option {
            display: flex;
            align-items: flex-start;
            cursor: pointer;
            position: relative;
        }

        .radio-option input[type="radio"] {
            position: absolute;
            opacity: 0;
            width: 0;
            height: 0;
        }

        .radio-checkmark {
            width: 20px;
            height: 20px;
            border: 2px solid #5f6368;
            border-radius: 50%;
            margin-right: 12px;
            display: inline-block;
            flex-shrink: 0;
            position: relative;
            transition: border-color 0.2s;
            margin-top: 1px;
        }

        .radio-option input[type="radio"]:checked + .radio-checkmark {
            border-color: var(--primary-color);
        }

        .radio-option input[type="radio"]:checked + .radio-checkmark::after {
            content: "";
            position: absolute;
            width: 10px;
            height: 10px;
            top: 3px;
            left: 3px;
            border-radius: 50%;
            background-color: var(--primary-color);
        }

        .radio-text {
            font-size: 14px;
            color: var(--text-color);
            line-height: 1.4;
        }

        .points-badge {
            position: absolute;
            right: 24px;
            top: 24px;
            font-size: 12px;
            color: var(--text-secondary);
        }

        /* Navigation Buttons */
        .navigation-panel {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 16px;
            padding: 0 4px;
        }

        .nav-buttons-left {
            display: flex;
            gap: 8px;
        }

        .btn {
            border: none;
            border-radius: 4px;
            font-size: 14px;
            font-weight: 500;
            padding: 0 16px;
            height: 36px;
            cursor: pointer;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            transition: background-color 0.2s;
        }

        .btn-primary {
            background-color: var(--primary-color);
            color: white;
        }

        .btn-primary:hover, .btn-primary:focus {
            background-color: var(--primary-dark);
        }

        .btn-text {
            background-color: transparent;
            color: var(--primary-color);
        }

        .btn-text:hover, .btn-text:focus {
            background-color: rgba(103, 58, 183, 0.04);
        }

        .btn-clear {
            background-color: transparent;
            color: var(--primary-color);
            border: none;
            font-size: 14px;
            cursor: pointer;
            padding: 8px;
        }

        /* Error Messages */
        .error-message {
            color: var(--text-error);
            font-size: 12px;
            margin-top: 8px;
            display: none;
            align-items: center;
            gap: 8px;
        }

        /* Views State Management */
        .page-view {
            display: none;
        }

        .page-view.active {
            display: block;
        }

        /* Footer Info */
        .footer-info {
            text-align: center;
            color: var(--text-secondary);
            font-size: 11px;
            margin-top: 24px;
            line-height: 1.6;
        }

        .footer-info a {
            color: var(--text-secondary);
            text-decoration: underline;
        }

        .google-logo {
            font-family: Arial, sans-serif;
            font-size: 18px;
            font-weight: 500;
            margin-top: 16px;
            color: #5f6368;
            letter-spacing: -0.5px;
        }
        
        /* Result Page Box */
        .score-container {
            text-align: center;
            padding: 12px 0;
        }

        .score-headline {
            font-size: 20px;
            color: var(--primary-color);
            margin-bottom: 8px;
            font-weight: 500;
        }

        .score-badge {
            font-size: 42px;
            font-weight: bold;
            color: var(--text-color);
            margin: 12px 0;
        }

        /* SVG Icons */
        .icon {
            width: 16px;
            height: 16px;
            fill: currentColor;
            display: inline-block;
            vertical-align: middle;
        }
        .icon-error {
            fill: var(--text-error);
        }
    </style>
</head>
<body>

    <div class="container">
        <form id="googleForm" onsubmit="return false;">
            
            <div id="page1" class="page-view active">
                <div class="card header-card">
                    <h1>ASESMEN SUMATIF PP 7 GENAP 2025/2026</h1>
                    <div class="meta-info">
                        <div class="meta-line">
                            <span class="meta-email">roridimas29@gmail.com</span>
                            <a href="#" class="meta-link" onclick="alert('Simulasi ganti akun'); return false;">Ganti akun</a>
                        </div>
                        <div class="meta-icon-text">
                            <svg class="icon" viewBox="0 0 24 24"><path d="M18 11.5c.83 0 1.5-.67 1.5-1.5s-.67-1.5-1.5-1.5-1.5.67-1.5 1.5.67 1.5 1.5 1.5zm-6 0c.83 0 1.5-.67 1.5-1.5s-.67-1.5-1.5-1.5-1.5.67-1.5 1.5.67 1.5 1.5 1.5zm-6 0c.83 0 1.5-.67 1.5-1.5S6.83 8.5 6 8.5 4.5 9.17 4.5 10s.67 1.5 1.5 1.5zm6 4c-2.33 0-4.22 1.39-5 3.33h10c-.78-1.94-2.67-3.33-5-3.33zM12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-3.31 0-6-2.69-6-6 0-1.01.25-1.97.7-2.8l1.46 1.46c-.1.41-.16.84-.16 1.34 0 2.21 1.79 4 4 4s4-1.79 4-4c0-.5-.06-.93-.16-1.34l1.46-1.46c.45.83.7 1.79.7 2.8 0 3.31-2.69 6-6 6z"/></svg>
                            Tidak dibagikan
                        </div>
                    </div>
                    <div class="required-notice">* Menunjukkan pertanyaan yang wajib diisi</div>
                </div>

                <div class="card">
                    <div class="form-group">
                        <label class="label">NAMA<span class="required-star">*</span></label>
                        <div class="input-underline-container">
                            <input type="text" id="input_nama" class="input-underline" placeholder="Jawaban Anda" required>
                        </div>
                        <div class="error-message" id="error_nama">
                            <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                            Pertanyaan ini wajib diisi
                        </div>
                    </div>
                </div>

                <div class="card">
                    <div class="form-group">
                        <label class="label">KELAS<span class="required-star">*</span></label>
                        <div class="input-underline-container">
                            <input type="text" id="input_kelas" class="input-underline" placeholder="Jawaban Anda" required>
                        </div>
                        <div class="error-message" id="error_kelas">
                            <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                            Pertanyaan ini wajib diisi
                        </div>
                    </div>
                </div>

                <div class="card">
                    <div class="form-group">
                        <label class="label">NOMOR UJIAN<span class="required-star">*</span></label>
                        <div class="input-underline-container">
                            <input type="text" id="input_nomor" class="input-underline" placeholder="Jawaban Anda" required>
                        </div>
                        <div class="error-message" id="error_nomor">
                            <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                            Pertanyaan ini wajib diisi
                        </div>
                    </div>
                </div>

                <div class="card">
                    <div class="form-group">
                        <label class="label">MATA PELAJARAN<span class="required-star">*</span></label>
                        <div class="input-underline-container">
                            <input type="text" id="input_mapel" class="input-underline" placeholder="Jawaban Anda" required>
                        </div>
                        <div class="error-message" id="error_mapel">
                            <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                            Pertanyaan ini wajib diisi
                        </div>
                    </div>
                </div>

                <div class="card">
                    <div class="form-group">
                        <label class="label">TOKEN<span class="required-star">*</span></label>
                        <div class="input-underline-container">
                            <input type="text" id="input_token" class="input-underline" placeholder="Jawaban Anda" required>
                        </div>
                        <div class="error-message" id="error_token">
                            <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                            Token salah atau tidak sesuai!
                        </div>
                    </div>
                </div>

                <div class="navigation-panel">
                    <div class="nav-buttons-left">
                        <button type="button" class="btn btn-primary" onclick="validatePage1()">Berikutnya</button>
                    </div>
                    <button type="button" class="btn-clear" onclick="clearForm()">Kosongkan formulir</button>
                </div>
            </div>


            <div id="page2" class="page-view">
                <div class="card question-header">SOAL NO 1</div>
                
                <div class="card">
                    <div class="points-badge">2 poin</div>
                    <label class="label">Bahlil adalah pemerintah asal Indonesia yang kebanyakan:<span class="required-star">*</span></label>
                    
                    <div class="radio-group">
                        <label class="radio-option">
                            <input type="radio" name="soal1" value="A">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">A. nyocot</span>
                        </label>
                        <label class="radio-option">
                            <input type="radio" name="soal1" value="B">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">B. nya wit</span>
                        </label>
                        <label class="radio-option">
                            <input type="radio" name="soal1" value="C">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">C. MAS BAHLIL GANTENG (MBG)</span>
                        </label>
                    </div>
                    <div class="error-message" id="error_soal1">
                        <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                        Pertanyaan ini wajib diisi
                    </div>
                </div>

                <div class="navigation-panel">
                    <div class="nav-buttons-left">
                        <button type="button" class="btn btn-text" onclick="goToPage(1)">Kembali</button>
                        <button type="button" class="btn btn-primary" onclick="validateQuestionPage(2, 'soal1')">Berikutnya</button>
                    </div>
                    <button type="button" class="btn-clear" onclick="clearForm()">Kosongkan formulir</button>
                </div>
            </div>


            <div id="page3" class="page-view">
                <div class="card question-header">SOAL NO 2</div>
                
                <div class="card">
                    <div class="points-badge">2 poin</div>
                    <label class="label">seorang presiden bernama jokowi dodo sering menyebutkan kata Wiwok detok not onli tok detok, kata lanjutan yang benar adalah:<span class="required-star">*</span></label>
                    
                    <div class="radio-group">
                        <label class="radio-option">
                            <input type="radio" name="soal2" value="A">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">A. DI HINA-HINA SAYA JUGA DIAM DI MAKI MAKI SAYA JUGA DIAM NAMUN HARI INI SAYA AKAN LAWAN!</span>
                        </label>
                        <label class="radio-option">
                            <input type="radio" name="soal2" value="B">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">B. WONG SAYA ORANG SOLO TOH?</span>
                        </label>
                        <label class="radio-option">
                            <input type="radio" name="soal2" value="C">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">C. OH KAGET!</span>
                        </label>
                    </div>
                    <div class="error-message" id="error_soal2">
                        <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                        Pertanyaan ini wajib diisi
                    </div>
                </div>

                <div class="navigation-panel">
                    <div class="nav-buttons-left">
                        <button type="button" class="btn btn-text" onclick="goToPage(2)">Kembali</button>
                        <button type="button" class="btn btn-primary" onclick="validateQuestionPage(3, 'soal2')">Berikutnya</button>
                    </div>
                    <button type="button" class="btn-clear" onclick="clearForm()">Kosongkan formulir</button>
                </div>
            </div>


            <div id="page4" class="page-view">
                <div class="card question-header">SOAL NO 3</div>
                
                <div class="card">
                    <div class="points-badge">2 poin</div>
                    <label class="label">seorang anak bernama joko menyukai wanita di kelasnya namun wanita tersebut memilih laki-laki lain. Kata yang pantas untuk joko adalah:<span class="required-star">*</span></label>
                    
                    <div class="radio-group">
                        <label class="radio-option">
                            <input type="radio" name="soal3" value="A">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">A. BADAN KAYA BIAWAK MAU SPEK DEWI MIMPI REK 😹</span>
                        </label>
                        <label class="radio-option">
                            <input type="radio" name="soal3" value="B">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">B. mengejar cinta yang bukan miliknya lebih baik menjauh darinya</span>
                        </label>
                        <label class="radio-option">
                            <input type="radio" name="soal3" value="C">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">C. MY kisah mu my kisah ku</span>
                        </label>
                    </div>
                    <div class="error-message" id="error_soal3">
                        <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                        Pertanyaan ini wajib diisi
                    </div>
                </div>

                <div class="navigation-panel">
                    <div class="nav-buttons-left">
                        <button type="button" class="btn btn-text" onclick="goToPage(3)">Kembali</button>
                        <button type="button" class="btn btn-primary" onclick="validateQuestionPage(4, 'soal3')">Berikutnya</button>
                    </div>
                    <button type="button" class="btn-clear" onclick="clearForm()">Kosongkan formulir</button>
                </div>
            </div>


            <div id="page5" class="page-view">
                <div class="card question-header">SOAL NO 4</div>
                
                <div class="card">
                    <div class="points-badge">2 poin</div>
                    <label class="label">Dalam BPUPKI ada Panitia Sembilan yang merumuskan Pancasila. Hikmah yang dapat diambil adalah:<span class="required-star">*</span></label>
                    
                    <div class="radio-group">
                        <label class="radio-option">
                            <input type="radio" name="soal4" value="A">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">A. jangan jadi panitia sembilan</span>
                        </label>
                        <label class="radio-option">
                            <input type="radio" name="soal4" value="B">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">B. kejar kerja kerasmu dan nikmati hasilnya</span>
                        </label>
                        <label class="radio-option">
                            <input type="radio" name="soal4" value="C">
                            <span class="radio-checkmark"></span>
                            <span class="radio-text">C. soekarno</span>
                        </label>
                    </div>
                    <div class="error-message" id="error_soal4">
                        <svg class="icon icon-error" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></svg>
                        Pertanyaan ini wajib diisi
                    </div>
                </div>

                <div class="navigation-panel">
                    <div class="nav-buttons-left">
                        <button type="button" class="btn btn-text" onclick="goToPage(4)">Kembali</button>
                        <button type="button" class="btn btn-primary" onclick="submitForm()">Kirim</button>
                    </div>
                    <button type="button" class="btn-clear" onclick="clearForm()">Kosongkan formulir</button>
                </div>
            </div>


            <div id="pageResult" class="page-view">
                <div class="card header-card">
                    <h1>ASESMEN SUMATIF PP 7 GENAP 2025/2026</h1>
                    <div style="margin-top: 16px; font-size: 14px;">
                        Tanggapan Anda telah direkam.
                    </div>
                </div>

                <div class="card">
                    <div class="score-container">
                        <div class="score-headline">Skor Anda:</div>
                        <div class="score-badge" id="scoreDisplay">0 / 8</div>
                        <button type="button" class="btn btn-primary" style="margin-top:8px;" onclick="restartForm()">Isi kembali formulir</button>
                    </div>
                </div>
            </div>

        </form>

        <div class="footer-info">
            Konten ini tidak dibuat atau didukung oleh Google. <a href="#" onclick="return false;">Laporkan Penyalahgunaan</a> - <a href="#" onclick="return false;">Persyaratan Layanan</a> - <a href="#" onclick="return false;">Kebijakan Privasi</a>
            <div class="google-logo">Google Formulir</div>
        </div>
    </div>

    <script>
        const TOKEN_BENAR = "PP 7 2034";
        
        // Kunci Jawaban & Bobot Nilai
        const kunciJawaban = {
            soal1: { answer: "C", score: 2 },
            soal2: { answer: "A", score: 2 },
            soal3: { answer: "A", score: 2 },
            soal4: { answer: "B", score: 2 }
        };

        function goToPage(pageNum) {
            // Sembunyikan semua halaman form
            document.querySelectorAll('.page-view').forEach(p => p.classList.remove('active'));
            
            // Tampilkan halaman yang dituju
            if(pageNum === 'Result') {
                document.getElementById('pageResult').classList.add('active');
            } else {
                document.getElementById('page' + pageNum).classList.add('active');
            }
            window.scrollTo(0, 0);
        }

        function validatePage1() {
            let isValid = true;
            const fields = ['nama', 'kelas', 'nomor', 'mapel'];
            
            // Cek kelengkapan biodata teks
            fields.forEach(f => {
                const input = document.getElementById('input_' + f);
                const error = document.getElementById('error_' + f);
                if (!input.value.trim()) {
                    error.style.display = 'flex';
                    isValid = false;
                } else {
                    error.style.display = 'none';
                }
            });

            // Cek kesesuaian Token
            const tokenInput = document.getElementById('input_token');
            const tokenError = document.getElementById('error_token');
            if (tokenInput.value.trim() !== TOKEN_BENAR) {
                tokenError.style.display = 'flex';
                isValid = false;
            } else {
                tokenError.style.display = 'none';
            }

            if (isValid) {
                goToPage(2);
            }
        }

        function validateQuestionPage(currentPageNum, radioName) {
            const selected = document.querySelector(`input[name="${radioName}"]:checked`);
            const errorBox = document.getElementById('error_' + radioName);
            
            if (!selected) {
                errorBox.style.display = 'flex';
            } else {
                errorBox.style.display = 'none';
                goToPage(currentPageNum + 1);
            }
        }

        function submitForm() {
            // Validasi soal terakhir
            const selected = document.querySelector('input[name="soal4"]:checked');
            const errorBox = document.getElementById('error_soal4');
            
            if (!selected) {
                errorBox.style.display = 'flex';
                return;
            } else {
                errorBox.style.display = 'none';
            }

            // Proses Penghitungan Nilai Akhir
            let totalNilai = 0;
            for (let key in kunciJawaban) {
                const userAns = document.querySelector(`input[name="${key}"]:checked`);
                if (userAns && userAns.value === kunciJawaban[key].answer) {
                    totalNilai += kunciJawaban[key].score;
                }
            }

            // Aturan Rentang Skor: Maksimum 8, Minimum 2
            if (totalNilai < 2) {
                totalNilai = 2;
            }
            if (totalNilai > 8) {
                totalNilai = 8;
            }

            // Tampilkan hasil akhir ke layar
            document.getElementById('scoreDisplay').innerText = totalNilai + " / 8";
            goToPage('Result');
        }

        function clearForm() {
            if (confirm("Apakah Anda yakin ingin menghapus semua jawaban?")) {
                document.getElementById('googleForm').reset();
                document.querySelectorAll('.error-message').forEach(err => err.style.display = 'none');
                goToPage(1);
            }
        }

        function restartForm() {
            document.getElementById('googleForm').reset();
            document.querySelectorAll('.error-message').forEach(err => err.style.display = 'none');
            goToPage(1);
        }

        // Event listener otomatis untuk menghilangkan pesan error saat mengetik
        document.querySelectorAll('.input-underline').forEach(input => {
            input.addEventListener('input', function() {
                const errId = this.id.replace('input_', 'error_');
                const errMsg = document.getElementById(errId);
                if (errMsg && this.value.trim()) {
                    errMsg.style.display = 'none';
                }
            });
        });
    </script>
</body>
</html>
