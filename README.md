<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>📥📄 PaperPort</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #121212;
      color: #e0e0e0;
    }

    header {
      text-align: center;
      padding: 40px 20px;
      background: #1f1f1f;
      animation: fadeInDown 1s ease;
      box-shadow: 0 2px 10px rgba(0,0,0,0.5);
    }

    header h1 {
      font-size: 3rem;
      margin: 0;
      color: #90caf9;
    }

    header p {
      font-size: 1.2rem;
      color: #ccc;
      margin-top: 10px;
    }

    section {
      padding: 40px 20px;
      max-width: 700px;
      margin: auto;
      animation: fadeInUp 1s ease;
    }

    h2 {
      font-size: 2rem;
      color: #bb86fc;
      border-bottom: 2px solid #333;
      padding-bottom: 10px;
      margin-bottom: 30px;
    }

    form {
      background-color: #1f1f1f;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 0 20px rgba(0,0,0,0.2);
      animation: fadeIn 1s ease;
    }

    label {
      font-size: 1.1rem;
      display: block;
      margin-bottom: 10px;
    }

    input[type="file"] {
      padding: 10px;
      background-color: #2c2c2c;
      border: 1px solid #333;
      color: #ccc;
      border-radius: 8px;
      width: 100%;
    }

    input[type="submit"] {
      margin-top: 20px;
      padding: 12px 24px;
      font-size: 1rem;
      background-color: #03dac6;
      border: none;
      border-radius: 10px;
      color: #121212;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    input[type="submit"]:hover {
      background-color: #00bfa5;
    }

    p {
      margin-top: 20px;
      font-size: 0.95rem;
      color: #aaa;
    }

    /* Image Upload Preview Simulation */
    .image-preview {
      margin-top: 40px;
      text-align: center;
      padding: 20px;
      border: 2px dashed #444;
      border-radius: 10px;
      background-color: #1a1a1a;
      animation: fadeIn 1.5s ease;
    }

    .image-preview img {
      width: 200px;
      height: auto;
      opacity: 0.7;
    }

    .image-preview p {
      margin-top: 10px;
      font-size: 0.9rem;
      color: #666;
    }

    /* Animations */
    @keyframes fadeInDown {
      from { opacity: 0; transform: translateY(-30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

  </style>
</head>
<body>

  <!-- Website Logo and Title -->
  <header>
    <h1>📥📄 PaperPort</h1>
    <p>Your gateway to organizing research papers</p>
  </header>

  <!-- Import Papers Section -->
  <section>
    <h2>Import Papers</h2>

    <!-- File Upload Form -->
    <form action="/upload" method="post" enctype="multipart/form-data">
      <label for="paperUpload">Select a paper to upload:</label>
      <input type="file" id="paperUpload" name="paperUpload" accept=".pdf,.doc,.docx,.txt,.png,.jpg,.jpeg"><br>
      <input type="submit" value="Upload Paper">
    </form>

    <!-- Info -->
    <p>Supported formats: PDF, DOC, DOCX, TXT, PNG, JPG</p>

    <!-- Image Preview Simulation -->
    <div class="image-preview">
      <img src="https://via.placeholder.com/200x150?text=Image+Preview" alt="Preview">
      <p>Your uploaded image will appear here</p>
    </div>
  </section>

</body>
</html>
