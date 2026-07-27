# html-12
<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mini-Loyiha 1: HTML Jadvallar</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f4f7f6;
      padding: 30px;
      color: #333;
    }

    h1 {
      text-align: center;
      color: #2c3e50;
      margin-bottom: 30px;
    }

    /* 1. Asosiy Jadval Stillari */
    table {
      width: 100%;
      max-width: 900px;
      margin: 0 auto 40px auto;
      border-collapse: collapse; /* border-collapse sharti */
      background-color: #ffffff;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
      border-radius: 8px;
      overflow: hidden;
    }

    /* Caption (Jadval nomi) */
    caption {
      font-size: 1.3rem;
      font-weight: bold;
      margin-bottom: 12px;
      color: #2c3e50;
      text-align: left;
    }

    /* th uchun alohida stil */
    th {
      background-color: #3498db;
      color: #ffffff;
      padding: 14px 16px;
      text-align: left;
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    /* td uchun alohida stil */
    td {
      padding: 12px 16px;
      border-bottom: 1px solid #eef2f5;
      font-size: 0.95rem;
      color: #555555;
    }

    /* tr:nth-child(even) - Alternativ (Zebra) ranglar */
    tbody tr:nth-child(even) {
      background-color: #f8fbfd;
    }

    /* Hover effekti tr:hover */
    tbody tr:hover {
      background-color: #eaf4fb;
      transition: background-color 0.2s ease-in-out;
    }

    /* Murakkab jadval uchun qo'shimcha bezak */
    .total-row {
      font-weight: bold;
      background-color: #e8f4fc !important;
      color: #2c3e50;
    }
  </style>
</head>
<body>

  <h1>HTML Jadvallar Topshirig'i</h1>

  <!-- 1-JADVAL: Oddiy jadval -->
  <table>
    <caption>1. Haftalik Dars Jadvali (Oddiy Jadval)</caption>
    <thead>
      <tr>
        <th>Kun</th>
        <th>1-dars</th>
        <th>2-dars</th>
        <th>3-dars</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Dushanba</td>
        <td>HTML / CSS</td>
        <td>Matematika</td>
        <td>Ingliz tili</td>
      </tr>
      <tr>
        <td>Seshanba</td>
        <td>JavaScript</td>
        <td>Fizika</td>
        <td>Tarix</td>
      </tr>
      <tr>
        <td>Chorshanba</td>
        <td>Python</td>
        <td>HTML / CSS</td>
        <td>Matematika</td>
      </tr>
      <tr>
        <td>Payshanba</td>
        <td>Ingliz tili</td>
        <td>JavaScript</td>
        <td>Informatika</td>
      </tr>
      <tr>
        <td>Juma</td>
        <td>Loyiha ishi</td>
        <td>Python</td>
        <td>Kiberxavfsizlik</td>
      </tr>
    </tbody>
  </table>


  <!-- 2-JADVAL: Murakkab jadval (colspan va rowspan ishlatilgan) -->
  <table>
    <caption>2. Oylik Sotuv Hisoboti (Murakkab Jadval)</caption>
    <thead>
      <tr>
        <th>Kategoriya</th>
        <th>Mahsulot</th>
        <th>Chorak 1</th>
        <th>Chorak 2</th>
        <th>Jami Sotuv</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <!-- rowspan - 2 ta qatorni birlashtirish -->
        <td rowspan="2">Elektronika</td>
        <td>Noutbuk</td>
        <td>$12,000</td>
        <td>$15,000</td>
        <td>$27,000</td>
      </tr>
      <tr>
        <td>Smarfon</td>
        <td>$8,500</td>
        <td>$10,200</td>
        <td>$18,700</td>
      </tr>
      <tr>
        <td rowspan="2">Maishiy Texnika</td>
        <td>Muzlatgich</td>
        <td>$5,000</td>
        <td>$6,100</td>
        <td>$11,100</td>
      </tr>
      <tr>
        <td>KIR yuvish mashinasi</td>
        <td>$4,200</td>
        <td>$4,800</td>
        <td>$9,000</td>
      </tr>
      <tr class="total-row">
        <!-- colspan - 4 ta ustunni birlashtirish -->
        <td colspan="4">Umumiy Tushum:</td>
        <td>$65,800</td>
      </tr>
    </tbody>
  </table>

</body>
</html>
