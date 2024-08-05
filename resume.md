---
layout: page
title: Resume
subtitle:
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RESUME PDF in HTML</title>
    <style>
        body, html {
            height: 100%;
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100%;
            padding: 10px;
            box-sizing: border-box;
        }

        .pdf {
            width: 100%;
            max-width: 1000px;
            aspect-ratio: 4 / 3;
            border: 1px solid #ccc;
        }

        h1, h3 {
            text-align: center;
            margin: 10px 0;
        }

        h1 {
            color: green;
        }

        @media (max-width: 1000px) {
            .pdf {
                width: 100%;
                height: auto;
            }
        }
    </style>

</head>
<body>
    <div class="container">
        <object class="pdf" data="/assets/pdf/Resume_Emerald_PHH_010824.pdf" type="application/pdf">
            <p>Your browser does not support PDFs. Please download the PDF to view it: <a href="/assets/pdf/Resume_Emerald_PHH_010824.pdf">Download PDF</a>.</p>
        </object>
    </div>
</body>
</html>
<!-- Full: https://github.com/EmeraldPhyu/emeraldphyu.github.io/blob/master/assets/pdf/Resume_Emerald_PHH_010824.pdf -->
<!-- Test: PDF "https://media.geeksforgeeks.org/wp-content/cdn-uploads/20210101201653/PDF.pdf" -->
