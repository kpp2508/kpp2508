<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ฐานข้อมูลการรับเบี้ยยังชีพ</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>ฐานข้อมูลการรับเบี้ยยังชีพของตำบลกุดยม</h1>

        <!-- Login Form -->
        <div id="login-form">
            <h2>เข้าสู่ระบบ</h2>
            <form id="login">
                <label for="username">ชื่อผู้ใช้:</label>
                <input type="text" id="username" required>
                <label for="password">รหัสผ่าน:</label>
                <input type="password" id="password" required>
                <button type="submit">เข้าสู่ระบบ</button>
            </form>
        </div>

        <!-- Data Entry Form -->
        <div id="data-form" style="display:none;">
            <h2>บันทึกข้อมูล</h2>
            <form id="data-entry">
                <label for="type">ประเภท:</label>
                <select id="type" required>
                    <option value="ผู้สูงอายุ">ผู้สูงอายุ</option>
                    <option value="ผู้พิการ">ผู้พิการ</option>
                    <option value="ผู้ป่วยเอดส์">ผู้ป่วยเอดส์</option>
                </select>

                <label for="registration-date">วันที่ลงทะเบียน:</label>
                <input type="date" id="registration-date" required>

                <label for="birth-date">วัน/เดือน/ปี เกิด:</label>
                <input type="date" id="birth-date" required>

                <label for="age">อายุ:</label>
                <input type="text" id="age" readonly>

                <label for="address">ที่อยู่:</label>
                <select id="province" required>
                    <!-- Add province options -->
                </select>

                <select id="district" required>
                    <!-- Add district options -->
                </select>

                <select id="subdistrict" required>
                    <!-- Add subdistrict options -->
                </select>

                <select id="village" required>
                    <!-- Add village options -->
                </select>

                <label for="disability-type">พิการประเภท:</label>
                <select id="disability-type">
                    <option value="พิการทางการเห็น">พิการทางการเห็น</option>
                    <option value="พิการทางการได้ยินหรือสื่อความหมาย">พิการทางการได้ยินหรือสื่อความหมาย</option>
                    <option value="พิการทางการเคลื่อนไหวหรือทางร่างกาย">พิการทางการเคลื่อนไหวหรือทางร่างกาย</option>
                    <option value="พิการจิตใจหรือพฤติกรรม">พิการจิตใจหรือพฤติกรรม</option>
                    <option value="พิการทางสติปัญญา">พิการทางสติปัญญา</option>
                    <option value="พิการทางการเรียนรู้">พิการทางการเรียนรู้</option>
                    <option value="พิการทางการออทิสติก">พิการทางการออทิสติก</option>
                </select>

                <label for="phone">เบอร์โทรติดต่อ:</label>
                <input type="tel" id="phone" required>

                <label for="status">สถานะ:</label>
                <select id="status">
                    <option value="ปกติ">ปกติ</option>
                    <option value="ถึงแก่กรรม">ถึงแก่กรรม</option>
                    <option value="ย้ายที่อยู่">ย้ายที่อยู่</option>
                </select>

                <label for="bank-name">ชื่อบัญชีธนาคาร:</label>
                <input type="text" id="bank-name">

                <label for="bank-account">เลขที่บัญชีธนาคาร:</label>
                <input type="text" id="bank-account">

                <button type="submit">บันทึกข้อมูล</button>
            </form>
        </div>

        <!-- Report Section -->
        <div id="report-section" style="display:none;">
            <h2>รายงานข้อมูล</h2>
            <!-- Add report options here -->
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>

