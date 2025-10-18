<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tarefacil - Herramientas PDF</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/pdf-lib/1.17.1/pdf-lib.min.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            min-height: 100vh;
            padding: 20px;
        }

        .header {
            text-align: center;
            color: white;
            padding: 40px 20px;
            margin-bottom: 40px;
        }

        .logo {
            font-size: 3rem;
            font-weight: 700;
            letter-spacing: -2px;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }

        .tagline {
            font-size: 1.1rem;
            opacity: 0.95;
            font-weight: 300;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }

        .tool-card {
            background: white;
            border-radius: 20px;
            padding: 40px 30px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
        }

        .tool-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 50px rgba(0,0,0,0.15);
        }

        .tool-icon {
            font-size: 4rem;
            margin-bottom: 20px;
            text-align: center;
        }

        .tool-title {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 10px;
            text-align: center;
            color: #667eea;
        }

        .tool-description {
            text-align: center;
            color: #666;
            font-size: 0.95rem;
            line-height: 1.5;
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.7);
            z-index: 1000;
            padding: 20px;
            overflow-y: auto;
        }

        .modal.active {
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            background: white;
            border-radius: 20px;
            padding: 40px;
            max-width: 700px;
            width: 100%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
            animation: slideUp 0.3s ease;
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .close-btn {
            position: absolute;
            top: 20px;
            right: 20px;
            background: #f0f0f0;
            border: none;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            font-size: 1.5rem;
            cursor: pointer;
            transition: background 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .close-btn:hover {
            background: #e0e0e0;
        }

        .modal-title {
            font-size: 2rem;
            font-weight: 600;
            margin-bottom: 30px;
            color: #667eea;
            text-align: center;
        }

        .upload-area {
            border: 3px dashed #ddd;
            border-radius: 15px;
            padding: 60px 30px;
            text-align: center;
            background: #fafafa;
            transition: all 0.3s ease;
            cursor: pointer;
            margin-bottom: 30px;
        }

        .upload-area:hover {
            border-color: #667eea;
            background: #f5f5ff;
        }

        .upload-area.dragover {
            border-color: #667eea;
            background: #e8ebff;
            transform: scale(1.02);
        }

        .upload-icon {
            font-size: 4rem;
            margin-bottom: 15px;
        }

        .upload-text {
            font-size: 1.1rem;
            color: #333;
            margin-bottom: 8px;
            font-weight: 500;
        }

        .upload-hint {
            font-size: 0.9rem;
            color: #999;
        }

        input[type="file"] {
            display: none;
        }

        .file-list {
            margin-bottom: 25px;
            background: #fafafa;
            border-radius: 12px;
            overflow: hidden;
            max-height: 300px;
            overflow-y: auto;
        }

        .file-item {
            padding: 18px 20px;
            border-bottom: 1px solid #eee;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: white;
            transition: background 0.2s;
        }

        .file-item:hover {
            background: #f9f9f9;
        }

        .file-item:last-child {
            border-bottom: none;
        }

        .file-info {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .file-icon {
            font-size: 1.5rem;
        }

        .file-name {
            font-size: 0.95rem;
            color: #333;
            font-weight: 500;
        }

        .remove-btn {
            background: #fee;
            border: none;
            color: #e53e3e;
            cursor: pointer;
            font-size: 1.3rem;
            padding: 8px 12px;
            border-radius: 8px;
            transition: all 0.2s;
            font-weight: bold;
        }

        .remove-btn:hover {
            background: #fcc;
        }

        .action-btn {
            width: 100%;
            padding: 18px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            border-radius: 12px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);
        }

        .action-btn:hover:not(:disabled) {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(102, 126, 234, 0.5);
        }

        .action-btn:disabled {
            background: #ddd;
            cursor: not-allowed;
            color: #999;
            box-shadow: none;
        }

        .status {
            text-align: center;
            margin-top: 20px;
            padding: 15px;
            border-radius: 10px;
            font-size: 0.95rem;
            font-weight: 500;
        }

        .status.success {
            background: #d4edda;
            color: #155724;
        }

        .status.error {
            background: #f8d7da;
            color: #721c24;
        }

        .status.loading {
            background: #d1ecf1;
            color: #0c5460;
        }

        .hidden {
            display: none;
        }

        .footer {
            text-align: center;
            color: white;
            padding: 30px;
            opacity: 0.9;
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            .tools-grid {
                grid-template-columns: 1fr;
            }
            
            .modal-content {
                padding: 30px 20px;
            }
            
            .logo {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="header">
        <div class="logo">✨ tarefacil</div>
        <div class="tagline">Herramientas PDF simples y poderosas</div>
    </div>

    <div class="container">
        <div class="tools-grid">
            <div class="tool-card" onclick="openModal('merge')">
                <div class="tool-icon">📑</div>
                <div class="tool-title">Unir PDFs</div>
                <div class="tool-description">Combina múltiples archivos PDF en uno solo de forma rápida y sencilla</div>
            </div>

            <div class="tool-card" onclick="openModal('convert')">
                <div class="tool-icon">🖼️</div>
                <div class="tool-title">Imágenes a PDF</div>
                <div class="tool-description">Convierte tus imágenes JPG, PNG o WEBP en documentos PDF profesionales</div>
            </div>
        </div>
    </div>

    <!-- Modal Unir PDFs -->
    <div class="modal" id="mergeModal">
        <div class="modal-content">
            <button class="close-btn" onclick="closeModal('merge')">×</button>
            <h2 class="modal-title">📑 Unir PDFs</h2>

            <div class="upload-area" id="mergeUploadArea">
                <div class="upload-icon">📄</div>
                <div class="upload-text">Arrastra tus PDFs aquí</div>
                <div class="upload-hint">o haz clic para seleccionar archivos</div>
                <input type="file" id="mergeFileInput" accept=".pdf" multiple>
            </div>

            <div class="file-list hidden" id="mergeFileList"></div>

            <button class="action-btn" id="mergeBtn" disabled>Unir PDFs</button>
            
            <div class="status hidden" id="mergeStatus"></div>
        </div>
    </div>

    <!-- Modal Convertir Imágenes -->
    <div class="modal" id="convertModal">
        <div class="modal-content">
            <button class="close-btn" onclick="closeModal('convert')">×</button>
            <h2 class="modal-title">🖼️ Imágenes a PDF</h2>

            <div class="upload-area" id="convertUploadArea">
                <div class="upload-icon">🎨</div>
                <div class="upload-text">Arrastra tus imágenes aquí</div>
                <div class="upload-hint">JPG, PNG, WEBP - o haz clic para seleccionar</div>
                <input type="file" id="convertFileInput" accept="image/*" multiple>
            </div>

            <div class="file-list hidden" id="convertFileList"></div>

            <button class="action-btn" id="convertBtn" disabled>Convertir a PDF</button>
            
            <div class="status hidden" id="convertStatus"></div>
        </div>
    </div>

    <div class="footer">
        Hecho con ❤️ | Todas las operaciones se realizan en tu navegador - tus archivos permanecen privados
    </div>

    <script>
        const { PDFDocument, rgb } = PDFLib;
        
        // Variables globales
        let mergeFiles = [];
        let convertFiles = [];

        // Elementos del DOM - Merge
        const mergeModal = document.getElementById('mergeModal');
        const mergeUploadArea = document.getElementById('mergeUploadArea');
        const mergeFileInput = document.getElementById('mergeFileInput');
        const mergeFileList = document.getElementById('mergeFileList');
        const mergeBtn = document.getElementById('mergeBtn');
        const mergeStatus = document.getElementById('mergeStatus');

        // Elementos del DOM - Convert
        const convertModal = document.getElementById('convertModal');
        const convertUploadArea = document.getElementById('convertUploadArea');
        const convertFileInput = document.getElementById('convertFileInput');
        const convertFileList = document.getElementById('convertFileList');
        const convertBtn = document.getElementById('convertBtn');
        const convertStatus = document.getElementById('convertStatus');

        // Funciones de Modal
        function openModal(type) {
            if (type === 'merge') {
                mergeModal.classList.add('active');
            } else if (type === 'convert') {
                convertModal.classList.add('active');
            }
        }

        function closeModal(type) {
            if (type === 'merge') {
                mergeModal.classList.remove('active');
                mergeFiles = [];
                updateFileList('merge');
                hideStatus('merge');
            } else if (type === 'convert') {
                convertModal.classList.remove('active');
                convertFiles = [];
                updateFileList('convert');
                hideStatus('convert');
            }
        }

        // Cerrar modal al hacer clic fuera
        mergeModal.addEventListener('click', (e) => {
            if (e.target === mergeModal) closeModal('merge');
        });
        convertModal.addEventListener('click', (e) => {
            if (e.target === convertModal) closeModal('convert');
        });

        // ========== UNIR PDFs ==========

        mergeUploadArea.addEventListener('click', () => mergeFileInput.click());
        mergeUploadArea.addEventListener('dragover', (e) => {
            e.preventDefault();
            mergeUploadArea.classList.add('dragover');
        });
        mergeUploadArea.addEventListener('dragleave', () => {
            mergeUploadArea.classList.remove('dragover');
        });
        mergeUploadArea.addEventListener('drop', (e) => {
            e.preventDefault();
            mergeUploadArea.classList.remove('dragover');
            const files = Array.from(e.dataTransfer.files).filter(f => f.type === 'application/pdf');
            addFiles('merge', files);
        });
        mergeFileInput.addEventListener('change', (e) => {
            addFiles('merge', Array.from(e.target.files));
        });

        mergeBtn.addEventListener('click', async () => {
            if (mergeFiles.length < 2) {
                showStatus('merge', 'Necesitas al menos 2 archivos PDF', 'error');
                return;
            }

            mergeBtn.disabled = true;
            showStatus('merge', '⏳ Uniendo PDFs...', 'loading');

            try {
                const mergedPdf = await PDFDocument.create();

                for (const file of mergeFiles) {
                    const arrayBuffer = await file.arrayBuffer();
                    const pdf = await PDFDocument.load(arrayBuffer);
                    const copiedPages = await mergedPdf.copyPages(pdf, pdf.getPageIndices());
                    copiedPages.forEach((page) => mergedPdf.addPage(page));
                }

                const mergedPdfBytes = await mergedPdf.save();
                downloadFile(mergedPdfBytes, 'documento_unido.pdf', 'application/pdf');
                
                showStatus('merge', '✅ ¡PDF unido correctamente!', 'success');
                
                setTimeout(() => {
                    closeModal('merge');
                }, 2000);

            } catch (error) {
                showStatus('merge', '❌ Error al unir los PDFs', 'error');
                console.error(error);
            } finally {
                mergeBtn.disabled = false;
            }
        });

        // ========== CONVERTIR IMÁGENES A PDF ==========

        convertUploadArea.addEventListener('click', () => convertFileInput.click());
        convertUploadArea.addEventListener('dragover', (e) => {
            e.preventDefault();
            convertUploadArea.classList.add('dragover');
        });
        convertUploadArea.addEventListener('dragleave', () => {
            convertUploadArea.classList.remove('dragover');
        });
        convertUploadArea.addEventListener('drop', (e) => {
            e.preventDefault();
            convertUploadArea.classList.remove('dragover');
            const files = Array.from(e.dataTransfer.files).filter(f => f.type.startsWith('image/'));
            addFiles('convert', files);
        });
        convertFileInput.addEventListener('change', (e) => {
            addFiles('convert', Array.from(e.target.files));
        });

        convertBtn.addEventListener('click', async () => {
            if (convertFiles.length === 0) {
                showStatus('convert', 'Selecciona al menos una imagen', 'error');
                return;
            }

            convertBtn.disabled = true;
            showStatus('convert', '⏳ Convirtiendo imágenes a PDF...', 'loading');

            try {
                const pdfDoc = await PDFDocument.create();

                for (const file of convertFiles) {
                    const arrayBuffer = await file.arrayBuffer();
                    let image;

                    if (file.type === 'image/png') {
                        image = await pdfDoc.embedPng(arrayBuffer);
                    } else if (file.type === 'image/jpeg' || file.type === 'image/jpg') {
                        image = await pdfDoc.embedJpg(arrayBuffer);
                    } else {
                        // Para otros formatos, convertir a canvas y luego a JPG
                        const img = await createImageBitmap(new Blob([arrayBuffer]));
                        const canvas = document.createElement('canvas');
                        canvas.width = img.width;
                        canvas.height = img.height;
                        const ctx = canvas.getContext('2d');
                        ctx.drawImage(img, 0, 0);
                        const jpgData = await new Promise(resolve => {
                            canvas.toBlob(blob => blob.arrayBuffer().then(resolve), 'image/jpeg', 0.95);
                        });
                        image = await pdfDoc.embedJpg(jpgData);
                    }

                    const page = pdfDoc.addPage([image.width, image.height]);
                    page.drawImage(image, {
                        x: 0,
                        y: 0,
                        width: image.width,
                        height: image.height,
                    });
                }

                const pdfBytes = await pdfDoc.save();
                downloadFile(pdfBytes, 'imagenes_convertidas.pdf', 'application/pdf');
                
                showStatus('convert', '✅ ¡Imágenes convertidas correctamente!', 'success');
                
                setTimeout(() => {
                    closeModal('convert');
                }, 2000);

            } catch (error) {
                showStatus('convert', '❌ Error al convertir las imágenes', 'error');
                console.error(error);
            } finally {
                convertBtn.disabled = false;
            }
        });

        // ========== FUNCIONES AUXILIARES ==========

        function addFiles(type, files) {
            if (type === 'merge') {
                mergeFiles = [...mergeFiles, ...files];
                mergeFileInput.value = '';
            } else {
                convertFiles = [...convertFiles, ...files];
                convertFileInput.value = '';
            }
            updateFileList(type);
        }

        function updateFileList(type) {
            const files = type === 'merge' ? mergeFiles : convertFiles;
            const listElement = type === 'merge' ? mergeFileList : convertFileList;
            const btn = type === 'merge' ? mergeBtn : convertBtn;

            if (files.length === 0) {
                listElement.classList.add('hidden');
                btn.disabled = true;
                return;
            }

            listElement.classList.remove('hidden');
            btn.disabled = false;

            listElement.innerHTML = files.map((file, index) => `
                <div class="file-item">
                    <div class="file-info">
                        <span class="file-icon">${type === 'merge' ? '📄' : '🖼️'}</span>
                        <span class="file-name">${file.name}</span>
                    </div>
                    <button class="remove-btn" onclick="removeFile('${type}', ${index})">×</button>
                </div>
            `).join('');
        }

        function removeFile(type, index) {
            if (type === 'merge') {
                mergeFiles.splice(index, 1);
            } else {
                convertFiles.splice(index, 1);
            }
            updateFileList(type);
        }

        function showStatus(type, message, className) {
            const statusElement = type === 'merge' ? mergeStatus : convertStatus;
            statusElement.textContent = message;
            statusElement.className = 'status ' + className;
            statusElement.classList.remove('hidden');
        }

        function hideStatus(type) {
            const statusElement = type === 'merge' ? mergeStatus : convertStatus;
            statusElement.classList.add('hidden');
        }

        function downloadFile(data, filename, mimeType) {
            const blob = new Blob([data], { type: mimeType });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = filename;
            a.click();
            URL.revokeObjectURL(url);
        }
    </script>
</body>
</html>
