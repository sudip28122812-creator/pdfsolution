<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PDF Editor Pro - Edit, Convert, Compress PDF Files Online Free</title>
    <meta name="description" content="Free online PDF editor with tools to edit, convert, compress, and secure PDF files. Split, merge, rotate PDFs and more with our easy-to-use PDF tools.">
    <meta name="keywords" content="PDF editor, edit PDF, compress PDF, convert PDF, split PDF, merge PDF, PDF to Word, Word to PDF, JPG to PDF, PDF tools, online PDF editor">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            text-align: center;
            padding: 30px 0;
            background: linear-gradient(135deg, #2c3e50, #1a2530);
            color: white;
            border-radius: 10px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        header h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
        }
        
        header p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto;
            opacity: 0.9;
        }
        
        .upload-section {
            background: white;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .upload-area {
            border: 3px dashed #3498db;
            border-radius: 10px;
            padding: 40px;
            margin: 20px auto;
            max-width: 600px;
            cursor: pointer;
            transition: all 0.3s;
            position: relative;
        }
        
        .upload-area:hover {
            background-color: #f0f8ff;
            border-color: #2980b9;
        }
        
        .upload-area i {
            font-size: 60px;
            color: #3498db;
            margin-bottom: 15px;
        }
        
        .upload-area h3 {
            margin-bottom: 10px;
            color: #2c3e50;
        }
        
        #file-input {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            opacity: 0;
            cursor: pointer;
        }
        
        .btn {
            display: inline-block;
            background: #3498db;
            color: white;
            padding: 12px 25px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
            margin: 10px 5px;
        }
        
        .btn:hover {
            background: #2980b9;
            transform: translateY(-2px);
        }
        
        .btn-donate {
            background: #e74c3c;
        }
        
        .btn-donate:hover {
            background: #c0392b;
        }
        
        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            margin-bottom: 40px;
        }
        
        .tool-category {
            background: white;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .tool-category h3 {
            color: #2c3e50;
            padding-bottom: 15px;
            margin-bottom: 20px;
            border-bottom: 2px solid #3498db;
            display: flex;
            align-items: center;
        }
        
        .tool-category h3 i {
            margin-right: 10px;
            color: #3498db;
        }
        
        .tool-item {
            display: flex;
            align-items: center;
            padding: 12px 10px;
            border-radius: 5px;
            margin-bottom: 10px;
            transition: all 0.3s;
            cursor: pointer;
        }
        
        .tool-item:hover {
            background-color: #f0f8ff;
            transform: translateX(5px);
        }
        
        .tool-item i {
            margin-right: 15px;
            width: 24px;
            text-align: center;
            color: #3498db;
        }
        
        .features {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin: 40px 0;
        }
        
        .feature {
            flex-basis: calc(33.333% - 20px);
            background: white;
            padding: 25px;
            border-radius: 10px;
            margin-bottom: 20px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            text-align: center;
        }
        
        .feature i {
            font-size: 40px;
            color: #3498db;
            margin-bottom: 15px;
        }
        
        .ad-container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            margin: 30px 0;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .ad-placeholder {
            background: #f8f9fa;
            padding: 30px;
            border: 2px dashed #ccc;
            border-radius: 5px;
            margin: 10px 0;
        }
        
        .donation-section {
            background: white;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            margin: 30px 0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .donation-section h2 {
            color: #2c3e50;
            margin-bottom: 20px;
        }
        
        .donation-options {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 20px;
        }
        
        .donation-option {
            background: #f8f9fa;
            padding: 15px 25px;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s;
            border: 1px solid #e9ecef;
        }
        
        .donation-option:hover {
            background: #e9ecef;
            transform: translateY(-3px);
        }
        
        .upload-status {
            margin-top: 20px;
            padding: 15px;
            border-radius: 5px;
            background: #f8f9fa;
            display: none;
        }
        
        .upload-success {
            background: #d4edda;
            color: #155724;
            display: block;
        }
        
        .upload-error {
            background: #f8d7da;
            color: #721c24;
            display: block;
        }
        
        .file-info {
            margin-top: 15px;
            padding: 10px;
            background: #e9ecef;
            border-radius: 5px;
            display: none;
        }
        
        footer {
            text-align: center;
            padding: 20px;
            margin-top: 40px;
            color: #7f8c8d;
            border-top: 1px solid #eee;
        }
        
        @media (max-width: 768px) {
            .features {
                flex-direction: column;
            }
            
            .feature {
                flex-basis: 100%;
            }
            
            .tools-grid {
                grid-template-columns: 1fr;
            }
            
            .donation-options {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>PDF Editor Pro</h1>
            <p>All the PDF tools you need in one place - edit, convert, optimize, and secure your documents</p>
        </header>
        
        <section class="upload-section">
            <h2>Upload Your PDF File</h2>
            <p>Get started by uploading your PDF document</p>
            
            <div class="upload-area" id="drop-area">
                <i class="fas fa-file-pdf"></i>
                <h3>Drag & Drop your PDF here</h3>
                <p>or</p>
                <button class="btn" id="browse-btn"><i class="fas fa-upload"></i> Browse Files</button>
                <input type="file" id="file-input" accept=".pdf" />
            </div>
            
            <div class="upload-status" id="upload-status"></div>
            
            <div class="file-info" id="file-info">
                <h4>Uploaded File:</h4>
                <p id="file-name"></p>
                <p id="file-size"></p>
                <button class="btn" id="remove-file"><i class="fas fa-trash"></i> Remove File</button>
            </div>
        </section>
        
        <!-- AdSense Ad Unit -->
        <div class="ad-container">
            <h3>Supported by our partners</h3>
            <div class="ad-placeholder">
                <!-- Google AdSense Code would go here -->
                <p>Google AdSense Banner Ad</p>
            </div>
        </div>
        
        <h2 style="text-align: center; margin-bottom: 30px; color: #2c3e50;">All PDF Tools</h2>
        
        <div class="tools-grid">
            <div class="tool-category">
                <h3><i class="fas fa-cut"></i> Edit Pages</h3>
                <div class="tool-item">
                    <i class="fas fa-object-group"></i>
                    <span>Split PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-trash-alt"></i>
                    <span>Remove pages</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-cut"></i>
                    <span>Extract pages</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-layer-group"></i>
                    <span>Organize PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-scanner"></i>
                    <span>Scan to PDF</span>
                </div>
            </div>
            
            <div class="tool-category">
                <h3><i class="fas fa-tachometer-alt"></i> Optimize PDF</h3>
                <div class="tool-item">
                    <i class="fas fa-compress-arrows-alt"></i>
                    <span>Compress PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-wrench"></i>
                    <span>Repair PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-language"></i>
                    <span>OCR PDF</span>
                </div>
            </div>
            
            <div class="tool-category">
                <h3><i class="fas fa-exchange-alt"></i> Convert To PDF</h3>
                <div class="tool-item">
                    <i class="fas fa-file-image"></i>
                    <span>JPG to PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-file-word"></i>
                    <span>WORD to PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-file-powerpoint"></i>
                    <span>POWERPOINT to PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-file-excel"></i>
                    <span>EXCEL to PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-code"></i>
                    <span>HTML to PDF</span>
                </div>
            </div>
            
            <div class="tool-category">
                <h3><i class="fas fa-exchange-alt"></i> Convert From PDF</h3>
                <div class="tool-item">
                    <i class="fas fa-file-image"></i>
                    <span>PDF to JPG</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-file-word"></i>
                    <span>PDF to WORD</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-file-powerpoint"></i>
                    <span>PDF to POWERPOINT</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-file-excel"></i>
                    <span>PDF to EXCEL</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-file-alt"></i>
                    <span>PDF to PDF/A</span>
                </div>
            </div>
            
            <div class="tool-category">
                <h3><i class="fas fa-edit"></i> Edit PDF</h3>
                <div class="tool-item">
                    <i class="fas fa-sync"></i>
                    <span>Rotate PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-list-ol"></i>
                    <span>Add page numbers</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-tint"></i>
                    <span>Add watermark</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-crop"></i>
                    <span>Crop PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-pencil-alt"></i>
                    <span>Edit PDF</span>
                </div>
            </div>
            
            <div class="tool-category">
                <h3><i class="fas fa-lock"></i> PDF Security</h3>
                <div class="tool-item">
                    <i class="fas fa-unlock"></i>
                    <span>Unlock PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-shield-alt"></i>
                    <span>Protect PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-signature"></i>
                    <span>Sign PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-eye-slash"></i>
                    <span>Redact PDF</span>
                </div>
                <div class="tool-item">
                    <i class="fas fa-code-compare"></i>
                    <span>Compare PDF</span>
                </div>
            </div>
        </div>
        
        <!-- AdSense Ad Unit -->
        <div class="ad-container">
            <h3>Recommended Tools</h3>
            <div class="ad-placeholder">
                <!-- Google AdSense Code would go here -->
                <p>Google AdSense Rectangle Ad</p>
            </div>
        </div>
        
        <div class="features">
            <div class="feature">
                <i class="fas fa-lock"></i>
                <h3>Secure Processing</h3>
                <p>All files are processed securely and deleted from our servers after 2 hours</p>
            </div>
            <div class="feature">
                <i class="fas fa-bolt"></i>
                <h3>Fast Processing</h3>
                <p>Advanced algorithms ensure your PDFs are processed quickly</p>
            </div>
            <div class="feature">
                <i class="fas fa-check-circle"></i>
                <h3>High Quality</h3>
                <p>Maintain the highest quality output with all our tools</p>
            </div>
        </div>
        
        <!-- Donation Section -->
        <div class="donation-section">
            <h2>Support PDF Editor Pro</h2>
            <p>Help us keep this service free by making a donation. Your support helps us maintain and improve our tools.</p>
            
            <button class="btn btn-donate"><i class="fas fa-heart"></i> Donate Now</button>
            
            <div class="donation-options">
                <div class="donation-option">$5</div>
                <div class="donation-option">$10</div>
                <div class="donation-option">$25</div>
                <div class="donation-option">Custom Amount</div>
            </div>
        </div>
        
        <footer>
            <p>© 2023 PDF Editor Pro. All rights reserved.</p>
            <p>Privacy Policy | Terms of Service | Contact Us</p>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const dropArea = document.getElementById('drop-area');
            const fileInput = document.getElementById('file-input');
            const browseBtn = document.getElementById('browse-btn');
            const uploadStatus = document.getElementById('upload-status');
            const fileInfo = document.getElementById('file-info');
            const fileName = document.getElementById('file-name');
            const fileSize = document.getElementById('file-size');
            const removeFileBtn = document.getElementById('remove-file');
            const donateBtn = document.querySelector('.btn-donate');
            
            // Open file dialog when clicking the browse button
            browseBtn.addEventListener('click', function(e) {
                e.stopPropagation();
                fileInput.click();
            });
            
            // Open file dialog when clicking the drop area
            dropArea.addEventListener('click', function(e) {
                if (e.target === dropArea) {
                    fileInput.click();
                }
            });
            
            // Handle file selection
            fileInput.addEventListener('change', function() {
                if (this.files.length > 0) {
                    handleFile(this.files[0]);
                }
            });
            
            // Drag and drop functionality
            ['dragenter', 'dragover', 'dragleave', 'drop'].forEach(eventName => {
                dropArea.addEventListener(eventName, preventDefaults, false);
            });
            
            function preventDefaults(e) {
                e.preventDefault();
                e.stopPropagation();
            }
            
            ['dragenter', 'dragover'].forEach(eventName => {
                dropArea.addEventListener(eventName, highlight, false);
            });
            
            ['dragleave', 'drop'].forEach(eventName => {
                dropArea.addEventListener(eventName, unhighlight, false);
            });
            
            function highlight() {
                dropArea.style.backgroundColor = '#e3f2fd';
                dropArea.style.borderColor = '#2196f3';
            }
            
            function unhighlight() {
                dropArea.style.backgroundColor = '';
                dropArea.style.borderColor = '#3498db';
            }
            
            dropArea.addEventListener('drop', function(e) {
                const dt = e.dataTransfer;
                const files = dt.files;
                if (files.length > 0) {
                    handleFile(files[0]);
                }
            });
            
            // Handle the uploaded file
            function handleFile(file) {
                // Check if file is PDF
                if (file.type !== 'application/pdf') {
                    uploadStatus.textContent = 'Error: Please upload a PDF file';
                    uploadStatus.className = 'upload-status upload-error';
                    return;
                }
                
                // Check file size (max 50MB)
                if (file.size > 50 * 1024 * 1024) {
                    uploadStatus.textContent = 'Error: File size exceeds 50MB limit';
                    uploadStatus.className = 'upload-status upload-error';
                    return;
                }
                
                // Display success message
                uploadStatus.textContent = 'File uploaded successfully!';
                uploadStatus.className = 'upload-status upload-success';
                
                // Display file information
                fileName.textContent = `Name: ${file.name}`;
                fileSize.textContent = `Size: ${formatFileSize(file.size)}`;
                fileInfo.style.display = 'block';
                
                // You would typically send the file to a server here
                // For this example, we'll just simulate processing
                console.log('File uploaded:', file.name);
            }
            
            // Format file size
            function formatFileSize(bytes) {
                if (bytes === 0) return '0 Bytes';
                const k = 1024;
                const sizes = ['Bytes', 'KB', 'MB', 'GB'];
                const i = Math.floor(Math.log(bytes) / Math.log(k));
                return parseFloat((bytes / Math.pow(k, i)).toFixed(2)) + ' ' + sizes[i];
            }
            
            // Remove uploaded file
            removeFileBtn.addEventListener('click', function() {
                fileInput.value = '';
                uploadStatus.textContent = '';
                uploadStatus.className = 'upload-status';
                fileInfo.style.display = 'none';
            });
            
            // Donation button
            donateBtn.addEventListener('click', function() {
                alert('Thank you for your interest in supporting us! Donation options would be shown here.');
            });
            
            // Donation options
            const donationOptions = document.querySelectorAll('.donation-option');
            donationOptions.forEach(option => {
                option.addEventListener('click', function() {
                    if (this.textContent === 'Custom Amount') {
                        const amount = prompt('Enter custom donation amount:');
                        if (amount) {
                            alert(`Thank you for donating $${amount}!`);
                        }
                    } else {
                        alert(`Thank you for donating ${this.textContent}!`);
                    }
                });
            });
            
            // Tool items functionality
            const toolItems = document.querySelectorAll('.tool-item');
            toolItems.forEach(item => {
                item.addEventListener('click', function() {
                    // Check if a file is uploaded
                    if (!fileInput.files.length) {
                        uploadStatus.textContent = 'Please upload a PDF file first';
                        uploadStatus.className = 'upload-status upload-error';
                        return;
                    }
                    
                    alert(`"${this.textContent.trim()}" tool would process your PDF`);
                });
            });
        });
    </script>
</body>
</html>
