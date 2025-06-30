<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8" />
  <title>دعوة خاصة - فرقة SDF</title>
  <link href="https://fonts.googleapis.com/css2?family=UnifrakturCook:wght@700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      background-color: #000;
      font-family: 'UnifrakturCook', cursive;
      color: #ff0000;
      overflow: hidden;
      direction: rtl;
    }

    .creepy-background {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      font-size: 14px;
      color: rgba(255, 0, 0, 0.05);
      z-index: 0;
      line-height: 1.8;
      padding: 20px;
      user-select: none;
      pointer-events: none;
      white-space: pre-wrap;
      overflow: hidden;
    }

    .main-content {
      position: relative;
      z-index: 10;
      max-width: 700px;
      margin: 10vh auto;
      background: rgba(0, 0, 0, 0.85);
      border: 3px solid darkred;
      padding: 40px;
      color: #ff4444;
      box-shadow: 0 0 20px red;
      text-align: center;
      font-size: 22px;
      line-height: 2;
      border-radius: 12px;
      background-image: url("https://i.imgur.com/Fh4Xh9G.png");
      background-size: cover;
      background-position: center;
      background-blend-mode: overlay;
    }

    .buttons {
      margin-top: 30px;
    }

    .buttons button {
      background: transparent;
      border: 2px solid red;
      color: red;
      padding: 10px 30px;
      font-size: 20px;
      margin: 0 15px;
      cursor: pointer;
      transition: 0.3s;
      font-family: inherit;
    }

    .buttons button:hover {
      background: red;
      color: #000;
    }
  </style>
</head>
<body>

  <div class="creepy-background">
    الموت يقترب... الأصوات تتكرر... لا مفر... لا مفر... نحن نراقبك... لا عودة بعد الآن... هذه دعوتك الأخيرة... SDF لا ترحم... الخيانة تعني الاختفاء... كل من رفض، لم يُرَ مجددًا... الفرصة لا تأتي مرتين... لوس سانتوس لم تعد كما كانت...
  </div>

  <div class="main-content" id="invite-box">
    <h2>رسالة مشفّرة للغاية</h2>
    <p style="white-space: pre-line; text-align: right;">
      تصنيف: سري للغاية<br>
      جهة الإصدار: وحدة الردع الخاصة - SDF<br><br>
      &#x2713; تم التأكد من هويتك<br>
      &#x2713; تم مطابقة سجلّك<br>
      &#x2713; تم رصد نشاطك الأخير<br><br>
      بناءً على تقييم الأوامر العليا، تم اختيارك للالتحاق بـ "وحدة الردع الخاصة – SDF".<br>
      طبيعة المهام غير قابلة للنقاش. موقع التنفيذ غير قابل للنشر.<br><br>
      قبولك يُفعّل الوصول إلى المرحلة الأولى.<br>
      رفضك يُصنّف كتهديد داخلي… وستُتخذ الإجراءات تلقائيًا.<br><br>
      أمامك خيار لا ثاني له:<br>
      <strong>إما الدخول الكامل… أو التصفية الصامتة.</strong>
    </p>

    <div class="buttons">
      <button onclick="accept()">نعم، أقبل</button>
      <button onclick="reject()">لا، أرفض</button>
    </div>
  </div>

  <script>
    function accept() {
      const box = document.getElementById("invite-box");
      box.innerHTML = `
        <h2>تم القبول</h2>
        <p>
          تم تسجيل موافقتك بنجاح.<br><br>
          الموقع السري:<br>
          <strong>تحت مدينة الألعاب - لوس سانتوس 🎡</strong><br><br>
          لا تتحدث، لا تنظر للخلف... فقط تحرّك.
        </p>
      `;
    }

    function reject() {
      const box = document.getElementById("invite-box");
      box.innerHTML = `
        <h2>⚠️ تم رفض الدعوة</h2>
        <p>
          لقد اخترت أن تبتعد...<br>
          سيتم إرسال وحدة تعقّب الآن.<br><br>
          تذكّر: نحن لا ننسى، ولا نغفر.<br><br>
          👁️‍🗨️ سيتم إغلاق هذا المنفذ بعد لحظات...
        </p>
      `;
      setTimeout(() => {
        window.close();
      }, 5000);
    }
  </script>

</body>
</html>
