<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>📖 Library Session Invitation</title>
  <style>
    /* 🌤 Warm Vintage Theme */
    body {
      font-family: 'Georgia', serif;
      background: linear-gradient(135deg, #f3e5ab 0%, #f7ecd1 100%);
      color: #3b2f2f;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .envelope {
      background-color: #fffaf0;
      padding: 40px 45px;
      border-radius: 18px;
      box-shadow: 0 6px 20px rgba(80, 60, 40, 0.25);
      max-width: 550px;
      width: 90%;
      border: 2px solid #d4b483;
      background-image: radial-gradient(#f2e6c5 1px, transparent 1px);
      background-size: 10px 10px;
      position: relative;
      animation: fadeIn 1.2s ease-out;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* Decorative header ribbon */
    .ribbon {
      position: absolute;
      top: -10px;
      left: 50%;
      transform: translateX(-50%);
      background-color: #c29a6a;
      color: #fffaf0;
      padding: 6px 20px;
      border-radius: 6px;
      font-family: 'Trebuchet MS', sans-serif;
      font-weight: bold;
      letter-spacing: 0.5px;
      box-shadow: 0 3px 6px rgba(0,0,0,0.2);
    }

    h1 {
      font-family: 'Playfair Display', Georgia, serif;
      font-size: 2.1em;
      margin-top: 15px;
      color: #4a3728;
    }

    h2 {
      font-family: 'Courier New', monospace;
      font-weight: normal;
      color: #7b614f;
      font-size: 1.2em;
      margin-top: -5px;
      margin-bottom: 20px;
    }

    .details {
      text-align: left;
      margin-top: 25px;
      background: rgba(255, 245, 225, 0.7);
      border-left: 4px solid #d2a679;
      padding: 15px 20px;
      border-radius: 10px;
      font-size: 1.05em;
    }

    .details p {
      margin: 8px 0;
    }

    /* Buttons */
    .button-row {
      display: flex;
      justify-content: space-between;
      gap: 12px;
      margin-top: 30px;
    }

    .rsvp-button {
      flex-grow: 1;
      padding: 12px 0;
      border: none;
      border-radius: 8px;
      font-family: 'Trebuchet MS', sans-serif;
      font-size: 1em;
      font-weight: bold;
      cursor: pointer;
      transition: transform 0.1s ease, box-shadow 0.2s ease;
    }

    .accept {
      background-color: #b58863;
      color: #fffaf0;
      box-shadow: 0 3px 6px rgba(0,0,0,0.2);
    }

    .accept:hover {
      background-color: #a17250;
      transform: translateY(-2px);
    }

    .decline {
      background-color: #c97b63;
      color: #fffaf0;
      box-shadow: 0 3px 6px rgba(0,0,0,0.2);
    }

    .decline:hover {
      background-color: #a55b45;
      transform: translateY(-2px);
    }

    /* Footer note */
    .note {
      margin-top: 25px;
      font-style: italic;
      color: #6b5846;
      font-size: 0.95em;
    }

    /* Decorative stamp corner */
    .stamp {
      position: absolute;
      top: 20px;
      right: 25px;
      width: 50px;
      height: 50px;
      border: 2px dashed #b68d5b;
      border-radius: 8px;
      background-color: #f9e7b5;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.4em;
    }

    @media (max-width: 600px) {
      .button-row {
        flex-direction: column;
      }
    }
  </style>
</head>

<body>
  <div class="envelope">
    <div class="ribbon">Warm Invitation</div>
    <div class="stamp">📚</div>

    <h1>Library Session</h1>
    <h2>“Where caffeine meets concentration.” ☕</h2>

    <div class="details">
      <p><strong>📍 Location:</strong> National Library Malaysia, Kuala Lumpur</p>
      <p><strong>📅 Date:</strong> Tomorrow, 20 October 2025</p>
      <p><strong>🕘 Time:</strong> 8:00 AM onwards</p>
      <p><strong>🎒 Bring:</strong> Your laptop, notes & a curious mind</p>
    </div>

    <div class="button-row">
      <form action="https://formspree.io/f/xanppedv" method="POST">
        <input type="hidden" name="RSVP" value="ACCEPTED - See you at the study session!">
        <button type="submit" class="rsvp-button accept">   ✔ Count Me In!   </button>
      </form>

      <form action="https://formspree.io/f/xanppedv" method="POST">
        <input type="hidden" name="RSVP" value="DECLINED - Can’t make it this time.">
        <button type="submit" class="rsvp-button decline">   ✖ Maybe Next Time   </button>
      </form>
    </div>

    <div class="note">
      Feel free to text me if you have any questions 💬
    </div>
  </div>
</body>
</html>
