---
layout: page
title: Contact me
subtitle:
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Me</title>
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

        input, textarea {
            margin-bottom: 15px;
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 5px;
            width: 100%;
        }

        input[type="text"], textarea {
            width: 100%;
        }

        textarea {
            height: 150px;
            resize: vertical;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: green;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            align-self: center;
        }

        button:hover {
            background-color: darkgreen;
        }

        @media (max-width: 600px) {
            .container {
                padding: 10px;
            }

            button {
                width: 100%;
            }
        }
    </style>

</head>
<body>
    <div class="container">
        <h1>Contact Me</h1>
        <form action="https://formspree.io/f/xrbzqyzl" method="POST">
            <label for="title">Title</label>
            <input type="text" id="title" name="title" required>
            <label for="message">Message</label>
            <textarea id="message" name="message" required></textarea>
            <label> Attachment if any:<input type="file" name="upload">
            </label>
            <input type="hidden" name="_replyto" value="phyuhninhtway@gmail.com">
            <input type="hidden" name="_subject" value="New Contact Form Submission">
            <button type="submit">Send</button>
        </form>
    </div>
</body>
</html>
