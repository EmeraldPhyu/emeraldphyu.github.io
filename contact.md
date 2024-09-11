---
layout: page
title: Contact me
subtitle:
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body, html {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            box-sizing: border-box;
        }

        .container {
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
        }

        h1 {
            text-align: center;
            color: #333;
        }

        form {
            display: flex;
            flex-direction: column;
        }

        label {
            margin-bottom: 5px;
            font-weight: bold;
            color: #333;
        }

        input, textarea, button {
            margin-bottom: 15px;
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 5px;
            width: 100%;
        }

        input[type="file"] {
            padding: 5px;
        }

        textarea {
            height: 150px;
            resize: vertical;
        }

        .buttons {
            display: flex;
            justify-content: space-between;
            gap: 10px; /* Add space between the buttons */
        }

        button {
            font-size: 16px;
            color: white;
            background-color: #404040;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            flex: 1;
        }

        button.clear {
            background-color: #c4c2c2;
        }

        button:hover {
            opacity: 0.9;
        }

        @media (max-width: 600px) {
            .container {
                padding: 10px;
            }

            button {
                width: 100%;
            }

            .buttons {
                flex-direction: column;
            }

            button + button {
                margin-top: 10px;
            }
        }
    </style>

</head>
<body>
    <div class="container">
        <form id="contact-form" action="https://formspree.io/f/xrbzqyzl" method="POST">
            <label for="title">Title</label>
            <input type="text" id="title" name="title" required>
            <label for="message">Message</label>
            <textarea id="message" name="message" required> Or You may leave your contact! </textarea>
            <label for="contact">Leave your contact</label>
            <input type="text" id="contact" name="contact">
            <!-- <label for="attachment">Attachment</label>
            <input type="file" id="attachment" name="attachment"> -->
            <input type="hidden" name="_replyto" value="phyuhninhtway@gmail.com">
            <input type="hidden" name="_subject" value="New Contact Form Submission">
            <div class="buttons">
                <button type="submit">Send</button>
                <button type="button" class="clear" onclick="clearForm()">Clear</button>
            </div>
        </form>
    </div>
    <script>
        function clearForm() {
            document.getElementById('contact-form').reset();
        }
    </script>
</body>
</html>
