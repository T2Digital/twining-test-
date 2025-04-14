<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>احجز خدمة تنظيف احترافية في دقائق | توينينج للنظافة</title>
    <meta name="description" content="احصل على خدمات تنظيف شاملة ومميزة للمنازل والمكاتب من توينينج. أسعار تنافسية، حجز سهل، جودة عالية، وخدمة عملاء ممتازة. احجز الآن عبر واتساب.">
    <meta name="keywords" content="تنظيف منازل, تنظيف مكاتب, شركة نظافة, حجز تنظيف, تنظيف شامل, توينينج للنظافة">
    <meta name="robots" content="index, follow">
    <style>
        html { scroll-behavior: smooth; }
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            direction: rtl;
            background: #e0f7fa;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 90%;
            max-width: 400px;
            margin: 20px auto;
            padding: 20px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(0,0,0,0.1);
        }
        select, input, textarea, button {
            width: 100%;
            padding: 10px;
            margin-top: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }
        .logo {
            width: 100px;
            height: auto;
            margin-bottom: 10px;
        }
        .serviceItem {
            border: 1px solid #ddd;
            border-radius: 5px;
            padding: 10px;
            margin-top: 10px;
            background: #f9f9f9;
        }
        .note {
            background: #fffae6;
            padding: 10px;
            border: 1px dashed #e0c200;
            margin-top: 10px;
            border-radius: 5px;
        }
        .success-message {
            color: green;
            font-weight: bold;
            margin-top: 15px;
        }
        @media (max-width: 480px) {
            .container { padding: 15px; }
            select, input, textarea, button { font-size: 14px; }
        }
    </style>
</head>
<body>
<div class="container">
    <img src="https://i.postimg.cc/bvjDNQ0j/Whats-App-Image-2025-04-07-at-21-17-23-e65cadc5-removebg-preview.png" alt="شعار الشركة" class="logo">
    <h2>طلب خدمة - توينينج لخدمات النظافة</h2>
    <div id="servicesContainer">
        <div class="serviceItem">
            <label>اختر الخدمة</label>
            <select class="service" onchange="calculatePrice()">

                <option value="35">خدمة تنظيف عميق - 35 جنيه للمتر</option>
                <option value="50">تنظيف ما بعد البناء والتشطيب - 50 جنيه للمتر</option>
                <option value="75">تنظيف شلتة الالياف الصناعية - 75 جنيه</option>
                <option value="75">تنظيف موكيت عادى - 75 جنيه للمتر</option>
                <option value="75">تنظيف موكيت فايير - 75 جنيه للمتر</option>
                <option value="75">تنظيف مخدات الكنب - 75 جنيه للواحدة</option>
                <option value="600">تنظيف كنبة ٢ مقعد - 600 جنيه</option>
                <option value="750">تنظيف كنبة ٣ مقعد - 750 جنيه</option>
                <option value="1400">تنظيف كتبة حرف ( L) - 1400 جنيه</option>
                <option value="75">تنظيف مخدات صغيرة - 75 جنيه للواحدة</option>
                <option value="100">تنظيف مخدات كبيرة - 100 جنيه للواحدة</option>
                <option value="250">تنظيف كرسى انتيريه - 250 جنيه</option>
                <option value="200">تنظيف كرسى صالون يد خشب - 200 جنيه</option>
                <option value="450">تنظيف فوتیه - 450 جنيه</option>
                <option value="300">تنظيف كرسي عثمانى - 300 جنيه</option>
                <option value="150">تنظيف كرسى سفره ظهر وقاعدة - 150 جنيه</option>
                <option value="100">تنظيف كرسى سفرة قاعدة فقط - 100 جنيه</option>
                <option value="100">تنظيف كرسى بدون ذراع وظهر - 100 جنيه</option>
                <option value="300">تنظيف شاذلونج - 300 جنيه</option>
                <option value="200">تنظيف كرسى هزاز - 200 جنيه</option>
                <option value="900">تنظيف مرتبة كيتج ٢م - 900 جنيه</option>
                <option value="800">تنظيف مرتبة ديل ١٨٠ سم - 800 جنيه</option>
                <option value="700">تنظيف مرتبة كوين ١٦٠ سم - 700 جنيه</option>
                <option value="700">تنظيف مرتبة سنجل ١٤٠ سم - 700 جنيه</option>
                <option value="150">تنظيف شباك غرفة الوميتال - 150 جنيه</option>
                <option value="300">تنظيف باب بلكونة الوميتال - 300 جنيه</option>
                <option value="750">التنظيف اليومى المنتظم (10ص - 6م) بدون أدوات - 750 جنيه</option>            </select>
            <input type="number" class="area" placeholder="العدد أو المساحة" oninput="calculatePrice()">
            <button onclick="removeService(this)">❌ حذف</button>
        </div>
    </div>
    <button onclick="addService()">➕ إضافة خدمة أخرى</button>
    <p>💰 السعر الإجمالي: <span id="totalPrice">0</span> جنيه</p>

    <input type="text" id="name" placeholder="الاسم" required>
    <input type="tel" id="phone" placeholder="رقم الهاتف" required>
    <input type="text" id="address" placeholder="العنوان بالتفصيل" required>
    <label for="date">📅 تاريخ الحجز</label>
    <input type="date" id="date" required>
    <select id="gender" required>
        <option value="ذكر">ذكر</option>
        <option value="أنثى">أنثى</option>
    </select>
    <textarea id="notes" placeholder="ملاحظات إضافية"></textarea>
    <div class="note">
        💵 يجب دفع نصف قيمة الطلب مقدمًا (أي <span id="halfPrice">0</span> جنيه) <br>
        يرجى التحويل على رقم محفظة <strong>01116199928</strong> ورفع صورة إثبات الدفع.
    </div>
    <input type="file" id="paymentProof" accept="image/*" required>
    <button onclick="getLocation()">📍 مشاركة الموقع</button>
    <input type="text" id="location" placeholder="موقعك" readonly>
    <button onclick="validateAndSubmit()">📲 تأكيد الحجز</button>
    <p id="successMessage" class="success-message" style="display:none;">تم تأكيد الحجز و شكرا لإختيارك شركة توينينج لخدمات النظافة 🌟</p>
