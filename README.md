<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Christmas Party</title>
        <link rel="stylesheet" href="styles.css">
   <style>
        body, html {
            height: 100%;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        .image-background {
            position: relative;
            width: 100%;
            height: 100%;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .image-background img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            filter: brightness(70%);
        }
        .center-text-overlay {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: white;
            text-align: center;
            padding: 20px;
            background-color: rgba(255, 28, 28, 1);
            border-radius: 10px;
        }
        .highlights-event {
          position: absolute;
          left: 24px;
          bottom: 24px;
          width: 260px;
          max-width: calc(100% - 48px);
          background: rgba(0,0,0,0.45);
          color: #fff;
          border-radius: 10px;
          overflow: hidden;
          transition: height 300ms ease, width 300ms ease, transform 300ms ease;
          box-shadow: 0 8px 20px rgba(0,0,0,0.5);
          cursor: pointer;
          padding: 0;
          height: 48px; 
        }
        .highlights-event h2 {
          margin: 0;
          font-size: 16px;
          font-weight: 700;
          padding: 12px 14px;
          color: #ffd; 
          background: linear-gradient(90deg, rgba(255,255,255,0.03), rgba(255,255,255,0.02));
        }
        .highlights-event nav {
          max-height: 0;
          opacity: 0;
          transition: opacity 250ms ease, max-height 300ms ease;
          padding: 0 14px 12px 14px;
        }
        .highlight-item {
          padding: 8px 0;
          font-size: 14px;
          border-bottom: 1px dashed rgba(255,255,255,0.06);
          transform: translateY(6px);
          opacity: 0;
          transition: transform 300ms ease, opacity 300ms ease;
        }
        .highlight-item:last-child { border-bottom: none; }
        .highlights-event:hover,
        .highlights-event:focus-within {
          height: auto;
          width: 320px;
          max-width: calc(100% - 48px);
          transform: translateY(-6px);
        }
        .highlights-event:hover nav,
        .highlights-event:focus-within nav {
          max-height: 400px;
          opacity: 1;
        }
        .highlights-event:hover .highlight-item,
        .highlights-event:focus-within .highlight-item {
          transform: translateY(0);
          opacity: 1;
        }
        @media (max-width: 520px) {
          .highlights-event { left: auto; right: 12px; bottom: 12px; width: 220px; }
          .highlights-event:hover, .highlights-event:focus-within { width: 90%; }
        }
    </style>
    </head>
    <body>
        <div class="image-background">
        <img src="https://i.ibb.co/WNV8GXgh/Screenshot-2025-10-24-215629.png" alt="background" border="0">
        </div>
        <div class="center-text-overlay">
            <h1>Join Us for a Festive Christmas Party!</h1>
            <p>Date: December 20, 2025 | Time: 7:00 PM | Venue: Downtown Community Hall</p>
            <p>Enjoy an evening of joy, laughter, and holiday cheer with friends and family. There will be food, drinks, music, and fun activities for all ages!</p>
            <p>RSVP by December 10th to ensure your spot at the celebration.</p>
            <p>We look forward to celebrating the holiday season with you!</p>
        <section class="highlights-event">
        <h2>
            Upcoming events
        </h2>
    <section class="highlights-event" tabindex="0" aria-label="Upcoming events">
        <h2>Upcoming events</h2>
    <nav aria-hidden="false">
      <div class="highlight-item">Funtime games</div>
      <div class="highlight-item">Delicious food</div>
      <div class="highlight-item">Great music</div>
      <div class="highlight-item">Dance competition</div>
        </nav>
        </section>
        </div>
    </body>
</html>
    
    
