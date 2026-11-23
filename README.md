# Simple Input Form

Ek clean aur responsive HTML + CSS input form jise aap kisi bhi web project ya practice page mein directly use kar sakte hain.

## Features
- Dark mode layout with clean focus states
- Name, Email, aur Message input fields
- Built-in HTML5 form validation (`required`, `type="email"`)

## Code (`index.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Simple Input Form</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: system-ui, -apple-system, sans-serif;
    }

    body {
      min-height: 100vh;
      display: grid;
      place-items: center;
      background: #0f172a;
      color: #f8fafc;
      padding: 16px;
    }

    .form-box {
      width: 100%;
      max-width: 400px;
      background: #1e293b;
      padding: 24px;
      border-radius: 12px;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.35);
    }

    .form-box h2 {
      margin-bottom: 18px;
      font-size: 1.35rem;
    }

    .field {
      margin-bottom: 14px;
    }

    label {
      display: block;
      margin-bottom: 6px;
      font-size: 0.9rem;
      color: #cbd5e1;
    }

    input,
    textarea {
      width: 100%;
      padding: 10px 12px;
      border-radius: 8px;
      border: 1px solid #334155;
      background: #0f172a;
      color: #f8fafc;
      font-size: 0.95rem;
      outline: none;
    }

    input:focus,
    textarea:focus {
      border-color: #38bdf8;
    }

    button {
      width: 100%;
      padding: 11px;
      border: none;
      border-radius: 8px;
      background: #38bdf8;
      color: #0f172a;
      font-weight: 600;
      font-size: 0.95rem;
      cursor: pointer;
    }

    button:hover {
      background: #0ea5e9;
    }
  </style>
</head>
<body>
  <form class="form-box">
    <h2>Contact Form</h2>

    <div class="field">
      <label for="name">Name</label>
      <input id="name" type="text" placeholder="Enter your name" required />
    </div>

    <div class="field">
      <label for="email">Email</label>
      <input id="email" type="email" placeholder="you@example.com" required />
    </div>

    <div class="field">
      <label for="message">Message</label>
      <textarea id="message" rows="3" placeholder="Write your message..."></textarea>
    </div>

    <button type="submit">Submit</button>
  </form>
</body>
</html>
```

## Usage
Is code ko `index.html` file mein save karein aur kisi bhi browser mein open kar lein.
