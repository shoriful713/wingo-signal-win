<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Wingo Signal Bot</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 50px;
      background-color: #f7f7f7;
    }
    h1 {
      color: #ff6600;
    }
    #signal {
      font-size: 2em;
      color: green;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <h1>Wingo Signal Bot</h1>
  <p>সর্বশেষ সিগন্যাল:</p>
  <div id="signal">লোড হচ্ছে...</div>

  <script>
    // ডেমো সিগন্যাল (পরে রিয়েল টাইমে সংযুক্ত করা যাবে)
    const signals = ["Green 3 Small", "Red 6 Big", "Violet 0"];
    let i = 0;

    setInterval(() => {
      document.getElementById("signal").innerText = signals[i % signals.length];
      i++;
    }, 30000); // প্রতি ৩০ সেকেন্ডে সিগন্যাল বদলাবে
  </script>
</body>
</html>
