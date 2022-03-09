# Monito

หน้ากากระบบ Back Office หรือ Dashboard สำหรับใช้ในองค์กร เพื่อให้รูปแบบและประสบการณ์การใช้งานของผู้ใช้เป็นไปในทิศทางเดียวกัน ภาษาที่ใช้มี HTML, CSS, jQuery โดยใช้ [Bootstrap 4](https://getbootstrap.com) เป็น framework ในการพัฒนา

### Demo
> https://monito.tech

### Documentation
> https://zeroheight.com/914352caa

## โครงสร้างไฟล์

>>>
root
- :file_folder: assets สำหรับเก็บ resource
- :file_folder: pages สำหรับเก็บ template
- :file_folder: uploads สำหรับเก็บสิ่งที่ผู้ใช้งานอัปโหลดจากระบบ
- :file_folder: scss สำหรับเก็บไฟล์ scss ก่อนที่จะ compile
>>>


## การใช้งาน

1. เลือก template ที่ต้องการได้จากโฟลเดอร์ **pages**
2. วางไฟล์ css ที่ปรับแต่งไว้แล้วที่โฟลเดอร์ **assets >> css >> theme**
3. ปรับแต่ง theme ตามวิธีการด้านล่าง

#### Header
แก้ไข favicon

```html
<!-- Favicon -->
<link rel="icon" type="image/png" href="../../assets/img/favicon/{Image file}">
```

เรียกไฟล์ theme css ที่ต้องการใช้

```html
<!-- Custom CSS -->
<link rel="stylesheet" type="text/css" href="../../assets/css/theme/{CSS file}">
```

#### Footer
แก้ไขลิงก์ของ copyright หากไม่มีลิงก์ให้ใส่ '#'

```html
<a href="{Link}" class="font-weight-bold ml-1 link" title="" target="_blank"></a>
```

#### Content
ในส่วนของ content สามารถจัดการ layout และ coding ได้ในส่วนนี้

```html
<!-- ========================= Page content ===============================   -->
            <div class="container-content">
                <div class="example">Input content HERE !</div>
            </div>
<!-- ========================= End Page content =============================   -->
```

## การปรับแต่ง CSS
ในส่วนของการปรับแต่ง css นั้น ให้ใช้การเปลี่ยนค่าตัวแปรของ css ในไฟล์ตามตัวอย่างด้านล่าง

```css
:root {
    --primary-color: #5512d5;
    --secondary-color: #97999b;
    --tertiary-color: #01f59d;
    --text-secondary-color: #ffffff;
    --copyright-year: '2020';
    --copyright-brand: 'Lucky Leasing';
    --logo-brand: url("../../img/logo/lucky-logo.svg");
}
```