</div>

<script>
function calculatePrice() {
    let total = 0;
    const services = document.querySelectorAll('.service');
    const areas = document.querySelectorAll('.area');
    for (let i = 0; i < services.length; i++) {
        const price = parseFloat(services[i].value);
        const amount = parseFloat(areas[i].value) || 0;
        total += price * amount;
    }
    document.getElementById('totalPrice').innerText = total;
    document.getElementById('halfPrice').innerText = Math.ceil(total / 2);
}

function addService() {
    const container = document.getElementById('servicesContainer');
    const newService = container.firstElementChild.cloneNode(true);
    newService.querySelector('.area').value = '';
    container.appendChild(newService);
}

function removeService(btn) {
    const container = document.getElementById('servicesContainer');
    if (container.children.length > 1) btn.parentElement.remove();
}

function getLocation() {
    if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(function(position) {
            const lat = position.coords.latitude;
            const lon = position.coords.longitude;
            document.getElementById('location').value = `https://www.google.com/maps?q=${lat},${lon}`;
        }, function(error) {
            alert("فشل في الحصول على الموقع. الرجاء التأكد من تفعيل GPS أو المحاولة لاحقًا.");
        });
    } else {
        alert("المتصفح لا يدعم مشاركة الموقع.");
    }
}

function validateAndSubmit() {
    const proofInput = document.getElementById('paymentProof');
    if (!proofInput.files.length) {
        alert("يجب رفع صورة إثبات الدفع لتأكيد الحجز.");
        return;
    }
    const proofURL = URL.createObjectURL(proofInput.files[0]);
    sendWhatsApp(proofURL);
    sendEmail(proofURL);
    document.getElementById('successMessage').style.display = 'block';
}

function sendWhatsApp(proofURL) {
    const name = document.getElementById('name').value;
    const phone = document.getElementById('phone').value;
    const address = document.getElementById('address').value;
    const date = document.getElementById('date').value;
    const gender = document.getElementById('gender').value;
    const notes = document.getElementById('notes').value;
    const location = document.getElementById('location').value;
    let services = document.querySelectorAll('.service');
    let areas = document.querySelectorAll('.area');
    let serviceText = '';
    for (let i = 0; i < services.length; i++) {
        const label = services[i].selectedOptions[0].text;
        const qty = areas[i].value;
        serviceText += `\n- ${label} × ${qty}`;
    }
    const total = document.getElementById('totalPrice').innerText;
    const half = document.getElementById('halfPrice').innerText;
    const message = `🔹 اسم العميل: ${name}\n📞 رقم الهاتف: ${phone}\n📍 العنوان: ${address}\n📅 التاريخ: ${date}\n👤 النوع: ${gender}\n\n🧹 الخدمات:${serviceText}\n💰 الإجمالي: ${total} جنيه\n💵 نصف القيمة: ${half} جنيه\n📍 موقعك: ${location}\n📝 ملاحظات: ${notes}\n🖼️ رابط صورة الدفع: ${proofURL}`;
    const url = `https://wa.me/201116199928?text=${encodeURIComponent(message)}`;
    window.open(url, '_blank');
}

function sendEmail(proofURL) {
    const name = document.getElementById('name').value;
    const phone = document.getElementById('phone').value;
    const address = document.getElementById('address').value;
    const date = document.getElementById('date').value;
    const gender = document.getElementById('gender').value;
    const notes = document.getElementById('notes').value;
    const location = document.getElementById('location').value;
    const total = document.getElementById('totalPrice').innerText;
    let services = document.querySelectorAll('.service');
    let areas = document.querySelectorAll('.area');
    let serviceText = '';
    for (let i = 0; i < services.length; i++) {
        const label = services[i].selectedOptions[0].text;
        const qty = areas[i].value;
        serviceText += `\n- ${label} × ${qty}`;
    }
    const body = `اسم العميل: ${name}\nرقم الهاتف: ${phone}\nالعنوان: ${address}\nتاريخ الحجز: ${date}\nالنوع: ${gender}\nالخدمات:${serviceText}\nالإجمالي: ${total} جنيه\nملاحظات: ${notes}\nموقع العميل: ${location}\nرابط إثبات الدفع: ${proofURL}`;
    window.location.href = `mailto:info@twiningcleaning.com?subject=طلب حجز تنظيف من ${name}&body=${encodeURIComponent(body)}`;
}
</script>
</body>
</html>
